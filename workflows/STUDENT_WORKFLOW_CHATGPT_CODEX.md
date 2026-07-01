# Student Workflow for ChatGPT Codex

This file explains how students should use ChatGPT Codex / OpenAI Codex / Codex CLI responsibly in this course.

This document is written for students who are new to Codex.

Read this file before using Codex on any OJ problem.

For shared lab computers, replace `<student-id>` with your own student ID, for example `pscp-66123456/`, and use only your own folder.

---

## 1. What Is Codex?

Codex is an AI coding tool from OpenAI.

It is different from normal ChatGPT web chat.

Normal ChatGPT web chat usually answers your messages in a browser.

Codex can work more directly with code.

Depending on the version, Codex may be able to:

- read code files,
- suggest changes,
- edit files,
- run commands,
- run Python code,
- inspect a project folder,
- help debug code.

Because Codex can work with files and commands, it must be used carefully.

---

## 2. Which Codex Version Does This File Cover?

This workflow covers:

- ChatGPT Codex,
- OpenAI Codex,
- Codex CLI,
- Codex app, only if explicitly allowed by the instructor,
- Codex in an IDE or coding environment, if available.

For this course, the recommended Codex workflow is:

```text
VS Code + Codex CLI
```

This means:

1. You write and test code in VS Code.
2. You open the VS Code terminal.
3. You run Codex CLI from the VS Code terminal.
4. Codex helps you review, debug, or test your code.

The Codex app may be used only if the instructor explicitly allows it.

Even when using the Codex app, students must still:

- use VS Code as the official editor,
- test final code in VS Code,
- submit final code to the OJ by themselves,
- follow the course AI policy,
- use the provided `AGENTS.md` file if the app supports project instructions or project context.

If you use ChatGPT only as normal browser chat, use:

```text
workflows/STUDENT_WORKFLOW_WEB_CHAT.md
```

Other AI coding tools are not part of the course workflow unless the instructor announces a separate workflow.

---

## 3. Course Rule: VS Code Is Still the Official Editor

VS Code is the official editor for this course.

Students must use VS Code for writing, running, testing, and preparing final code before OJ submission.

Codex is only an assistant.

Codex is not the official editor.

Codex is not the place where you submit your answer.

The course OJ is still the official place for code submission.

---

## 4. What Codex Is Allowed to Help With

Codex may help you:

- review your first plan,
- explain a Python concept,
- explain an error message,
- find a bug in code you already wrote,
- suggest test cases,
- check input and output logic,
- explain why a test case fails,
- suggest a small code improvement after explaining the reason.

Codex must not replace your own thinking.

You must not use Codex to:

- solve the whole OJ problem from zero,
- generate complete accepted code without your own attempt,
- rewrite the whole solution without explanation,
- submit to the OJ,
- write `submission.md` for you,
- write `ai_reflection.md` for you,
- invent fake test results,
- invent fake OJ results.

If you cannot explain the final code, you should not submit it.

---

## 5. Before Using Codex

Before using Codex on any OJ problem, do these steps first.

### Step 1: Read the OJ Problem Yourself

Read the problem statement in the course OJ.

Do not ask Codex immediately.

### Step 2: Think by Yourself First

Before using Codex, you must already have your own attempt.

At minimum, you should know or write:

```text
Problem understanding:
Input:
Output:
Constraints:
First plan:
```

If the problem is learning-log required, write this in `submission.md`.

If the problem is not learning-log required, this may be a private note or handwritten note.

Your understanding may be incomplete or incorrect.

That is okay.

The important point is that you tried before using Codex.

---

## 6. Install Codex CLI

Codex CLI is an app/command-line tool.

You must install it before you can run the `codex` command.

If Codex CLI is already installed on your computer or lab computer, skip this section.

### Windows PowerShell

Open Windows PowerShell.

Run this command:

```powershell
powershell -ExecutionPolicy ByPass -c "irm https://chatgpt.com/codex/install.ps1 | iex"
```

After installation, check that Codex works:

```powershell
codex
```

The first time you run Codex, it will ask you to sign in.

Sign in with your ChatGPT account if your plan supports Codex.

### macOS or Linux

Open Terminal and run:

```bash
curl -fsSL https://chatgpt.com/codex/install.sh | sh
```

After installation, check that Codex works:

```bash
codex
```

The first time you run Codex, it will ask you to sign in.

Sign in with your ChatGPT account if your plan supports Codex.

