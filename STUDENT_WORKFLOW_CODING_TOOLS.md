# Student Workflow for AI Coding Tools

This file explains how students should use AI coding tools responsibly in this course.

The official editor for this course is VS Code.

Students must write, run, and test Python code in VS Code before submitting to the course OJ.

AI tools may be used only as assistants under the course AI policy.

This workflow applies to AI tools that can help directly with code, files, commands, or the coding environment.

Examples include:

- ChatGPT Codex / OpenAI Codex / Codex CLI
- Claude Code
- Claude Cowork, if available to the student's account
- Gemini CLI
- GitHub Copilot in VS Code
- VS Code AI extensions
- other AI coding agents
- other terminal-based AI tools

This workflow applies whether the tool is free or paid.

The important question is not whether the account is free or paid.

The important question is whether the AI can help directly with code, files, commands, or the coding environment.

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

Reason:

- the class can follow the same setup,
- the instructor can support students more easily,
- beginner students avoid confusion from multiple environments,
- AI tools are kept as assistants rather than replacing the programming workflow.

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
| CLI or terminal AI tools | Gemini CLI, other terminal-based agents |
| Code completion and chat tools in VS Code | GitHub Copilot in VS Code |
| VS Code AI extensions | Continue, Codeium, Tabnine, Windsurf, or other similar extensions |
| Other AI coding agents | Any tool that can read files, edit code, or run commands |

If a tool can read, write, or suggest code directly in the coding environment, use this workflow.

---

## 4. Difference from Web Chat AI

Web Chat AI tools, such as ChatGPT, Claude, or Gemini in a browser, require students to copy and paste information manually.

AI coding tools are more powerful because they may work directly with code and files.

Therefore, AI coding tools require stricter discipline.

Students must:

- write their own first plan before using the tool,
- control what the tool is allowed to do,
- review every AI-generated change,
- run tests themselves,
- understand the final code,
- record AI use honestly when required.

---

## 5. Files You Should Know

Before using AI coding tools, read these files:

| File | Purpose |
|---|---|
| `README.md` | Main course policy and submission rules |
| `COURSE_AI_INSTRUCTIONS.md` | Main AI coach instructions |
| `STUDENT_WORKFLOW_CODING_TOOLS.md` | This general workflow for AI coding tools |
| `SUBMISSION_TEMPLATE.md` | Blank template for `submission.md` |
| `SUBMISSION_TEMPLATE_sample_no_AI.md` | Example submission when AI was not used |
| `SUBMISSION_TEMPLATE_sample_AI.md` | Example submission when AI was used |
| `AI_REFLECTION_TEMPLATE.md` | Blank template for `ai_reflection.md` |
| `AI_REFLECTION_TEMPLATE_sample.md` | Example AI reflection |

If your instructor provides a tool-specific workflow, read it too:

| Tool | Workflow |
|---|---|
| ChatGPT Codex / OpenAI Codex / Codex CLI | `STUDENT_WORKFLOW_CHATGPT_CODEX.md` |
| Claude Code / Claude Cowork | `STUDENT_WORKFLOW_CLAUDE_CODE.md` |
| Gemini CLI | `STUDENT_WORKFLOW_GEMINI_CLI.md` |
| GitHub Copilot in VS Code | `STUDENT_WORKFLOW_GITHUB_COPILOT_VSCODE.md` |
| Other VS Code AI extensions | `STUDENT_WORKFLOW_VSCODE_AI_EXTENSIONS.md` |

Cursor and other AI-first editors are not part of the official workflow unless explicitly allowed by the instructor.

---

## 6. Check Whether the OJ Problem Is Learning-Log Required

For every assigned OJ problem, first check whether the problem is marked as learning-log required by the instructor or in the OJ.

There are two cases:

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

## 7. Required Steps Before Using Any AI Coding Tool

Use this section before using any AI coding tool on an OJ problem.

This applies to both:

- normal OJ problems,
- learning-log-required OJ problems.

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

If you do not fully understand the problem, still write what you currently understand.

Your understanding may be incomplete or incorrect, but you must make a genuine attempt.

### Step 3: Decide What Help You Need

Before opening or prompting the AI tool, decide what kind of help you need.

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

### Step 4: Keep the AI Scope Small

Ask the AI tool for limited help.

Good examples:

```text
Review my first plan. Do not write the full solution.
```

