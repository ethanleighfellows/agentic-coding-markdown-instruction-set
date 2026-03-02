# Agentic Coding Markdown Instruction Set

These are the core markdown files designed to be cloned into a new repository when "vibe-coding" or working with AI coding agents. The goal of these files is to establish clear guidelines, enforce coding quality standards, and define workflows to ensure continual improvement and maintain a robust development process.

## Included Files

### 1. `Guidelines.md`
This is the authoritative reference for all coding agents working in the repository. It sets the overarching standards and quality guidelines, including:
- **Agent Role & Mindset:** Emphasizes correctness, small diffs, and acting as a senior engineer.
- **Project Structure & Dos/Don'ts:** Defines where code lives and the best practices to follow (e.g., using TypeScript, functional components, design tokens).
- **Commands & Safety:** Specifies acceptable commands and outlines actions that require explicit user approval (like irreversible infrastructure changes).
- **Testing & Code Style:** Mandates test-driven development, high test coverage, and strict code style conventions (TypeScript, pure functions, meaningful comments).
- **Architecture & Workflow:** Details the principles of separation of concerns and the step-by-step process for implementing features, fixing bugs, and refactoring.
- **Git Conventions & Security:** Outlines branching strategies, conventional commits, and critical security rules.

### 2. `Napkin.md`
The Napkin serves as a continuously curated, per-repo markdown runbook. It is not a chronological log but a live knowledge base designed for fast reuse in future sessions:
- **Session Start Protocol:** Agents must read and internalize this file silently at the start of every session.
- **Curation Rules:** Requires continuous curation—re-prioritizing items, merging duplicates, and enforcing category limits.
- **Content Focus:** Captures recurring, high-frequency guidance, hard-won project gotchas, and specific user directives. Every entry must include an actionable "Do instead" instruction to prevent repeating mistakes.

### 3. `Progress.md`
This file acts as the Agent Progress Log, maintaining the state between sessions to give agents full context immediately upon starting:
- **Project Status:** Tracks overall completion, the last working state, and current blockers.
- **Task Management:** Organizes work into To-do, In Progress, Completed, and a prioritized Backlog.
- **Issue & Decision Tracking:** Logs known defects and key architectural or implementation decisions.
- **Session Resumption:** Provides explicit instructions for agents on how to start a new session (e.g., read guidelines, read napkin, triage).

### 4. `Theorist.md` & `THEORY.md`
The Theorist skill ensures the creation and maintenance of `THEORY.md`, a living essay that captures the operating theory of the work being done. It differs from a log or task list by focusing on the narrative, strategy, and mental models guiding the project:
- **Purpose:** Acts as a cohesive narrative document explaining the problem thesis, operating theory, systematic strategy, and key discoveries.
- **Session Behavior:** Instructs agents to read `THEORY.md` at the start of a session and only create it once enough context exists to form a meaningful narrative.
- **Continuous Updates:** Requires frequent rewrites (not appends) after major work loops, ensuring the theory adapts to shifting understanding or discoveries.

### 5. `Start.md`
This file acts as the Agent Initialization & Workflow Protocol. It establishes the rigid, chronological sequence AI agents must follow when starting a work session to guarantee all instructions are properly loaded:
- **Phase 1: Context Loading:** Mandates that the agent silently reads `Guidelines.md`, `Napkin.md`, and `Theorist.md` before taking any action.
- **Phase 2: State Alignment:** Directs the agent to review `Progress.md` to identify the most critical next steps and overarching project status.
- **Phase 3: Execution Commences:** Authorizes the agent to begin the first listed task, emphasizing the continuous need to update the theory and runbook documents as work progresses.
