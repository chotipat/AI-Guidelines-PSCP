# AI Guidelines for PSCP

This repository provides guidelines and templates for using AI responsibly in the Problem Solving and Computer Programming course at IT KMITL.

This repository does not contain OJ problems, official solutions, hidden test cases, or course-restricted materials.

The official editor for this course is VS Code.

Students must use VS Code for writing, running, and testing Python code before submitting final code to the course OJ.

---

## 1. Purpose of This Repository

This repository explains how students should use AI tools in this course.

AI may be used as:

- a problem-solving coach,
- a pseudocode or flowchart reviewer,
- a debugging assistant,
- a test-case generator,
- a reflection helper.

AI must not be used as a replacement for the student's own thinking.

The main goal is to help students develop problem-solving and programming skills, not only to obtain accepted answers from the OJ.

---

## 2. Files in This Repository

| File | Purpose |
|---|---|
| `README.md` | Main course policy and submission rules |
| `README.th.md` | Thai version of the main course policy and submission rules |
| `policies/LAB_COMPUTER_USAGE.md` | Shared lab computer usage policy |
| `policies/LAB_COMPUTER_USAGE.th.md` | Thai shared lab computer usage policy |
| `instructions/COURSE_AI_INSTRUCTIONS.md` | Main AI coach instructions for ChatGPT, Claude, Gemini web chat, and similar AI tools |
| `instructions/AGENTS.md` | Shared course AI rules for coding agents. Codex can use this file directly |
| `instructions/CLAUDE.md` | Ready-to-use Claude Code instruction wrapper. Copy this together with `instructions/AGENTS.md` into `pscp/` before using Claude Code |
| `workflows/STUDENT_WORKFLOW_WEB_CHAT.md` | Workflow for AI tools used through a browser or chat interface |
| `workflows/STUDENT_WORKFLOW_WEB_CHAT.th.md` | Thai workflow for AI tools used through a browser or chat interface |
| `workflows/STUDENT_WORKFLOW_CHATGPT_CODEX.md` | Tool-specific workflow for ChatGPT Codex, OpenAI Codex, Codex CLI, and optional Codex app use |
| `workflows/STUDENT_WORKFLOW_CHATGPT_CODEX.th.md` | Thai tool-specific workflow for ChatGPT Codex, OpenAI Codex, Codex CLI, and optional Codex app use |
| `workflows/STUDENT_WORKFLOW_CLAUDE_CODE.md` | Tool-specific workflow for Claude Code CLI and optional Claude desktop app / Claude Cowork use |
| `workflows/STUDENT_WORKFLOW_CLAUDE_CODE.th.md` | Thai tool-specific workflow for Claude Code CLI and optional Claude desktop app / Claude Cowork use |
| `templates/SUBMISSION_TEMPLATE.md` | Blank template for creating `submission.md`, required only for learning-log-required OJ problems |
| `templates/SUBMISSION_TEMPLATE.th.md` | Thai version of the `submission.md` template |
| `templates/AI_REFLECTION_TEMPLATE.md` | Blank template for `ai_reflection.md`, required only when AI was used on a learning-log-required OJ problem |
| `templates/AI_REFLECTION_TEMPLATE.th.md` | Thai version of the `ai_reflection.md` template |
| `examples/SUBMISSION_TEMPLATE_sample_no_AI.md` | Example of a completed `submission.md` when AI was not used |
| `examples/SUBMISSION_TEMPLATE_sample_AI.md` | Example of a completed `submission.md` when AI was used |
| `examples/AI_REFLECTION_TEMPLATE_sample.md` | Example of a completed `ai_reflection.md` |
| `examples/SUBMISSION_TEMPLATE_sample_no_AI.th.md` | Thai example of a completed `submission.md` when AI was not used |
| `examples/SUBMISSION_TEMPLATE_sample_AI.th.md` | Thai example of a completed `submission.md` when AI was used |
| `examples/AI_REFLECTION_TEMPLATE_sample.th.md` | Thai example of a completed `ai_reflection.md` |

Read this `README.md` or `README.th.md` first.

Read `policies/LAB_COMPUTER_USAGE.md` before using a shared lab computer.

When using a shared lab computer, students must use their own `pscp-<student-id>/` folder, log out of all accounts after use, and ensure that AI tools do not access another student's files.

Use `templates/SUBMISSION_TEMPLATE.md` to create your own `submission.md`.

Use `templates/AI_REFLECTION_TEMPLATE.md` to create your own `ai_reflection.md` when AI was used on a learning-log-required problem.

