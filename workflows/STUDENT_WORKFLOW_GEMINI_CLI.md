# Student Workflow for Gemini CLI

This file explains how students should use Gemini CLI responsibly in this course.

This document is written for students who are new to Gemini CLI.

Read this file before using Gemini CLI on any OJ problem.

---

## 1. What Is Gemini CLI?

Gemini CLI is an AI coding agent from Google that runs in a terminal.

It is different from normal Gemini web chat.

Normal Gemini web chat is used mainly by typing messages in a browser or chat window.

Gemini CLI can work more directly with code and project folders.

Depending on the configuration, Gemini CLI may be able to:

- read project files,
- read code files,
- suggest code changes,
- edit files,
- run commands,
- use built-in tools such as file read, file write, grep, and terminal,
- use MCP servers if configured,
- help debug code,
- help review code,
- help create or improve test cases,
- use a project context file such as `GEMINI.md`.

Because Gemini CLI can work with files, tools, and commands, it must be used carefully.

---

## 2. Gemini Tools Students May See

Students may see Gemini in three main ways.

| Tool | How it is used | Which workflow to follow |
|---|---|---|
| Gemini web chat | Use Gemini in a browser as normal chat | `workflows/STUDENT_WORKFLOW_WEB_CHAT.md` |
| Gemini Code Assist in VS Code | Gemini inside VS Code. Agent mode may be powered by Gemini CLI and may use tools | Use only if the instructor allows it |
| Gemini CLI | Terminal tool started with the `gemini` command | This file |

For this course, the recommended Gemini workflow is:

```text
VS Code + Gemini CLI
```

This means:

1. You write and test code in VS Code.
2. You open the VS Code terminal.
3. You run Gemini CLI from the VS Code terminal.
4. Gemini helps you review, debug, explain, or test your code.

Gemini Code Assist agent mode in VS Code may be used only if the instructor explicitly allows it.

Even when using Gemini Code Assist agent mode, students must still:

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

Gemini CLI is only an assistant.

Gemini CLI is not the official editor.

Gemini CLI is not the place where students submit answers.

The course OJ is still the official place for code submission.

---

## 4. What Gemini CLI Is Allowed to Help With

Gemini CLI may help students:

- review a first plan,
- explain a Python concept,
- explain an error message,
- find a bug in code the student already wrote,
- suggest test cases,
- check input and output logic,
- explain why a test case fails,
- suggest a small code improvement after explaining the reason.

Gemini CLI must not replace the student's own thinking.

Students must not use Gemini CLI to:

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

## 5. Before Using Gemini CLI

Before using Gemini CLI on any OJ problem, do these steps first.

### Step 1: Read the OJ Problem Yourself

Read the problem statement in the course OJ.

Do not ask Gemini CLI immediately.

### Step 2: Think by Yourself First

Before using Gemini CLI, students must already have their own attempt.

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

The important point is that the student tried before using Gemini CLI.

---

## 6. Install Gemini CLI

Gemini CLI is an app/command-line tool.

Students must install it before they can run the `gemini` command.

If Gemini CLI is already installed on the computer or lab computer, skip this section.

### Requirement

Gemini CLI requires Node.js 20.0.0 or newer.

### macOS, Linux, or WSL

Open Terminal.

Check your Node.js version:

```bash
node --version
```

If Node.js is not installed, follow the instructor's setup method before installing Gemini CLI.

Install Gemini CLI:

```bash
npm install -g @google/gemini-cli
```

After installation, check that Gemini CLI works:

```bash
gemini
```

The first time Gemini CLI runs, it may ask the user to sign in or choose an authentication method.

### Windows PowerShell

Open Windows PowerShell.

Check your Node.js version:

```powershell
node --version
```

If Node.js is not installed, follow the instructor's setup method before installing Gemini CLI.

Install Gemini CLI:

```powershell
npm install -g @google/gemini-cli
```

After installation, check that Gemini CLI works:

```powershell
gemini
```

The first time Gemini CLI runs, it may ask the user to sign in or choose an authentication method.

