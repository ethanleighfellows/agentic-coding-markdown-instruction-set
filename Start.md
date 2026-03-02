# Start.md — Agent Initialization & Workflow Protocol

> **CRITICAL:** This file defines the exact chronological sequence an AI coding agent must follow when starting a new session in this repository. 
> Do not skip any steps. Do not start executing tasks until the context-loading phase is complete.

---

## Phase 1: Context Loading (Silent Phase)
*Before executing any commands, making any plans, or writing any code, the agent must silently read and internalize the following core instruction files in this exact order.*

### 1. Read `Guidelines.md`
- **Purpose:** Understand the strict engineering standards, code style, architecture principles, and security rules for this repository.
- **Action:** Read the file. Adopt the "senior engineer" mindset. Acknowledge allowed vs. restricted actions (e.g., when to ask for permission vs. auto-executing).

### 2. Read `Napkin.md` 
- **Purpose:** Load the highest-priority, curated gotchas, recurring issues, and user directives specific to this repository.
- **Action:** Read the file. Immediately apply the "Do instead" rules contained within. Ensure you do not repeat past mistakes. Do not announce that you read it.

### 3. Read `Theorist.md` & Initialize `THEORY.md`
- **Purpose:** Understand the overarching strategic narrative and the "why" behind the current codebase state.
- **Action:** 
  1. Read `Theorist.md` to understand how the theory document works.
  2. Check if a file named `THEORY.md` exists in the repository root.
  3. **If `THEORY.md` exists:** Read it to understand the current operating theory, problem thesis, and recent pivots.
  4. **If `THEORY.md` does not exist:** Do *not* create an empty skeleton immediately. Wait until you have enough context from the upcoming tasks to write a meaningful narrative, then create it.

---

## Phase 2: State Alignment
*After loading the static rules and theories, understand the current state of the project timeline.*

### 4. Read `Progress.md`
- **Purpose:** Determine the immediate next steps, known bugs, and overall project status.
- **Action:** Read the file. Review the "Overall completion" status, "Current blocker," and the "Key Decisions Log." Identify the highest-priority item in the "To-do Tasks" or "Backlog" sections.

---

## Phase 3: Execution Commences
*With full context loaded, you are now ready to begin active work.*

### 5. Commence Tasks
- **Action:** Begin executing the very first task listed in the "To-do Tasks" section of `Progress.md`.
- **Ongoing Rules during Execution:**
  - **Updates:** Update `Napkin.md` immediately if you encounter a new, reusable gotcha.
  - **Theory Shifts:** Update `THEORY.md` holistically (never append) if your understanding of the root problem or systematic strategy changes.
  - **Testing:** Write tests first, and run CI/linting checks before marking a task complete.
  - **Progress Tracking:** Upon completing the task, update `Progress.md` to move the task to "Completed", update the completion status, and log any key decisions made.

---

*End of Initialization sequence. The agent may now begin.*