You may read sample files in `examples/` to understand the expected level of detail, but you must not copy sample content into your own submission.

Thai `.th.md` files are provided for the README, policies, workflow documents, templates, and sample examples.

The English instruction files remain the primary files for AI tools and coding agents.

---

## 3. Official Editor Policy

VS Code is the official editor for this course.

Students must use VS Code for:

- writing Python code,
- running Python code,
- testing their code locally,
- preparing final code before OJ submission.

AI tools may be used only as assistants under the course AI policy.

AI-first editors such as Cursor are not part of the official workflow unless explicitly allowed by the instructor.

If the instructor does not explicitly allow another editor, students should use VS Code only.

---

## 4. Which Workflow Should I Read?

Choose the workflow based on how the AI tool is used, not based on whether the account is free or paid.

| If you use... | Read this workflow |
|---|---|
| ChatGPT, Claude, Gemini, or another AI tool through a browser/chat interface | `workflows/STUDENT_WORKFLOW_WEB_CHAT.md` |
| ChatGPT Codex, OpenAI Codex, Codex CLI, or Codex app | `workflows/STUDENT_WORKFLOW_CHATGPT_CODEX.md` |
| Claude Code CLI, or Claude desktop app / Claude Cowork if explicitly allowed by the instructor | `workflows/STUDENT_WORKFLOW_CLAUDE_CODE.md` |

Important:

- Free or paid account status is not the main distinction.
- The main distinction is whether the AI is used only as a chat assistant or whether it can work inside the coding environment.
- If the AI can read files, edit code, run commands, or suggest code directly inside VS Code or a terminal, treat it as a coding tool.
- GitHub Copilot in VS Code and other VS Code AI extensions are not part of the official workflow unless explicitly allowed by the instructor.
- Cursor and other AI-first editors are not part of the official workflow unless explicitly allowed by the instructor, because VS Code is the required editor for this course.

Other AI coding tools, VS Code AI extensions, and AI-first editors are not part of the course workflow unless the instructor announces a separate workflow.

---

## 5. Tool-Specific Quick Notes

Detailed setup and usage rules are explained in the workflow files.

Read the correct workflow before using each tool.

### Codex

If you use ChatGPT Codex, OpenAI Codex, Codex CLI, or Codex app, read:

```text
workflows/STUDENT_WORKFLOW_CHATGPT_CODEX.md
```

For Codex CLI, the recommended course workflow is:

```text
VS Code + Codex CLI
```

Students should copy:

```text
instructions/AGENTS.md
```

into their local course folder as:

```text
pscp/AGENTS.md
```

### Claude Code

If you use Claude Code, read:

```text
workflows/STUDENT_WORKFLOW_CLAUDE_CODE.md
```

For Claude Code CLI, the recommended course workflow is:

```text
VS Code + Claude Code CLI
```

Claude Code reads project instructions from:

```text
CLAUDE.md
```

Students should copy:

```text
instructions/AGENTS.md
instructions/CLAUDE.md
```

into their local course folder as:

```text
pscp/AGENTS.md
pscp/CLAUDE.md
```

### Tools Not Included in the Course Workflow

Other AI coding tools, VS Code AI extensions, and AI-first editors are not part of the course workflow unless the instructor announces a separate workflow.

VS Code remains the official editor.

The course OJ remains the official place for code submission.

---

## 6. What Students Must Write by Themselves

The following parts must be written by the student. AI may review, ask questions, or give suggestions, but AI must not write these parts for submission.

Students must write by themselves:

1. their own problem understanding,
2. input, output, and constraint analysis,
3. initial pseudocode, flowchart idea, or first plan,
4. explanation of their own algorithm,
5. final submitted code to the OJ that they understand and can explain,
6. their own test cases and test results,
7. their own `submission.md`, when the OJ problem is learning-log required,
8. their own `ai_reflection.md`, when AI was used on a learning-log-required OJ problem.

Students are not allowed to submit:

- AI-generated code that they cannot explain,
- AI-generated problem analysis copied directly without revision,
- AI-generated reflection that does not describe their real process,
- AI-generated pseudocode copied without understanding,
- fake AI reflection,
- fake testing results,
- fake OJ results.

Students do not need to submit the full AI conversation.

However, when interacting with AI, students must write their own questions, explain the problem in their own words, provide their own first plan, and verify AI suggestions by themselves.

The student is responsible for the final answer, final code, OJ submission, and explanation.

