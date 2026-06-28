# Student Workflow for Claude Code

This file explains how students should use Claude Code responsibly in this course.

This document is written for students who are new to Claude Code.

Read this file before using Claude Code on any OJ problem.

---

## 1. What Is Claude Code?

Claude Code is an AI coding tool from Anthropic.

It is different from normal Claude web chat.

Normal Claude web chat is used mainly by typing messages in a browser or chat window.

Claude Code can work more directly with code.

Depending on the version or interface, Claude Code may be able to:

- read code files,
- read a project folder,
- suggest code changes,
- edit files,
- run commands,
- run Python code,
- help debug code,
- help review code,
- help create test cases.

Because Claude Code can work with files and commands, it must be used carefully.

---

## 2. Claude Tools Students May See

Students may see Claude in three main ways.

| Tool | How it is used | Which workflow to follow |
|---|---|---|
| Claude web chat | Use Claude in a browser as normal chat | `workflows/STUDENT_WORKFLOW_WEB_CHAT.md` |
| Claude desktop app | Downloaded Claude app. It may include normal Claude chat, Claude Code, or Claude Cowork depending on account and features | Use only if the instructor allows it |
| Claude Code CLI | Terminal tool started with the `claude` command | This file |

For this course, the recommended Claude Code workflow is:

```text
VS Code + Claude Code CLI
```

This means:

1. You write and test code in VS Code.
2. You open the VS Code terminal.
3. You run Claude Code CLI from the VS Code terminal.
4. Claude helps you review, debug, explain, or test your code.

The Claude desktop app, Claude Code inside the desktop app, and Claude Cowork may be used only if the instructor explicitly allows them.

Even when using those tools, students must still:

- use VS Code as the official editor,
- test final code in VS Code,
- submit final code to the OJ by themselves,
- follow the course AI policy,
- understand the final code.

---

## 3. Course Rule: VS Code Is Still the Official Editor

VS Code is the official editor for this course.

Students must use VS Code for:

- writing Python code,
- running Python code,
- testing Python code,
- preparing final code before OJ submission.

Claude Code is only an assistant.

Claude Code is not the official editor.

Claude Code is not the place where students submit answers.

The course OJ is still the official place for code submission.

---

## 4. What Claude Code Is Allowed to Help With

Claude Code may help students:

- review a first plan,
- explain a Python concept,
- explain an error message,
- find a bug in code the student already wrote,
- suggest test cases,
- check input and output logic,
- explain why a test case fails,
- suggest a small code improvement after explaining the reason.

Claude Code must not replace the student's own thinking.

Students must not use Claude Code to:

- solve the whole OJ problem from zero,
- generate complete accepted code without their own attempt,
- rewrite the whole solution without understanding,
- submit to the OJ,
- write `submission.md` for the student,
- write `ai_reflection.md` for the student,
- invent fake test results,
- invent fake OJ results.

If the student cannot explain the final code, the student should not submit it.

---

## 5. Before Using Claude Code

Before using Claude Code on any OJ problem, do these steps first.

### Step 1: Read the OJ Problem Yourself

Read the problem statement in the course OJ.

Do not ask Claude Code immediately.

### Step 2: Think by Yourself First

Before using Claude Code, students must already have their own attempt.

At minimum, students should know or write:

```text
Problem understanding:
Input:
Output:
Constraints:
First plan:
```

If the problem is learning-log required, write this in `submission.md`.

If the problem is not learning-log required, this may be a private note or handwritten note.

The first understanding may be incomplete or incorrect.

That is okay.

The important point is that the student tried before using Claude Code.

---

## 6. Install Claude Code CLI

Claude Code CLI is an app/command-line tool.

Students must install it before they can run the `claude` command.

If Claude Code CLI is already installed on the computer or lab computer, skip this section.

### Windows PowerShell

Open Windows PowerShell.

Run this command:

```powershell
irm https://claude.ai/install.ps1 | iex
```

After installation, check that Claude Code works:

```powershell
claude
```

The first time Claude Code runs, it will ask the user to sign in.