```text
Look at this function and explain why it fails this test case.
```

```text
Suggest three useful test cases and explain why they are useful.
```

```text
Explain this error message and point me to the likely line causing it.
```

Avoid broad commands such as:

```text
Solve this OJ problem.
```

```text
Make the code pass.
```

```text
Rewrite my whole solution.
```

```text
Implement everything.
```

---

## 8. Using `COURSE_AI_INSTRUCTIONS.md` With Coding Tools

When the tool supports custom instructions, project instructions, rules files, agent instructions, or system prompts, use `COURSE_AI_INSTRUCTIONS.md`.

Examples:

- project instructions,
- custom instruction files,
- agent instruction files,
- rule files,
- prompt files,
- chat context,
- tool-specific memory or rules.

If the tool does not support custom instructions, manually follow the rules in `COURSE_AI_INSTRUCTIONS.md`.

The most important rule is:

```text
The AI should act as a coach, not as a final-answer generator.
```

The AI should help the student think, debug, and test.

The AI should not complete the whole OJ problem without the student's own attempt.

---

## 9. Safe Workflow While Using AI Coding Tools

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

Ask the AI to explain the issue before suggesting code changes.

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

### Step 4: Apply Changes Yourself When Possible

When possible, type or edit the code yourself after understanding the AI suggestion.

If the tool edits files automatically, review the change before keeping it.

### Step 5: Run the Code Yourself

Run the code in VS Code or terminal.

Test at least 3 different test cases.

Use cases that are different from each other.

For each test case, know:

- why you chose it,
- expected output,
- actual output,
- whether it passed.

### Step 6: Submit to OJ Yourself

The student must submit the code to the OJ.

Do not use AI to submit the work.

### Step 7: Record AI Use If Required

If the problem is learning-log required and AI was used, complete:

```text
submission.md
ai_reflection.md
```

---

## 10. Reviewing AI-Generated Code

If the AI tool generated or edited code, the student must review it.

Before submitting, the student should be able to answer:

```text
What does this code do?
Why does this algorithm work?
How does the input reading work?
What does each important variable mean?
What happens in a small case?
What happens in a special or unusual case?
What tests did I run?
What did AI help with?
What did I verify by myself?
```

If the student cannot answer these questions, they should not submit the code yet.

---

## 11. Autocomplete and Inline Suggestions

Some tools suggest code while the student is typing.

Examples:

- GitHub Copilot inline suggestions,
- VS Code AI extension suggestions,
- other code completion tools.

Students may use these suggestions only if they understand them.

Rules:

- Do not accept a long suggestion without reading it.
- Do not accept code that uses concepts you cannot explain.
- Do not accept code that changes the algorithm without understanding why.
- If a suggestion completes a major part of the solution, treat it as AI use.
- If the problem is learning-log required and AI suggestions were used meaningfully, complete `ai_reflection.md`.

Small autocomplete suggestions for syntax or variable names may still count as AI assistance, but the key issue is whether AI meaningfully helped solve the problem.

When unsure, disclose the AI use.

---

## 12. Agentic Tools That Can Edit Files or Run Commands

Some tools can edit files or run commands.

Examples:

- ChatGPT Codex / OpenAI Codex / Codex CLI,
- Claude Code,
- Claude Cowork,
- Gemini CLI,
- some AI coding agents,
- terminal-based AI tools.

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
Show a small change first.
```

```text
Do not rewrite the whole file.
```

```text
Do not run commands without explaining them first.
```

After the tool makes changes, review the diff or changed code.

---

## 13. Tool-Specific Guidance

This file gives the general rules.

For detailed steps, follow the tool-specific workflow if provided.

### ChatGPT Codex / OpenAI Codex / Codex CLI

Use:

```text
STUDENT_WORKFLOW_CHATGPT_CODEX.md
```

Use this when OpenAI's coding tool can inspect files, edit files, run commands, or act as a coding agent.

### Claude Code / Claude Cowork

Use:

```text
STUDENT_WORKFLOW_CLAUDE_CODE.md
```

Use this when Claude can inspect files, edit files, run commands, or act as a coding agent.

### Gemini CLI

Use:

```text
STUDENT_WORKFLOW_GEMINI_CLI.md
```

Use this when Gemini is used through a terminal or CLI.

### GitHub Copilot in VS Code

Use:

```text
STUDENT_WORKFLOW_GITHUB_COPILOT_VSCODE.md
```

Use this when AI gives inline completions, chat suggestions, or edits in VS Code.

### VS Code AI Extensions

Use:

```text
STUDENT_WORKFLOW_VSCODE_AI_EXTENSIONS.md
```

Use this for other AI extensions in VS Code.

### Other AI Coding Agents

If no tool-specific file exists, use this general workflow and choose the closest matching category:

| Tool Behavior | Follow Similar Workflow |
|---|---|
| Works in terminal or CLI | Gemini CLI workflow |
| Works inside VS Code as an extension | VS Code AI extensions workflow |
| Gives inline completions in VS Code | GitHub Copilot VS Code workflow |
| Can edit files and run commands as an agent | ChatGPT Codex, Claude Code, or Gemini CLI workflow |

### Cursor and Other AI-First Editors

Cursor and other AI-first editors are not part of the official course workflow unless explicitly allowed by the instructor.

Students should use VS Code as the official editor.

---

## 14. Workflow for a Normal OJ Problem

Use this workflow when the problem is not learning-log required.

### Step 1: Read the OJ Problem

Read the problem yourself.

### Step 2: Think and Write a First Plan

Write a private first plan before using AI.

### Step 3: Code and Test in VS Code

Write code in VS Code and test locally.

### Step 4: If You Use an AI Coding Tool, Follow Sections 7-12

Before using the tool, follow the required steps in this file.

### Step 5: Submit to OJ

Submit final code to the OJ.

No GitHub learning log is required unless the instructor asks for it.

However, you must still understand your code and explain AI use if asked.

---

## 15. Workflow for a Learning-Log-Required Problem Without AI

Use this workflow when the problem is learning-log required and you do not use AI.

### Step 1: Create a Learning Log Folder

Example:

```text
oj001
```

### Step 2: Create `submission.md`

Copy `SUBMISSION_TEMPLATE.md` and rename it:

```text
submission.md
```

### Step 3: Fill in Your Own Thinking

Write:

- OJ information,
- problem understanding,
- first plan,
- final approach,
- at least 3 test cases.

### Step 4: Code, Test, Submit

Code in VS Code, test locally, and submit to the OJ.

### Step 5: Push to GitHub

The folder should contain:

```text
oj001/
└── submission.md
```

---

## 16. Workflow for a Learning-Log-Required Problem With an AI Coding Tool

Use this workflow when the problem is learning-log required and you use an AI coding tool.

### Step 1: Create a Learning Log Folder

Example:

```text
oj002
```

### Step 2: Create `submission.md` Before Using AI

Copy `SUBMISSION_TEMPLATE.md` and rename it:

```text
submission.md
```

Before using AI, fill in at least:

- OJ problem number/title,
- independent time spent on this problem,
- your current problem understanding,
- your first plan.

### Step 3: Use the AI Coding Tool Carefully

Follow Sections 7-12.

Use the tool as a coach, reviewer, debugger, or test-case helper.

Do not let it solve the whole problem without your own understanding.

### Step 4: Code, Review, and Test

Review all AI-generated code or edits.

Test at least 3 cases in VS Code or terminal.

### Step 5: Submit to OJ

Submit the final code yourself.

Record:

- OJ submission ID,
- OJ status.

### Step 6: Complete `submission.md`

Finish all sections.

Do not paste full source code into GitHub.

Use the OJ submission ID instead.

### Step 7: Complete `ai_reflection.md`

Copy `AI_REFLECTION_TEMPLATE.md` and rename it:

```text
ai_reflection.md
```

Explain:

- OJ problem number/title,
- OJ submission ID,
- OJ status,
- which AI tool you used,
- whether you used `COURSE_AI_INSTRUCTIONS.md`,
- whether you read and followed the relevant workflow,
- what you asked AI to help with,
- what AI helped you notice,
- what you checked or changed by yourself,
- what you learned.

### Step 8: Push to GitHub

The folder should contain:

```text
oj002/
├── submission.md
└── ai_reflection.md
```

---

## 17. What Not to Put in GitHub

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

## 18. Quick Self-Check

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

## 19. Final Reminder

AI coding tools can be powerful.

They can help you think, debug, test, and learn.

They can also make it easy to submit code you do not understand.

Use them carefully.

Your final OJ submission is your responsibility.