### Optional: Run With npx

If the instructor allows it, Gemini CLI can also be run without permanent installation.

On macOS, Linux, or WSL:

```bash
npx @google/gemini-cli
```

On Windows PowerShell:

```powershell
npx @google/gemini-cli
```

For regular course use, installing with `npm install -g @google/gemini-cli` is usually easier.

### If Installation Fails

Do not try random commands from the internet.

Do not install packages with similar-looking names.

For this course, use the official package:

```text
@google/gemini-cli
```

Ask the instructor or TA if installation fails.

---

## 7. Sign In or Authentication

The first time you run:

```bash
gemini
```

Gemini CLI may ask you to choose an authentication method.

Use the method provided by the instructor.

If the instructor does not provide a specific method, follow the Gemini CLI sign-in instructions.

Do not put API keys, credentials, or tokens in a public GitHub repository.

Do not commit `.env` files that contain keys or tokens.

If you are not sure whether API keys are allowed, ask the instructor first.

---

## 8. Create the Course Project Folder

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
├── GEMINI.md
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

## 9. Add Course Instructions for Gemini CLI

Gemini CLI reads project context from a file named:

```text
GEMINI.md
```

For this course, the repository provides a ready-to-use Gemini instruction file:

```text
instructions/GEMINI.md
```

This file imports the shared course AI rules from:

```text
instructions/AGENTS.md
```

Students should copy both files into their local course folder:

```text
pscp/AGENTS.md
pscp/GEMINI.md
```

Recommended local structure:

```text
pscp/
├── AGENTS.md
├── GEMINI.md
├── oj001_work/
│   └── main.py
└── oj002_work/
    └── main.py
```

Students should not write their own `GEMINI.md`.

Students should not copy random instructions from the internet into `GEMINI.md`.

### Why Two Files?

`AGENTS.md` contains the shared course AI rules.

`GEMINI.md` is the file that Gemini CLI reads by default.

In this course, `GEMINI.md` imports `AGENTS.md` by using:

```markdown
@AGENTS.md
```

This avoids copying the same course rules into many files.

### Important

Always start Gemini CLI from the `pscp` folder.

This helps Gemini CLI find and follow `GEMINI.md`.

---

## 10. Open the Project in VS Code

Open VS Code.

Open the folder:

```text
pscp
```

Do not open only `oj002_work`.

Open the main `pscp` folder so that you can see:

```text
AGENTS.md
GEMINI.md
oj002_work/
```

Then create or open:

```text
oj002_work/main.py
```

Write your first code attempt in `main.py`.

---

## 11. Start Gemini CLI from VS Code

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
gemini
```

If Gemini CLI asks you to sign in, sign in using the method provided by the instructor.

---

## 12. First Prompt to Gemini CLI

Do not ask Gemini CLI to solve the problem.

Start with your own attempt.

Good first prompt:

```text
I am solving an OJ problem for my PSCP course.

Follow GEMINI.md.

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

## 13. If You Want Gemini CLI to Review Code

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

## 14. If You Want Gemini CLI to Debug

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

## 15. If You Want Gemini CLI to Suggest Test Cases

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

After Gemini CLI suggests test cases, students must run them by themselves in VS Code.

---

## 16. If You Allow Gemini CLI to Edit Code

Gemini CLI may ask to edit a file or suggest a patch.

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

After Gemini CLI edits the file:

1. Open `main.py` in VS Code.
2. Read the changed code.
3. Make sure you understand it.
4. Run the code yourself.
5. Test at least 3 different cases.

If Gemini CLI changes too much, reject the change or ask it to simplify.

---

## 17. Running Your Code

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

Gemini CLI may help suggest tests, but students are responsible for running and checking them.

---

## 18. Submit to the OJ Yourself

After testing, submit the final code to the course OJ by yourself.

Do not ask Gemini CLI to submit for you.

If the problem is learning-log required, record:

- OJ problem number/title,
- OJ submission ID,
- OJ status.

---

## 19. Learning-Log-Required Problems