Sign in with a Claude or Anthropic account if the account supports Claude Code.

### macOS, Linux, or WSL

Open Terminal.

Run this command:

```bash
curl -fsSL https://claude.ai/install.sh | bash
```

After installation, check that Claude Code works:

```bash
claude
```

The first time Claude Code runs, it will ask the user to sign in.

### If Installation Fails

Do not try random commands from the internet.

Ask the instructor or TA.

For this course, use only the installation method provided by the instructor or the official Claude Code documentation.

---

## 7. Create the Course Project Folder

Create one main folder for this course.

Recommended folder name:

```text
pscp
```

Inside `pscp`, keep OJ working folders.

Example:

```text
pscp/
├── AGENTS.md
├── CLAUDE.md
├── oj001_work/
│   └── main.py
├── oj002_work/
│   └── main.py
└── oj003_work/
    └── main.py
```

For OJ problem 002, create:

```text
pscp/oj002_work/main.py
```

Use `main.py` for local coding and testing.

Do not upload `main.py` or `solution.py` to the public GitHub learning log.

For the GitHub learning log, use only:

```text
submission.md
ai_reflection.md, if AI was used
```

---

## 8. Add Course Instructions for Claude Code

Claude Code reads project instructions from a file named:

```text
CLAUDE.md
```

For this course, the repository provides a ready-to-use Claude instruction file:

```text
instructions/CLAUDE.md
```

This file imports the shared course AI rules from:

```text
instructions/AGENTS.md
```

Students should copy both files into their local course folder:

```text
pscp/AGENTS.md
pscp/CLAUDE.md
```

Recommended local structure:

```text
pscp/
├── AGENTS.md
├── CLAUDE.md
├── oj001_work/
│   └── main.py
└── oj002_work/
    └── main.py
```

Students should not write their own `CLAUDE.md`.

Students should not copy random instructions from the internet into `CLAUDE.md`.

### Why Two Files?

`AGENTS.md` contains the shared course AI rules.

`CLAUDE.md` is the file that Claude Code reads.

In this course, `CLAUDE.md` imports `AGENTS.md` by using:

```markdown
@AGENTS.md
```

This avoids copying the same course rules into many files.

### Important

Always start Claude Code from the `pscp` folder.

This helps Claude Code find and follow `CLAUDE.md`.

---

## 9. Open the Project in VS Code

Open VS Code.

Open the folder:

```text
pscp
```

Do not open only `oj002_work`.

Open the main `pscp` folder so that you can see:

```text
AGENTS.md
CLAUDE.md
oj002_work/
```

Then create or open:

```text
oj002_work/main.py
```

Write your first code attempt in `main.py`.

---

## 10. Start Claude Code CLI from VS Code

In VS Code, open:

```text
Terminal > New Terminal
```

Make sure the terminal is at the `pscp` folder.

On macOS, Linux, or WSL, check with:

```bash
pwd
```

On Windows PowerShell, check with:

```powershell
Get-Location
```

The path should end with:

```text
pscp
```

Then run:

```bash
claude
```

If Claude Code asks you to sign in, sign in with your Claude or Anthropic account.

---

## 11. First Prompt to Claude Code

Do not ask Claude Code to solve the problem.

Start with your own attempt.

Good first prompt:

```text
I am solving an OJ problem for my PSCP course.

Follow CLAUDE.md.

Use VS Code workflow.

Do not write the full solution.

Only look at this file:
oj002_work/main.py

Here is my current understanding:
...

Input:
...

Output:
...

Constraints:
...

My first plan:
...

Please review my plan and tell me:
1. what seems correct,
2. what may be missing,
3. one small next step.

Do not edit files yet.
Do not run commands yet.
```

Replace `oj002_work/main.py` with the actual folder name.

---

## 12. If You Want Claude Code to Review Code

Use this kind of prompt:

```text
Please review oj002_work/main.py.

Do not rewrite the whole file.

First explain:
1. what my code is trying to do,
2. whether it matches my first plan,
3. one possible bug or missing case.

Do not edit the file yet.
Do not run commands yet.
```

