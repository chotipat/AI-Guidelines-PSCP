# Student Workflow for AI Coding Tools

This file explains how students should use AI coding tools responsibly in this course.

This file is a general fallback workflow for AI coding tools.

Use a tool-specific workflow when one is provided:

- `workflows/STUDENT_WORKFLOW_CHATGPT_CODEX.md`
- `workflows/STUDENT_WORKFLOW_CLAUDE_CODE.md`

GitHub Copilot in VS Code and other VS Code AI extensions are not part of the official workflow unless explicitly allowed by the instructor.

If they are allowed, follow this general workflow and any extra instruction provided by the instructor.

---

## 1. Official Editor Policy

VS Code is the official editor for this course.

Students must use VS Code for:

- writing Python code,
- running Python code,
- testing their code locally,
- preparing final code before OJ submission.

AI coding tools may be used only as assistants.

AI-first editors such as Cursor are not part of the official workflow unless explicitly allowed by the instructor.

If the instructor does not explicitly allow another editor, students should use VS Code only.

---

## 2. Main Rule

AI coding tools may be used as learning assistants, but they must not replace the student's own thinking.

Students must not let an AI coding tool solve the whole OJ problem from zero without their own attempt.

Before using any AI coding tool, students must first try to understand the problem and write their own first plan.

The student is responsible for:

- final code,
- OJ submission,
- testing,
- explanation,
- AI reflection, if required.

If the student cannot explain the final code, they should not submit it.

---

## 3. What Counts as an AI Coding Tool?

An AI coding tool is any AI tool that can work directly in or near the coding environment.

This includes tools that can:

- suggest code while typing,
- generate code inside VS Code,
- edit files,
- read project files,
- inspect folders,
- run terminal commands,
- debug from errors,
- create new files,
- act as a coding agent,
- interact with Git or GitHub,
- work through VS Code, an IDE, a terminal, or CLI.

Examples:

| Tool Type | Examples |
|---|---|
| OpenAI coding agents | ChatGPT Codex, OpenAI Codex, Codex CLI |
| Claude coding agents | Claude Code, Claude Cowork |
| CLI or terminal AI tools | Codex CLI or other instructor-approved terminal-based agents |
| Other AI coding agents | Any tool that can read files, edit code, or run commands |

If a tool can read, write, or suggest code directly in the coding environment, use this workflow.

---

## 4. Files You Should Know

Before using AI coding tools, read these files:

| File | Purpose |
|---|---|
| `README.md` | Main course policy and submission rules |
| `instructions/COURSE_AI_INSTRUCTIONS.md` | Main AI coach instructions |
| `workflows/STUDENT_WORKFLOW_CODING_TOOLS.md` | This general workflow for AI coding tools |
| `templates/SUBMISSION_TEMPLATE.md` | Blank template for `submission.md` |
| `templates/AI_REFLECTION_TEMPLATE.md` | Blank template for `ai_reflection.md` |
| `examples/SUBMISSION_TEMPLATE_sample_no_AI.md` | Example submission when AI was not used |
| `examples/SUBMISSION_TEMPLATE_sample_AI.md` | Example submission when AI was used |
| `examples/AI_REFLECTION_TEMPLATE_sample.md` | Example AI reflection |

If your instructor provides a tool-specific workflow, read it too:

| Tool | Workflow |
|---|---|
| ChatGPT Codex / OpenAI Codex / Codex CLI | `workflows/STUDENT_WORKFLOW_CHATGPT_CODEX.md` |
| Claude Code / Claude Cowork | `workflows/STUDENT_WORKFLOW_CLAUDE_CODE.md` |

---

## 5. Check Whether the OJ Problem Is Learning-Log Required

For every assigned OJ problem, first check whether the problem is marked as learning-log required by the instructor or in the OJ.

| Case | What to Submit |
|---|---|
| Normal OJ problem | Submit code to the OJ only |
| Learning-log-required OJ problem | Submit code to the OJ and create a GitHub learning log |

If the problem is not learning-log required, you do not need to submit `submission.md` or `ai_reflection.md`, even if you used an AI coding tool.

However, you must still understand your code and be able to explain your AI use if asked.

If the problem is learning-log required and you use an AI coding tool, you must submit:

```text
submission.md
ai_reflection.md
```

---

## 6. Required Steps Before Using Any AI Coding Tool

Use this section before using any AI coding tool on an OJ problem.

### Step 1: Read the OJ Problem Yourself

Read the problem statement carefully in the course OJ.

Do not ask the AI tool to solve it immediately.

### Step 2: Write Your Own Understanding

Before using the AI tool, write your own notes.

Use this format:

```text
Problem understanding:
Input:
Output:
Constraints:
First plan:
```

If the problem is learning-log required, write this in `submission.md`.

If the problem is not learning-log required, this may be your private note.

Your understanding may be incomplete or incorrect, but you must make a genuine attempt.

### Step 3: Decide What Help You Need

