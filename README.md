# Agentic AI for QA

A lightweight, reusable [AGENTS.md](https://agents.md/) template for AI-assisted quality assurance. It tells compatible coding agents how to approach **Java/Selenium** and **TypeScript/Playwright** testing, debugging, code reviews, and verification.

**What this repository is:** a set of instructions to copy into your own QA project. **What it is not:** a runnable test framework or a replacement for your project's own build and test configuration.

## Quick Start

### 1. Get the instructions

Open [AGENTS.md](./AGENTS.md), copy its contents, and save them as `AGENTS.md` in the **root of your own QA automation repository**.

Alternatively, clone this template to inspect it locally:

```bash
git clone https://github.com/myoussef87/Agentic-AI-For-QA.git
cd Agentic-AI-For-QA
```

Cloning this repository does **not** automatically add its instructions to your other projects; copy the file to the project you want Codex to work on.

### 2. Open your QA project in Codex

Start **Codex CLI** or **Codex Desktop** with your QA project's folder as the working directory. Codex can discover applicable `AGENTS.md` instructions from the project.

### 3. Verify the instructions are being used

Ask:

> Read the AGENTS.md instructions for this project. Summarize your QA role, coding standards, what requires approval, and how you will verify a change. Do not modify any files.

Check that the response mentions POM, reliable tests, verification, and approval before pushing.

### 4. Try a real task

**Review only:**

> Inspect the existing QA framework. Identify the three highest-impact reliability or maintainability issues, with file locations and suggested fixes. Do not modify files.

**Implement and verify:**

> Add a functional test for [describe the feature] following AGENTS.md and existing project conventions. Run the relevant tests and report what passed, failed, or could not run. Do not push changes.

Replace the bracketed feature with a real feature in your project. Agents can run tests only if your project has the necessary code, dependencies, tools, and environment access.

## What's Covered

| Area | Agent expectations |
| --- | --- |
| Tech stack | Java/Selenium and TypeScript/Playwright |
| Architecture | Clean Code, SOLID, Page Object Model, readable fluent interfaces |
| Test quality | Isolated tests, stable selectors, functional/regression/E2E/API coverage where relevant |
| Debugging | Evidence-based root-cause analysis, limited retries, no hidden failures |
| Safety | Ask before pushing, deploying, accessing production, or destructive operations |
| Delivery | Relevant checks and a short, transparent result report |
| Learning | Keep only verified, reusable lessons in AGENTS.md |

## Adapting the Template

Keep `AGENTS.md` short. Add **actual project-specific commands** (for example, how to run focused tests) once you know your repository's tools. Remove irrelevant technology references if your project only uses Selenium or only Playwright. Do not invent test results or assume that installing this file creates test infrastructure.

The agent instructions are **guidance, not permission enforcement**. Use GitHub branch protections, repository access settings, and Codex approval controls for technical safeguards.

## Contributing

Improvements to clarity, safety, and practical QA workflows are welcome. Keep changes small, avoid duplicated rules, and explain why each new instruction is reusable.

## References

- [AGENTS.md format and examples](https://agents.md/)
- [OpenAI Codex documentation](https://developers.openai.com/codex/)