### If Installation Fails

Do not try random commands from the internet.

Ask the instructor or TA.

For this course, use only the installation method provided by the instructor or the official Codex documentation.

---

## 7. Create the Course Project Folder

Create one main folder for this course.

Recommended folder name:

```text
pscp
```

Inside `pscp-<student-id>`, keep your OJ working folders.

Example:

```text
pscp-<student-id>/
├── AGENTS.md
├── oj2198_work/
│   └── main.py
├── oj0301_work/
│   └── main.py
└── oj1994_work/
    └── main.py
```

For OJ problem 0301, create:

```text
pscp-<student-id>/oj0301_work/main.py
```

Use `main.py` for local coding and testing.

Do not upload `main.py` or `solution.py` to your public GitHub learning log.

For the GitHub learning log, use only:

```text
submission.md
ai_reflection.md, if AI was used
```

---

## 8. Add the Course `AGENTS.md` File

Codex can use a file named:

```text
AGENTS.md
```

For this course, the instructor provides a ready-to-use file at:

```text
instructions/AGENTS.md
```

Students should copy this file into their local course folder as:

```text
pscp-<student-id>/AGENTS.md
```

Students should not write their own `AGENTS.md`.

Students should not copy random instructions from the internet into `AGENTS.md`.

Students do not need to manually copy the full `instructions/COURSE_AI_INSTRUCTIONS.md` into Codex each time.

The provided `instructions/AGENTS.md` already contains the course AI rules.

### Important

Always start Codex from the `pscp-<student-id>` folder.

This helps Codex find and follow the course `AGENTS.md`.

---

## 9. Open the Project in VS Code

Open VS Code.

Open the folder:

```text
pscp
```

Do not open only `oj0301_work`.

Open the main `pscp-<student-id>` folder so that you can see:

```text
AGENTS.md
oj0301_work/
```

Then create or open:

```text
oj0301_work/main.py
```

Write your first code attempt in `main.py`.

---

## 10. Start Codex CLI from VS Code

In VS Code, open:

```text
Terminal > New Terminal
```

Make sure the terminal is at the `pscp-<student-id>` folder.

You can check with:

```bash
pwd
```

On Windows PowerShell, you can also use:

```powershell
Get-Location
```

The path should end with:

```text
pscp
```

Then run:

```bash
codex
```

If Codex asks you to sign in, sign in with your ChatGPT account.

---

## 11. First Prompt to Codex

Do not ask Codex to solve the problem.

Start with your own attempt.

Good first prompt:

```text
I am solving an OJ problem for my PSCP course.

Follow AGENTS.md.

Use VS Code workflow.

Do not write the full solution.

Only look at this file:
oj0301_work/main.py

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
```

Replace `oj0301_work/main.py` with your actual folder name.

---

## 12. If You Want Codex to Review Code

Use this kind of prompt:

```text
Please review oj0301_work/main.py.

Do not rewrite the whole file.

First explain:
1. what my code is trying to do,
2. whether it matches my first plan,
3. one possible bug or missing case.

Do not edit the file yet.
```

---

## 13. If You Want Codex to Debug

Use this kind of prompt:

```text
My code fails this test case.

File:
oj0301_work/main.py

Input:
...

Expected output:
...

Actual output:
...

Please explain the likely bug first.

Do not rewrite the whole file.

Suggest the smallest change only.
```

---

## 14. If You Want Codex to Suggest Test Cases

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

After Codex suggests test cases, you must run them yourself in VS Code.

---

## 15. If You Allow Codex to Edit Code

Codex may ask to edit a file or suggest a patch.

Before allowing edits, ask:

```text
Explain what you plan to change before editing the file.
```

Then, if the change is reasonable, allow only a small edit.

Good instruction:

```text
Apply only the smallest necessary change to oj0301_work/main.py.

Do not rewrite unrelated parts of the file.

After editing, explain what changed and why.
```

After Codex edits the file:

1. Open `main.py` in VS Code.
2. Read the changed code.
3. Make sure you understand it.
4. Run the code yourself.
5. Test at least 3 different cases.

If Codex changes too much, reject the change or ask it to simplify.

---

## 16. Running Your Code

Run your code in the VS Code terminal.

Example:

```bash
python oj0301_work/main.py
```

or:

```bash
python3 oj0301_work/main.py
```

Test at least 3 different cases.

For each case, you should know:

- why you chose this case,
- expected output,
- actual output,
- whether it passed.