Good purposes:

```text
Review my first plan
Explain a Python concept
Suggest test cases
Help find a bug
Explain an error message
Check whether my input reading is correct
```

Bad purposes:

```text
Solve the whole problem for me
Generate the complete accepted code
Rewrite everything without explanation
Submit code I do not understand
```

---

## 7. Using Course AI Instructions With Coding Tools

When the tool supports custom instructions, project instructions, rules files, agent instructions, or system prompts, use:

```text
instructions/COURSE_AI_INSTRUCTIONS.md
```

For Codex, use the provided file:

```text
instructions/AGENTS.md
```

If the tool does not support custom instructions, manually follow the rules in `instructions/COURSE_AI_INSTRUCTIONS.md`.

The most important rule is:

```text
The AI should act as a coach, not as a final-answer generator.
```

---

## 8. Safe Workflow While Using AI Coding Tools

### Step 1: Start From Your Own Code or First Plan

Do not begin by asking the AI to create the full solution.

Start with your own:

- understanding,
- first plan,
- pseudocode,
- flowchart idea,
- partial code,
- test case,
- error message.

### Step 2: Ask for Explanation Before Code

Good prompt:

```text
Please explain the likely bug first. Do not rewrite the whole code yet.
```

### Step 3: Review Every AI Suggestion

Do not accept AI-generated code blindly.

Check:

- Does it match the OJ problem?
- Does it use the correct input format?
- Does it produce the exact output format?
- Can I explain each important line?
- Did it change more code than necessary?
- Did it introduce advanced code I do not understand?

### Step 4: Run the Code Yourself

Run the code in VS Code or terminal.

Test at least 3 different test cases.

### Step 5: Submit to OJ Yourself

The student must submit the code to the OJ.

Do not use AI to submit the work.

---

## 9. Agentic Tools That Can Edit Files or Run Commands

Some tools can edit files or run commands.

Use extra caution.

Students should not allow the agent to:

- solve the whole OJ problem from scratch,
- make large changes without explanation,
- run unknown commands,
- install packages unnecessarily,
- delete files,
- modify unrelated files,
- change Git history,
- submit to the OJ,
- access private data,
- upload files or code to external services without understanding.

Before allowing the tool to edit or run commands, ask:

```text
Explain what you plan to change before changing files.
```

```text
Do not rewrite the whole file.
```

```text
Do not run commands without explaining them first.
```

After the tool makes changes, review the diff or changed code.

---

## 10. Workflow for a Normal OJ Problem

Use this workflow when the problem is not learning-log required.

1. Read the OJ problem yourself.
2. Think and write a private first plan before using AI.
3. Code and test in VS Code.
4. If you use an AI coding tool, follow Sections 6-9.
5. Submit final code to the OJ.

No GitHub learning log is required unless the instructor asks for it.

However, you must still understand your code and explain AI use if asked.

---

## 11. Workflow for a Learning-Log-Required Problem With an AI Coding Tool

Use this workflow when the problem is learning-log required and you use an AI coding tool.

1. Create a learning log folder, for example `oj002/`.
2. Copy `templates/SUBMISSION_TEMPLATE.md` and rename it as `submission.md`.
3. Before using AI, fill in your problem understanding and first plan.
4. Use the AI coding tool carefully.
5. Review all AI-generated code or edits.
6. Test at least 3 cases in VS Code or terminal.
7. Submit final code to the OJ yourself.
8. Complete `submission.md`.
9. Copy `templates/AI_REFLECTION_TEMPLATE.md` and rename it as `ai_reflection.md`.
10. Push the learning log folder to GitHub.

Do not paste full source code into GitHub.

Use the OJ submission ID instead.

---

## 12. What Not to Put in GitHub

Do not put these in your public GitHub repository:

- official OJ problem statements,
- official solutions,
- hidden test cases,
- full AI chat logs,
- API keys or access tokens,
- private information,
- screenshots containing personal information,
- course materials that are not allowed to be redistributed,
- full source code files such as `solution.py`.

Your GitHub learning log should contain only:

- `submission.md`,
- `ai_reflection.md`, if AI was used,
- your own test cases,
- OJ submission references,
- your own explanations.

---

## 13. Quick Self-Check

This checklist is only for self-checking.

Students do not need to submit this checklist.

Before submitting to the OJ, make sure that:

```text
[ ] I wrote, ran, and tested my code in VS Code.
[ ] I understand my final code.
[ ] I reviewed any AI-generated code or suggestions before using them.
[ ] I tested at least 3 different cases.
[ ] I can explain what AI helped with, if AI was used.
```

If the problem is learning-log required, complete the required files:

```text
submission.md
ai_reflection.md, if AI was used
```

---

## 14. Final Reminder

AI coding tools can be powerful.

They can help you think, debug, test, and learn.

They can also make it easy to submit code you do not understand.

Use them carefully.

Your final OJ submission is your responsibility.