---

## 13. If You Want Claude Code to Debug

Use this kind of prompt:

```text
My code fails this test case.

File:
oj002_work/main.py

Input:
...

Expected output:
...

Actual output:
...

Please explain the likely bug first.

Do not rewrite the whole file.

Suggest the smallest change only.

Do not edit the file until I approve.
```

---

## 14. If You Want Claude Code to Suggest Test Cases

Use this kind of prompt:

```text
Please suggest 3 useful test cases for this problem.

Do not solve the problem.

For each test case, include:
1. why this case is useful,
2. input,
3. expected output.

Do not use hidden OJ tests.
```

After Claude Code suggests test cases, students must run them by themselves in VS Code.

---

## 15. If You Allow Claude Code to Edit Code

Claude Code may ask to edit a file or suggest a patch.

Before allowing edits, ask:

```text
Explain what you plan to change before editing the file.
```

Then, if the change is reasonable, allow only a small edit.

Good instruction:

```text
Apply only the smallest necessary change to oj002_work/main.py.

Do not rewrite unrelated parts of the file.

After editing, explain what changed and why.
```

After Claude Code edits the file:

1. Open `main.py` in VS Code.
2. Read the changed code.
3. Make sure you understand it.
4. Run the code yourself.
5. Test at least 3 different cases.

If Claude Code changes too much, reject the change or ask it to simplify.

---

## 16. Running Your Code

Run the code in the VS Code terminal.

Example:

```bash
python oj002_work/main.py
```

or:

```bash
python3 oj002_work/main.py
```

Test at least 3 different cases.

For each case, students should know:

- why this test case was chosen,
- expected output,
- actual output,
- whether it passed.

Claude Code may help suggest tests, but students are responsible for running and checking them.

---

## 17. Submit to the OJ Yourself

After testing, submit the final code to the course OJ by yourself.

Do not ask Claude Code to submit for you.

If the problem is learning-log required, record:

- OJ problem number/title,
- OJ submission ID,
- OJ status.

---

## 18. Learning-Log-Required Problems

If the OJ problem is learning-log required and Claude Code was used, submit:

```text
submission.md
ai_reflection.md
```

### In `submission.md`

Write in your own words:

- OJ information,
- independent time spent before AI,
- problem understanding,
- first plan,
- final approach,
- at least 3 test cases.

Do not include full source code in GitHub.

Use the OJ submission ID instead.

### In `ai_reflection.md`

Write your own reflection.

Mention:

- that you used Claude Code,
- whether you used `CLAUDE.md`,
- whether you copied `instructions/AGENTS.md` and `instructions/CLAUDE.md` into the local `pscp` folder,
- whether you followed this workflow,
- what you asked Claude Code to help with,
- what Claude Code helped you notice,
- what you checked or changed by yourself,
- what you learned.

Do not paste the full Claude Code conversation.

Do not ask Claude Code to write your reflection for you.

---

## 19. Normal OJ Problems

If the problem is not learning-log required:

- submit code to the OJ only,
- no GitHub learning log is required,
- no `submission.md` is required,
- no `ai_reflection.md` is required.

However, students must still understand the final code.

The instructor may ask students to explain:

- problem understanding,
- algorithm,
- code,
- test cases,
- what Claude Code helped with,
- what the student verified by themselves.

---

## 20. What Not to Put in the `pscp` Folder

Do not put these in the `pscp` folder:

- API keys,
- access tokens,
- private files,
- hidden OJ tests,
- official solutions,
- unrelated personal files,
- course-restricted materials that should not be copied.

For OJ work folders, keep only what is needed for coding and testing.

For example:

```text
pscp/oj002_work/main.py
```

Optional files such as `input.txt` may be used only for local testing.

Do not upload source code files to the public GitHub learning log.

---

## 21. Good Claude Code Prompts

### Plan Review

```text
Please review my first plan.

Do not write the full code.

Tell me:
1. what seems correct,
2. what may be missing,
3. one question I should think about next.
```

