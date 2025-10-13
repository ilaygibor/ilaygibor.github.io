import { motion } from "framer-motion";
import { ArrowRight, Github, Mail, Microscope, Cpu, Bot, GitBranch } from "lucide-react";
import { Button } from "@/components/ui/button";
import { Card, CardContent, CardHeader, CardTitle, CardDescription } from "@/components/ui/card";
import { Badge } from "@/components/ui/badge";

// Home page for Ilay Gibor — Engineering Portfolio
// Keep all original information, elevate presentation.

const fade = {
  hidden: { opacity: 0, y: 12 },
  show: (i = 0) => ({ opacity: 1, y: 0, transition: { delay: 0.06 * i, duration: 0.5 } }),
};

const SectionHeader = ({ eyebrow, title, description }) => (
  <div className="mx-auto max-w-3xl text-center">
    <motion.p className="text-sm tracking-widest text-muted-foreground" variants={fade}>
      {eyebrow}
    </motion.p>
    <motion.h2 className="mt-2 text-3xl font-semibold tracking-tight sm:text-4xl" variants={fade}>
      {title}
    </motion.h2>
    {description && (
      <motion.p className="mt-3 text-muted-foreground" variants={fade}>
        {description}
      </motion.p>
    )}
  </div>
);

const ProjectCard = ({ index, icon: Icon, title, subtitle, href, cta = "View Code & Docs → GitHub Repository" }) => (
  <motion.div variants={fade} custom={index}>
    <Card className="group relative overflow-hidden border-border/60 bg-gradient-to-b from-background to-muted/30 shadow-sm transition hover:shadow-md">
      <CardHeader className="pb-3">
        <div className="flex items-center gap-3">
          <div className="rounded-2xl border bg-background p-2 shadow-sm">
            <Icon className="h-5 w-5" />
          </div>
          <CardTitle className="text-lg">{title}</CardTitle>
        </div>
        <CardDescription className="pt-2 leading-relaxed">{subtitle}</CardDescription>
      </CardHeader>
      <CardContent className="pt-0">
        <Button asChild variant="secondary" className="w-full justify-between">
          <a href={href}>
            {cta}
            <ArrowRight className="h-4 w-4" />
          </a>
        </Button>
      </CardContent>
      <div className="pointer-events-none absolute inset-0 opacity-0 transition group-hover:opacity-100">
        <div className="absolute -right-16 -top-16 h-40 w-40 rounded-full bg-primary/10 blur-2xl" />
      </div>
    </Card>
  </motion.div>
);