---

## 7. What Is a Learning Log?

A learning log is a GitHub folder for one OJ problem that is specifically marked as learning-log required by the instructor or in the OJ.

It records the student's problem-solving process and, if AI was used for that learning-log-required problem, the student's AI reflection.

A learning log may contain:

| File | Meaning |
|---|---|
| `submission.md` | The student's problem-solving record |
| `ai_reflection.md` | The student's reflection on AI use, required only if AI was used |

Use one folder per learning-log-required OJ problem.

Folder names must follow this format:

```text
oj<problem-id>
```

Replace `<problem-id>` with the 4-digit OJ problem ID.

Do not use the order in which you solved the problems.

Examples:

```text
oj2198
oj0301
oj1994
```

Do not use other folder name formats.

---

## 8. Overall Workflow for Every OJ Problem

For every assigned OJ problem, follow this overall process.

### Step 1: Read the OJ Problem

Read the problem statement in the course OJ.

Do not ask AI immediately.

### Step 2: Think by Yourself First

Before using AI, students must think by themselves first.

Students should prepare their own initial problem-solving note, which may include:

```text
Problem understanding:
Input:
Output:
Constraints:
First plan:
```

This is not necessarily full code.

Writing code at this step is optional.

The purpose of this step is to show that the student tried to understand and plan the solution before using AI.

If the problem is learning-log required, this initial thinking must be written in `submission.md`.

### Step 3: Choose the Correct AI Workflow, If AI Is Used

If the student does not use AI, continue coding in VS Code.

If the student uses AI through a browser/chat interface, follow:

```text
workflows/STUDENT_WORKFLOW_WEB_CHAT.md
```

If the student uses Codex, follow:

```text
workflows/STUDENT_WORKFLOW_CHATGPT_CODEX.md
```

If the student uses Claude Code, follow:

```text
workflows/STUDENT_WORKFLOW_CLAUDE_CODE.md
```

Other AI coding tools are not part of the course workflow unless the instructor announces a separate workflow.

### Step 4: Code in VS Code

Write Python code in VS Code.

Use your own pseudocode, flowchart idea, or first plan as a guide.

### Step 5: Test Locally

Run the code in VS Code before submitting to the OJ.

Check:

- normal cases,
- different types of cases,
- exact output format,
- cases that may be easy to miss.

### Step 6: Submit to the OJ

Submit the final code to the course OJ.

The OJ result is the official result for correctness.

### Step 7: Submit a Learning Log Only If Required

Create and push a learning log to your own GitHub repository only when the OJ problem is marked as learning-log required.

If the problem is not learning-log required, no GitHub learning log is required, even if AI was used.

However, students are still responsible for understanding and explaining their final code and AI use when asked.

---

## 9. What Must Be Submitted?

There are two possible submission places:

1. the course OJ,
2. the student's own public GitHub learning log repository.

### 9.1 OJ Submission

For every assigned OJ problem, students must submit final code to the course OJ.

### 9.2 GitHub Learning Log Submission

Students must submit a GitHub learning log only for OJ problems that are marked as learning-log required.

| Situation | Submit to OJ? | GitHub learning log required? | `submission.md` required? | `ai_reflection.md` required? |
|---|---:|---:|---:|---:|
| Normal OJ problem, no AI used | Yes | No | No | No |
| Normal OJ problem, AI used | Yes | No | No | No |
| Learning-log-required OJ problem, no AI used | Yes | Yes | Yes | No |
| Learning-log-required OJ problem, AI used | Yes | Yes | Yes | Yes |

Important rules:

- A GitHub learning log is required only when the OJ problem is marked as learning-log required.
- For every learning-log-required problem, students must submit `submission.md`.
- If AI was used on a learning-log-required problem, students must also submit `ai_reflection.md`.
- For non-learning-log problems, students do not need to submit `submission.md` or `ai_reflection.md`, even if AI was used.
- However, students may be randomly asked to explain their problem understanding, algorithm, code, test cases, and AI use.

---

## 10. Responsibility for AI Use on Non-Learning-Log Problems

Students may use AI for OJ problems that are not marked as learning-log required.

For these problems, students do not need to submit a GitHub learning log.

However, using AI does not remove the student's responsibility.

Students must still be able to explain:

1. their problem understanding,
2. their algorithm,
3. their code,
4. their test cases,
5. how AI helped, if AI was used,
6. what they verified by themselves.

The instructor may randomly ask students to explain their solution or AI use.

