# 🚀 Ambitious Skills

> **"Model capabilities don't grow uniformly... We ought to be more ambitious when using AI."**
>
> — **Felix Rieseberg**, [*How to be more ambitious: A tutorial for humans with models*](https://felixrieseberg.com/how-to-be-more-ambitious-a-tutorial-for-humans-with-models/)

## 📖 Origin & Philosophy

This repository operationalizes the concepts introduced by **Felix Rieseberg** in his essay, [**"How to be more ambitious: A tutorial for humans with models"**](https://felixrieseberg.com/how-to-be-more-ambitious-a-tutorial-for-humans-with-models/).

### The Problem: The Capability–Ambition Gap

As frontier AI capabilities advance rapidly, human application remains largely trapped in the **Speed Trap**—using models merely to complete routine, incremental tasks slightly faster (drafting emails, formatting slide decks, producing superficial summaries). Decades of organizational socialization and narrow specialization produce a **self-efficacy deficit**, leading humans to anchor models to their own comfort zones rather than exploring high-leverage outcomes.

This repository provides structured, executable **skill definitions** targeting three distinct, non-speed vectors of ambition: **Altitude**, **Depth**, and **Range**.

## 🧭 The Three Ambitious Skills

```
                        ▲  ALTITUDE (The goal beyond the goal / Autonomous loops)
                        │
                        │
   RANGE ───────────────┼─────────────── DEPTH
   (Nouns to verbs /    │               (Specialist tools / Raw primary data /
    Adversarial crews)  │                Outside verification judges)
                        ▼

```

| Skill | Focus | Core Mechanism | 
| ----- | ----- | ----- | 
| [**`ambition-altitude`**](./ambition-altitude/SKILL.md) | **The Goal Beyond the Goal** | Ascends the abstraction ladder: replaces single periodic deliverables (e.g., quarterly slide decks) with strategic decision engines and autonomous, self-healing continuous monitoring loops. | 
| [**`ambition-depth`**](./ambition-depth/SKILL.md) | **Elite Domain Rigor** | Rejects superficial text and hand-waving tables. Mandates raw unaggregated primary data, real code/statistical modeling, unreasonable benchmarks, and objective external validation tests. | 
| [**`ambition-range`**](./ambition-range/SKILL.md) | **Cross-Domain Synthesis** | Deconstructs static nouns into active verbs, staffs multidisciplinary virtual specialist crews (e.g., journalists, forensic accountants, systems engineers), and runs adversarial red-team stress tests. | 

## 📂 Repository Structure

```
ambitious-skills/
├── README.md
├── LICENSE
├── ambition-altitude/
│   └── SKILL.md
├── ambition-depth/
│   └── SKILL.md
└── ambition-range/
    └── SKILL.md

```

Each `SKILL.md` file contains standard YAML frontmatter (`name`, `description`), foundational principles, clear trigger patterns, step-by-step execution workflows, and common failure modes (gotchas).

## 🛠️ Cross-Platform Deployment Guide

These skills can be imported and executed across Claude, ChatGPT, and Gemini:

### 1. Claude (Anthropic)

Claude natively excels at complex multi-step reasoning, systemic synthesis, and executing within structured harnesses.

#### Option A: Claude Projects *(Recommended for Pro / Team / Enterprise)*

1. Create a new Project named **"Ambitious Co-Pilot"**.

2. Under **Project Knowledge**, upload:

   * `ambition-altitude/SKILL.md`

   * `ambition-depth/SKILL.md`

   * `ambition-range/SKILL.md`

3. Under **Project Custom Instructions**, paste:

   ```
   You have access to three ambition skills in your project knowledge: ambition-altitude, ambition-depth, and ambition-range (inspired by Felix Rieseberg's ambition framework).
   
   When explicitly invoked by name (e.g., "apply ambition-depth", "/altitude") or when a request warrants systemic escalation, professional domain depth, or cross-disciplinary stress-testing, strictly follow the workflow, principles, and verification steps in the respective SKILL.md file. Never default to generic summaries or polite approximations.
   
   ```

4. Start a chat inside your Project.

#### Option B: Claude Code CLI / `CLAUDE.md`

For local terminal workflows with Claude Code, copy or link these skill files into your project's root `CLAUDE.md` or `.claude/skills/` directory so they are loaded automatically during code generation and system analysis.

### 2. ChatGPT (OpenAI)

ChatGPT pairs effectively with **Code Interpreter (Advanced Data Analysis)** to execute the data modeling and external verification required by `ambition-depth`.

#### Option A: Custom GPT (GPT Builder) *(Recommended)*

1. Open **Explore GPTs** → **Create**.

2. Name: **"Ambitious Problem Solver"**.

3. Under **Configure** → **Capabilities**, ensure **Code Interpreter** is checked (crucial for executing real Python code against raw datasets rather than generating approximations).

4. Under **Knowledge**, upload `ambition-altitude/SKILL.md`, `ambition-depth/SKILL.md`, and `ambition-range/SKILL.md`.

5. Under **Instructions**, add:

   ```
   Adopt the principles in the uploaded SKILL.md files (ambition-altitude, ambition-depth, ambition-range).
   When depth is requested, always execute real Python code, test raw datasets, and run objective validation rather than offering conversational approximations.
   
   ```

#### Option B: ChatGPT Projects (Plus / Team / Enterprise)

1. Create a Project named **"Ambitious Workflows"**.

2. Upload the `SKILL.md` files into **Files**.

3. In **Project Instructions**, prompt ChatGPT to reference the files whenever strategic planning, technical problem-solving, or cross-domain analysis is requested.

### 3. Gemini (Google)

Gemini’s massive 1M–2M token context window provides a distinct advantage for `ambition-depth` (ingesting entire unaggregated raw log dumps, databases, or large codebases) and `ambition-altitude` (ingesting complete historical company documentation).

#### Option A: Gemini Gems *(Recommended for Gemini Advanced)*

1. Open **Gem Manager** → **New Gem**.

2. Name the Gem **"Ambitious Thinking"**.

3. In the **Instructions** field, paste:

   ```
   You operate under three specialized ambition frameworks inspired by Felix Rieseberg:
   1. ambition-altitude: Elevate tasks to systemic outcomes and autonomous loops.
   2. ambition-depth: Demand specialist-grade tools, raw data analysis, and external verification.
   3. ambition-range: Break silos using verbs, multi-domain crews, and adversarial red teams.
   
   When requested, execute the structured workflows defined in these frameworks. Do not default to polite, surface-level summaries.
   
   ```

4. Attach the skill markdown files to the Gem's Knowledge base.

#### Option B: Google AI Studio

1. Open [Google AI Studio](https://aistudio.google.com/) and create a **Chat Prompt** using Gemini 1.5 Pro.

2. Paste the contents of the `SKILL.md` files into the **System Instructions** pane.

3. Ingest uncurated raw source files (server logs, full codebases, raw telemetry) into the prompt context and direct the model to run depth or altitude audits directly on the raw material.

## ⚡ Comparison: Mundane vs. Ambitious

| Mode | Mundane / Incremental Prompt | Ambitious Execution | 
| ----- | ----- | ----- | 
| **Altitude** | *"Update the 5-slide deck template with this quarter's metrics."* | *"Run **`ambition-altitude`** on our quarterly review. What are the top 3 capital allocation decisions leadership must make, and how do we design an automated monitoring harness that replaces this quarterly deck entirely?"* | 
| **Depth** | *"Why is customer churn increasing? Give me a summary table."* | *"Apply **`ambition-depth`** to these raw server event logs. Formulate a falsifiable hypothesis regarding latency during onboarding, build a predictive model in Python to test it, and evaluate performance on held-out data."* | 
| **Range** | *"Review this product release announcement and polish the copy."* | *"Run **`ambition-range`** on this release announcement. Deconstruct the deliverable into verbs, then assemble a virtual crew—an investigative tech reporter, a forensic accountant, and a competitor's red team—to stress-test every claim before release."* | 

## 💡 Practical Rules of Engagement

1. **Reject "Vocabulary Switching":** Adopting specialized terminology without running specialized methodology is not depth. Real depth requires running the actual mathematical, computational, or investigative techniques of an expert.

2. **Outside Judges Over Self-Grading:** Never let a model grade its own work. Mandate external linters, compiler checks, unit test suites, or live validation scripts.

3. **Nouns to Verbs:** Avoid asking for static artifacts (e.g., "a report", "a dashboard"). Instead, define the active human objective: *"Convincing skeptical executives to reallocate 30% of engineering bandwidth in under 15 minutes."*

## 📚 References & Attribution

* **Original Essay:** [*How to be more ambitious: A tutorial for humans with models*](https://felixrieseberg.com/how-to-be-more-ambitious-a-tutorial-for-humans-with-models/) (October 2026)

* **Author:** [Felix Rieseberg](https://felixrieseberg.com/) (Engineering Lead at Anthropic; co-maintainer of Electron)


## 📄 License

This repository is open-sourced under the [MIT License](LICENSE).