If the OJ problem is learning-log required and Gemini CLI was used, submit:

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

- that you used Gemini CLI,
- whether you used `GEMINI.md`,
- whether you copied `instructions/AGENTS.md` and `instructions/GEMINI.md` into the local `pscp` folder,
- whether you followed this workflow,
- what you asked Gemini CLI to help with,
- what Gemini CLI helped you notice,
- what you checked or changed by yourself,
- what you learned.

Do not paste the full Gemini CLI conversation.

Do not ask Gemini CLI to write your reflection for you.

---

## 20. Normal OJ Problems

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
- what Gemini CLI helped with,
- what the student verified by themselves.

---

## 21. What Not to Put in the `pscp` Folder

Do not put these in the `pscp` folder:

- API keys,
- access tokens,
- private files,
- hidden OJ tests,
- official solutions,
- unrelated personal files,
- course-restricted materials that should not be copied,
- `.env` files that contain keys or tokens.

For OJ work folders, keep only what is needed for coding and testing.

For example:

```text
pscp/oj002_work/main.py
```

Optional files such as `input.txt` may be used only for local testing.

Do not upload source code files to the public GitHub learning log.

---

## 22. Good Gemini CLI Prompts

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

## 23. Bad Gemini CLI Prompts

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

## 24. If Gemini CLI Gives Too Much Help

Sometimes Gemini CLI may give a full solution too early.

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

## 25. If Gemini CLI Edits Too Much Code

If Gemini CLI changes too many lines, ask it to reduce the change.

Prompt:

```text
This change is too large.

Please explain the smallest necessary change only.

Do not rewrite unrelated code.
```

You may reject Gemini CLI's change and write your own simpler version.

---

## 26. Commands and Auto Modes: Be Careful

Gemini CLI may run commands and use tools.

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

### Do Not Use YOLO or Auto-Accept Mode

Do not use:

```bash
gemini --yolo
```

Do not turn on auto-accept mode.

YOLO mode and auto-accept mode can allow Gemini CLI to approve tool calls automatically.

For this course, students should review and approve actions manually.

---

## 27. Optional: Gemini Code Assist Agent Mode in VS Code

For this course, the main recommended workflow is:

```text
VS Code + Gemini CLI
```

Gemini Code Assist agent mode in VS Code may be used only if the instructor explicitly allows it.

If allowed, students must still follow these rules:

1. Use VS Code as the official editor.
2. Use the `pscp` project folder.
3. Use the course AI rules.
4. Use Gemini only as a coach, reviewer, debugger, or test-case helper.
5. Do not ask Gemini to solve the whole OJ problem from zero.
6. Do not let Gemini submit to the OJ.
7. Write, run, and test the final code in VS Code.
8. If the problem is learning-log required, complete `submission.md` and `ai_reflection.md`.

For beginner PSCP work, the terminal CLI workflow is simpler and easier to control.

---

## 28. Quick Self-Check

This checklist is only for self-checking.

Students do not need to submit this checklist.

Before submitting to the OJ, make sure that:

```text
[ ] I used VS Code to write, run, and test my code.
[ ] I wrote my own problem understanding before using Gemini CLI.
[ ] I wrote my own first plan before using Gemini CLI.
[ ] I copied AGENTS.md and GEMINI.md into the pscp folder.
[ ] I used Gemini CLI as a coach, reviewer, debugger, or test-case helper.
[ ] I reviewed any Gemini CLI-generated code or edits.
[ ] I did not use YOLO mode or auto-accept mode.
[ ] I tested at least 3 different cases by myself.
[ ] I understand my final code.
[ ] I can explain what Gemini CLI helped with.
```

If the problem is learning-log required, complete:

```text
submission.md
ai_reflection.md
```

---

## 29. Final Reminder

Gemini CLI is powerful because it can work with files, tools, and commands.

This also makes it risky if used carelessly.

Use Gemini CLI to learn, review, debug, and test.

Do not use Gemini CLI to replace your own problem solving.

Your final OJ submission is your responsibility.