### Code Review

```text
Please review oj002_work/main.py.

Do not edit the file yet.

Explain one possible issue and suggest one small next step.
```

### Debugging

```text
My code fails this test case.

Input:
...

Expected output:
...

Actual output:
...

Please explain the likely bug first.

Do not rewrite the whole code.
```

### Small Code Fix

```text
Suggest the smallest code change needed.

Explain why it works.

Do not rewrite unrelated parts of the file.
```

### Test Cases

```text
Please suggest 3 useful test cases.

Do not solve the problem.

For each test case, explain why it is useful.
```

---

## 22. Bad Claude Code Prompts

Avoid prompts like these:

```text
Solve this OJ problem.
```

```text
Write the full accepted code.
```

```text
Make my code pass the OJ.
```

```text
Rewrite the whole file.
```

```text
Edit everything until it works.
```

```text
Submit this to the OJ.
```

```text
Write my submission.md.
```

```text
Write my ai_reflection.md.
```

---

## 23. If Claude Code Gives Too Much Help

Sometimes Claude Code may give a full solution too early.

Do not copy it immediately.

Reply:

```text
Please stop giving the full solution.

Explain only the main idea and ask me guiding questions.

I want to write the code myself.
```

Then write your own code in VS Code.

You may use the explanation to improve your understanding, but you must not submit code you cannot explain.

---

## 24. If Claude Code Edits Too Much Code

If Claude Code changes too many lines, ask it to reduce the change.

Prompt:

```text
This change is too large.

Please explain the smallest necessary change only.

Do not rewrite unrelated code.
```

You may reject Claude Code's change and write your own simpler version.

---

## 25. Commands: Be Careful

Claude Code may run commands.

For this course, common safe commands are usually:

```bash
python oj002_work/main.py
```

or:

```bash
python3 oj002_work/main.py
```

Be careful with commands that:

- delete files,
- reset Git history,
- install packages,
- upload files,
- expose secrets,
- modify unrelated folders,
- commit or push accidentally.

For beginner PSCP problems, most package installation commands are not needed.

If you do not understand a command, do not allow it.

Ask:

```text
Explain what this command does before running it.
```

---

## 26. Optional: Claude Desktop App, Claude Code in the App, or Claude Cowork

For this course, the main recommended workflow is:

```text
VS Code + Claude Code CLI
```

The Claude desktop app, Claude Code inside the desktop app, and Claude Cowork may be used only if the instructor explicitly allows them.

If allowed, students must still follow these rules:

1. Use VS Code as the official editor.
2. Use the `pscp` project folder.
3. Use the course AI rules.
4. Use Claude only as a coach, reviewer, debugger, or test-case helper.
5. Do not ask Claude to solve the whole OJ problem from zero.
6. Do not let Claude submit to the OJ.
7. Write, run, and test the final code in VS Code.
8. If the problem is learning-log required, complete `submission.md` and `ai_reflection.md`.

For beginner PSCP work, the terminal CLI workflow is simpler and easier to control.

---

## 27. Quick Self-Check

This checklist is only for self-checking.

Students do not need to submit this checklist.

Before submitting to the OJ, make sure that:

```text
[ ] I used VS Code to write, run, and test my code.
[ ] I wrote my own problem understanding before using Claude Code.
[ ] I wrote my own first plan before using Claude Code.
[ ] I copied AGENTS.md and CLAUDE.md into the pscp folder.
[ ] I used Claude Code as a coach, reviewer, debugger, or test-case helper.
[ ] I reviewed any Claude Code-generated code or edits.
[ ] I tested at least 3 different cases by myself.
[ ] I understand my final code.
[ ] I can explain what Claude Code helped with.
```

If the problem is learning-log required, complete:

```text
submission.md
ai_reflection.md
```

---

## 28. Final Reminder

Claude Code is powerful because it can work with files and commands.

This also makes it risky if used carelessly.

Use Claude Code to learn, review, debug, and test.

Do not use Claude Code to replace your own problem solving.

Your final OJ submission is your responsibility.