If a student cannot explain their submitted code, the submission may be treated as not demonstrating the student's own understanding.

---

## 11. When to Use `submission.md`

Use:

```text
templates/SUBMISSION_TEMPLATE.md
```

to create a file named:

```text
submission.md
```

You may read the examples in `examples/` before writing your own `submission.md`.

Do not copy the sample content into your own work.

`submission.md` is required only when the OJ problem is marked as learning-log required.

### When to Start `submission.md`

Start `submission.md` before using AI.

If AI is not used, start `submission.md` while solving the learning-log-required problem.

Before using AI, students must fill in at least:

```text
Problem understanding:
Input:
Output:
Constraints:
First plan:
Independent time spent on this problem:
```

If the student does not fully understand the problem yet, they must still write what they currently understand.

The answer may be incomplete or incorrect, but the student must make a genuine attempt before using AI.

Do not write only "not clear yet." Write the best current understanding, even if it may be wrong.

### When to Finish `submission.md`

Finish `submission.md` after:

1. coding in VS Code,
2. testing locally,
3. submitting to the OJ, if submitted,
4. knowing the current OJ status.

### Code in `submission.md`

Do not copy the full code into `submission.md`.

Use the OJ submission ID instead.

The submitted code should be checked in the OJ.

---

## 12. When to Use `ai_reflection.md`

Use:

```text
templates/AI_REFLECTION_TEMPLATE.md
```

to create a file named:

```text
ai_reflection.md
```

`ai_reflection.md` is required only when AI was used on a learning-log-required problem.

If AI was used on a non-learning-log problem, `ai_reflection.md` is not required, but the student must still understand and explain the solution when asked.

Your `ai_reflection.md` should explain:

1. OJ problem number/title,
2. OJ submission ID,
3. OJ status,
4. which AI tool you used,
5. whether you used `instructions/COURSE_AI_INSTRUCTIONS.md`, `instructions/AGENTS.md`, `instructions/CLAUDE.md`, or another approved course instruction file,
6. whether you read and followed the relevant workflow,
7. what you asked AI to help with,
8. what AI helped you notice,
9. what you checked or changed by yourself,
10. what you learned.

The reflection must describe your real process.

Do not ask AI to invent the reflection for you.

AI may help with grammar, formatting, or clarity after you write your own reflection.

---

## 13. Recommended Student GitHub Repository Structure

Each student should create one public GitHub repository for learning-log-required records.

Recommended repository name:

```text
pscp-<student-id>
```

Replace `<student-id>` with your own student ID.

Do not include the angle brackets `< >` in the actual repository name.

Example:

```text
pscp-66123456
```

Recommended structure:

```text
pscp-<student-id>/
├── README.md
├── oj2198/
│   ├── submission.md
│   └── ai_reflection.md
├── oj0301/
│   └── submission.md
└── oj1994/
    ├── submission.md
    └── ai_reflection.md
```

Use one folder per learning-log-required OJ problem.

Folder names must follow this format only:

```text
oj<problem-id>
```

The `<problem-id>` must be the 4-digit OJ problem ID, not the order in which the student solved the problems.

Examples:

```text
oj2198
oj0301
oj1994
```

The repository should be public so that the instructor can review it easily.

However, students must not include:

- official OJ problem statements,
- official solutions,
- hidden test cases,
- private data,
- access tokens or API keys,
- screenshots containing personal information,
- course materials that are not allowed to be redistributed,
- full source code files such as `solution.py`.

The repository should contain only the student's own problem-solving records, own test cases, own OJ submission references, and own AI reflections.

---

## 14. What to Put in Each Learning Log Folder

Each learning log folder may contain:

| File | When required | Purpose |
|---|---|---|
| `submission.md` | Required for every learning-log-required problem | Problem-solving record and OJ submission reference |
| `ai_reflection.md` | Required only if AI was used on that learning-log-required problem | Reflection on how AI helped and what the student verified independently |

Do not include `solution.py` in the GitHub learning log.

Use the OJ submission ID in `submission.md` instead.

### Example 1: Learning Log Required, No AI Used

```text
oj0301/
└── submission.md
```

### Example 2: Learning Log Required, AI Used

```text
oj2198/
├── submission.md
└── ai_reflection.md
```

### Example 3: No Learning Log Required

No GitHub folder is required.

Only OJ submission is required.

---

## 15. Final Reminder

AI can help you think, debug, and test.

You are still responsible for understanding, writing, testing, and explaining your own solution.