export default function Home() {
  return (
    <div className="min-h-screen bg-gradient-to-b from-background via-background to-muted/30">
      {/* Nav */}
      <header className="sticky top-0 z-50 w-full backdrop-blur supports-[backdrop-filter]:bg-background/60">
        <div className="mx-auto flex max-w-6xl items-center justify-between px-5 py-3">
          <a href="#top" className="font-semibold tracking-tight">Ilay Gibor</a>
          <nav className="hidden gap-6 text-sm sm:flex">
            <a href="#research" className="text-muted-foreground hover:text-foreground">Research</a>
            <a href="#engineering" className="text-muted-foreground hover:text-foreground">Engineering</a>
            <a href="#contact" className="text-muted-foreground hover:text-foreground">Contact</a>
            <a href="https://github.com/IlayGibor" className="inline-flex items-center gap-2 text-muted-foreground hover:text-foreground">
              <Github className="h-4 w-4" /> GitHub
            </a>
          </nav>
        </div>
        <div className="h-px w-full bg-gradient-to-r from-transparent via-border to-transparent" />
      </header>

      {/* Hero */}
      <section id="top" className="relative">
        <div className="absolute inset-0 -z-10 overflow-hidden">
          <div className="absolute left-1/2 top-10 h-72 w-72 -translate-x-1/2 rounded-full bg-primary/10 blur-3xl" />
          <div className="absolute left-[15%] top-64 h-56 w-56 rounded-full bg-primary/5 blur-2xl" />
          <div className="absolute right-[10%] top-40 h-64 w-64 rounded-full bg-primary/10 blur-2xl" />
        </div>
        <motion.div
          className="mx-auto grid max-w-6xl grid-cols-1 items-center gap-10 px-5 py-20 sm:grid-cols-2"
          initial="hidden"
          whileInView="show"
          viewport={{ once: true }}
        >
          <motion.div variants={fade}>
            <div className="inline-flex items-center gap-2 rounded-full border px-3 py-1 text-xs text-muted-foreground">
              <span>Engineering Portfolio</span>
              <span className="h-1 w-1 rounded-full bg-primary/60" />
              <span>Robotics • ML • Bioengineering</span>
            </div>
            <h1 className="mt-4 text-4xl font-semibold leading-tight sm:text-5xl">
              Ilay Gibor — Engineering Portfolio
            </h1>
            <p className="mt-4 text-base leading-relaxed text-muted-foreground">
              Welcome! I’m Ilay, a high-school engineer working at the intersection of <strong>robotics</strong>, <strong>machine learning</strong>, and <strong>bioengineering</strong>.
              This site collects my research and engineering projects with links to the complete code and documentation.
            </p>
            <div className="mt-6 flex flex-wrap items-center gap-3">
              <Badge variant="secondary" className="text-xs">Robotics</Badge>
              <Badge variant="secondary" className="text-xs">Machine Learning</Badge>
              <Badge variant="secondary" className="text-xs">Bioengineering</Badge>
              <Badge variant="outline" className="text-xs">Open‑source</Badge>
            </div>
            <div className="mt-6 flex flex-wrap gap-3">
              <Button asChild>
                <a href="#research">
                  Explore Projects <ArrowRight className="ml-2 h-4 w-4" />
                </a>
              </Button>
              <Button asChild variant="secondary">
                <a href="https://github.com/IlayGibor" className="inline-flex items-center gap-2">
                  <Github className="h-4 w-4" /> GitHub
                </a>
              </Button>
            </div>
          </motion.div>
          <motion.div className="relative" variants={fade}>
            <div className="aspect-[4/3] w-full rounded-3xl border bg-gradient-to-br from-muted to-background p-6 shadow-inner">
              <div className="grid h-full grid-cols-3 gap-3">
                <div className="rounded-2xl border bg-background/70 p-4 shadow-sm">
                  <div className="flex items-center gap-3">
                    <Microscope className="h-5 w-5" />
                    <span className="text-sm font-medium">Research</span>
                  </div>
                  <p className="mt-2 text-xs text-muted-foreground">
                    Collagen segmentation • Data robustness • Reproducible pipelines
                  </p>
                </div>
                <div className="rounded-2xl border bg-background/70 p-4 shadow-sm">
                  <div className="flex items-center gap-3">
                    <Cpu className="h-5 w-5" />
                    <span className="text-sm font-medium">Robotics</span>
                  </div>
                  <p className="mt-2 text-xs text-muted-foreground">
                    Vision pipelines • PID tuning • Autonomous & Tele‑op
                  </p>
                </div>
                <div className="rounded-2xl border bg-background/70 p-4 shadow-sm">
                  <div className="flex items-center gap-3">
                    <Bot className="h-5 w-5" />
                    <span className="text-sm font-medium">ML + Apps</span>
                  </div>
                  <p className="mt-2 text-xs text-muted-foreground">
                    Hackathon builds • Full‑stack prototypes • Fast iteration
                  </p>
                </div>
                <div className="col-span-3 rounded-2xl border bg-background/70 p-4 shadow-sm">
                  <div className="flex items-center gap-3">
                    <GitBranch className="h-5 w-5" />
                    <span className="text-sm font-medium">Reproducibility</span>
                  </div>
                  <p className="mt-2 text-xs text-muted-foreground">
                    All repositories include detailed READMEs and requirements.txt files for reproducibility.
                  </p>
                </div>
              </div>
            </div>
          </motion.div>
        </motion.div>
      </section>

      {/* Research Projects */}
      <section id="research" className="px-5 py-16">
        <SectionHeader
          eyebrow="Research Projects"
          title="Applied ML & Bioengineering"
          description={
            "Automated segmentation of collagen sub‑types in histopathology slides for permeability simulation; " +
            "and comparative studies of model robustness under controlled data corruptions."
          }
        />
        <motion.div
          className="mx-auto mt-10 grid max-w-6xl grid-cols-1 gap-6 sm:grid-cols-2"
          initial="hidden"
          whileInView="show"
          viewport={{ once: true }}
        >
          <ProjectCard
            index={0}
            icon={Microscope}
            title="Research Paper 1 — Collagen Segmentation"
            subtitle="Automated segmentation of collagen sub‑types in histopathology slides for permeability simulation."
            href="./projects/research1/"
          />
          <ProjectCard
            index={1}
            icon={Cpu}
            title="Research Paper 2 — ML Data Optimization / Robustness"
            subtitle="Compared machine‑learning models under different data corruptions to evaluate robustness and validation stability."
            href="./projects/research2/"
          />
        </motion.div>
      </section>

      {/* Engineering Projects */}
      <section id="engineering" className="px-5 py-16">
        <SectionHeader
          eyebrow="Engineering & Applied Projects"
          title="Robotics, Systems, and Hackathons"
          description="Selected builds spanning autonomous control, computer vision, and full‑stack prototyping."
        />
        <motion.div
          className="mx-auto mt-10 grid max-w-6xl grid-cols-1 gap-6 md:grid-cols-2"
          initial="hidden"
          whileInView="show"
          viewport={{ once: true }}
        >
          <ProjectCard
            index={0}
            icon={Bot}
            title="FTC Robotics Codebase"
            subtitle="Full autonomous and tele‑op control system for our FTC robot, including vision pipelines and PID tuning."
            href="./projects/robotics/"
            cta="View Code → GitHub Repository"
          />
          <ProjectCard
            index={1}
            icon={Cpu}
            title="KoHack App — Hackathon Project (2nd Place)"
            subtitle="24‑hour hackathon app built to [describe problem later]; front‑end + back‑end completed under tight deadline."
            href="./projects/kohack/"
            cta="View Code → GitHub Repository"
          />
        </motion.div>

        <div className="mx-auto mt-10 max-w-6xl">
          <blockquote className="rounded-2xl border bg-muted/40 p-5 text-sm text-muted-foreground">
            <em>
              “All repositories include detailed READMEs and requirements.txt files for reproducibility.”
            </em>
          </blockquote>
        </div>
      </section>

      {/* Contact */}
      <section id="contact" className="px-5 py-16">
        <SectionHeader eyebrow="Contact" title="Let’s connect" />
        <motion.div
          className="mx-auto mt-8 flex max-w-2xl flex-col items-center gap-3 text-center"
          initial="hidden"
          whileInView="show"
          viewport={{ once: true }}
        >
          <p className="text-muted-foreground">
            <strong>Email:</strong> your.email@example.com
            <br />
            <strong>GitHub:</strong> <a className="underline-offset-4 hover:underline" href="https://github.com/IlayGibor">github.com/IlayGibor</a>
          </p>
          <div className="mt-3 flex gap-3">
            <Button asChild>
              <a href="mailto:your.email@example.com" className="inline-flex items-center gap-2">
                <Mail className="h-4 w-4" /> Email Me
              </a>
            </Button>
            <Button asChild variant="secondary">
              <a href="https://github.com/IlayGibor" className="inline-flex items-center gap-2">
                <Github className="h-4 w-4" /> GitHub Profile
              </a>
            </Button>
          </div>
        </motion.div>
      </section>

      <footer className="border-t bg-background/60 py-8">
        <div className="mx-auto max-w-6xl px-5 text-xs text-muted-foreground">
          <div>© {new Date().getFullYear()} Ilay Gibor. All rights reserved.</div>
          <div className="mt-1">Built with React, Tailwind, shadcn/ui, and Framer Motion.</div>
        </div>
      </footer>
    </div>
  );
}