Codex may help suggest tests, but you are responsible for running and checking them.

---

## 17. Submit to the OJ Yourself

After testing, submit your final code to the course OJ yourself.

Do not ask Codex to submit for you.

If the problem is learning-log required, record:

- OJ problem number/title,
- OJ submission ID,
- OJ status.

---

## 18. Learning-Log-Required Problems

If the OJ problem is learning-log required and you used Codex, submit:

```text
submission.md
ai_reflection.md
```

### In `submission.md`

Write your own:

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

- that you used Codex,
- whether you used the course `AGENTS.md`,
- whether you followed this workflow,
- what you asked Codex to help with,
- what Codex helped you notice,
- what you checked or changed by yourself,
- what you learned.

Do not paste the full Codex conversation.

Do not ask Codex to write your reflection for you.

---

## 19. Normal OJ Problems

If the problem is not learning-log required:

- submit code to the OJ only,
- no GitHub learning log is required,
- no `submission.md` is required,
- no `ai_reflection.md` is required.

However, you must still understand your final code.

The instructor may ask you to explain:

- your problem understanding,
- your algorithm,
- your code,
- your test cases,
- what Codex helped with,
- what you verified by yourself.

---

## 20. What Not to Put in the `pscp-<student-id>` Folder

Do not put these in the `pscp-<student-id>` folder:

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
pscp-<student-id>/oj0301_work/main.py
```

Optional files such as `input.txt` may be used only for your own local testing.

Do not upload source code files to the public GitHub learning log.

---

## 21. Good Codex Prompts

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
Please review oj0301_work/main.py.

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

### Small Fix

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

## 22. Bad Codex Prompts

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

## 23. If Codex Gives Too Much Help

Sometimes Codex may give a full solution too early.

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

## 24. If Codex Edits Too Much Code

If Codex changes too many lines, ask it to reduce the change.

Prompt:

```text
This change is too large.

Please explain the smallest necessary change only.

Do not rewrite unrelated code.
```

You may reject Codex's change and write your own simpler version.

---

## 25. Commands: Be Careful

Codex may run commands.

For this course, common safe commands are usually:

```bash
python oj0301_work/main.py
```

or:

```bash
python3 oj0301_work/main.py
```

Be careful with commands that:

- delete files,
- reset Git history,
- install packages,
- upload files,
- expose secrets,
- modify unrelated folders.

For beginner PSCP problems, most package installation commands are not needed.

If you do not understand a command, do not allow it.

Ask:

```text
Explain what this command does before running it.
```

---

## 26. Optional: Using the Codex App

The Codex app is available on macOS and Windows.

However, for this course, the Codex app is not the main recommended workflow.

The main recommended workflow is:

```text
VS Code + Codex CLI
```

Students may use the Codex app only if the instructor explicitly allows it.

If the instructor allows the Codex app, students must still follow these rules:

1. Choose the `pscp-<student-id>` folder as the project folder.
2. Make sure the provided `AGENTS.md` file is inside the `pscp-<student-id>` folder.
3. Use Codex only as a coach, reviewer, debugger, or test-case helper.
4. Do not ask Codex to solve the whole OJ problem from zero.
5. Do not let Codex submit to the OJ.
6. Write, run, and test the final code in VS Code.
7. Submit final code to the OJ by yourself.
8. If the problem is learning-log required, complete `submission.md` and `ai_reflection.md`.

For beginner PSCP work, the Codex app may be more powerful than necessary.

Use it carefully.

---

## 27. Quick Self-Check

This checklist is only for self-checking.

Students do not need to submit this checklist.

Before submitting to the OJ, make sure that:

```text
[ ] I used VS Code to write, run, and test my code.
[ ] I wrote my own problem understanding before using Codex.
[ ] I wrote my own first plan before using Codex.
[ ] I used the course AGENTS.md file.
[ ] I used Codex as a coach, reviewer, debugger, or test-case helper.
[ ] I reviewed any Codex-generated code or edits.
[ ] I tested at least 3 different cases by myself.
[ ] I understand my final code.
[ ] I can explain what Codex helped with.
```

If the problem is learning-log required, complete:

```text
submission.md
ai_reflection.md
```

---

## 28. Final Reminder

Codex is powerful because it can work with code and commands.

This also makes it risky if used carelessly.

Use Codex to learn, review, debug, and test.

Do not use Codex to replace your own problem solving.

Your final OJ submission is your responsibility.
