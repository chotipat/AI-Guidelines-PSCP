# Shared Lab Computer Usage Policy

This policy applies when students use shared computers in the computer lab for the Problem Solving and Computer Programming course.

Lab computers are shared devices. They may be used by different students at different times.

Students must protect their own accounts, files, AI sessions, and OJ submissions. Students must also respect other students' privacy and work.

---

## 1. Main Principles

When using a shared lab computer, students must:

1. use only their own accounts,
2. use only their own working folder,
3. protect their passwords, tokens, and login sessions,
4. avoid leaving files or accounts open after use,
5. make sure AI tools do not access another student's files,
6. submit only their own work to the OJ,
7. log out and clean up before leaving the computer.

A lab computer is not a personal computer.

Students are responsible for checking that the computer is safe to use before starting and clean before leaving.

---

## 2. Required Working Folder

Students must use a personal working folder.

Recommended folder name:

```text
pscp-<student-id>
```

Replace `<student-id>` with your own student ID.

Do not include the angle brackets `< >` in the actual folder name.

Example:

```text
pscp-66123456
```

For temporary work on an OJ problem, use a problem-specific working folder such as:

```text
pscp-66123456/
├── oj2198_work/
├── oj0301_work/
└── oj1994_work/
```

For learning-log-required problems, use folders based on the OJ problem ID:

```text
pscp-66123456/
├── oj2198/
│   ├── submission.md
│   └── ai_reflection.md
└── oj0301/
    └── submission.md
```

The folder name `oj<problem-id>` must use the 4-digit OJ problem ID.

Examples:

```text
oj2198
oj0301
oj1994
```

Do not use `oj001`, `oj002`, or `oj003` unless those are the actual OJ problem IDs.

---

## 3. Before Using a Lab Computer

Before starting work, students must check:

- no other student's VS Code project is open,
- no other student's terminal session is active,
- no other student's GitHub, OJ, ChatGPT, Claude, Gemini, Codex, or Claude Code account is logged in,
- no file from another student is open in VS Code,
- the current folder is not another student's folder.

Recommended steps:

1. Close old browser tabs.
2. Close old VS Code windows that do not belong to you.
3. Open your own folder only.
4. Use a Private / Incognito browser window when logging in to web services.
5. Check the terminal location before running commands.

Use these commands to check your location:

```bash
pwd
ls
```

Make sure you are inside your own folder, for example:

```text
pscp-66123456/
```

---

## 4. During Lab Work

Students must:

- work only inside their own folder,
- write and test code in VS Code,
- submit final code to the OJ by themselves,
- use their own GitHub account only,
- use their own AI account only,
- keep passwords, tokens, and API keys private,
- check before copying code, error messages, or file contents into AI tools.

Students must not:

- open another student's folder,
- read another student's code,
- copy another student's files,
- edit or delete another student's files,
- submit another student's solution,
- use another student's logged-in account,
- allow AI tools to read folders that may contain another student's files.

---

## 5. Using AI on Shared Lab Computers

AI may be used only under the course AI policy.

On shared lab computers, the safest AI workflow is:

```text
VS Code + web chat in a Private / Incognito browser window
```

Examples of web chat tools:

```text
ChatGPT
Claude
Gemini web chat
```

When using AI web chat, students must:

1. log in with their own account,
2. avoid saving passwords in the browser,
3. avoid choosing "remember me" on shared computers,
4. paste only their own code, error messages, or explanations,
5. avoid uploading folders that may contain other students' files,
6. log out and close the Private / Incognito window after use.

Students must not submit AI-generated code that they cannot explain.

Students must still write, run, test, and submit the final code themselves.

---

## 6. Using Codex or Claude Code on Shared Lab Computers

Codex CLI and Claude Code CLI can read files, edit files, and run commands.

Therefore, they require extra care on shared computers.

Students may use Codex CLI or Claude Code CLI on lab computers only if allowed by the instructor.

Before using Codex or Claude Code, students must check:

```bash
pwd
ls
```

The current directory must be inside the student's own folder, for example:

```text
pscp-66123456/
```

Students must not ask Codex or Claude Code to:

- scan the whole computer,
- inspect another student's folder,
- edit files outside the student's own folder,
- read hidden tokens, passwords, or private files,
- submit to the OJ,
- write `submission.md` or `ai_reflection.md` for the student.

When using Claude Code, students should copy course instruction files into their own folder only:

```text
pscp-66123456/AGENTS.md
pscp-66123456/CLAUDE.md
```

When using Codex, students should copy:

```text
pscp-66123456/AGENTS.md
```

Do not place course AI instruction files in another student's folder.

---

## 7. GitHub, OJ, and Browser Safety

Students must protect their accounts.

Students must not save passwords on lab computers.

Students must log out from:

- OJ,
- GitHub,
- ChatGPT,
- Claude,
- Gemini,
- Codex,
- Claude Code,
- email or any other personal account.

Students should use Private / Incognito mode when possible.

Students must not leave access tokens, API keys, `.env` files, SSH keys, or browser sessions on lab computers.

If a student accidentally leaves an account logged in, they should log out as soon as possible and inform the instructor or TA if needed.

---

## 8. End-of-Session Checklist

Before leaving the lab computer, students must:

1. save their own work,
2. push learning-log files to GitHub if required,
3. submit final code to the OJ if ready,
4. close VS Code,
5. log out of OJ,
6. log out of GitHub,
7. log out of AI tools,
8. close all browser windows,
9. delete temporary files from Desktop, Downloads, and Trash if they are no longer needed,
10. make sure no passwords, tokens, or private files are left behind.

Recommended final check:

```bash
pwd
ls
```

Make sure no personal files are left in a shared location unless the instructor has told students to store files there.

---

## 9. If You Find Another Student's Account or Files

If you find another student's account still logged in:

1. do not use the account,
2. do not read private messages or files,
3. log out if it is clearly safe to do so,
4. inform the instructor or TA.

If you find another student's files:

1. do not open them,
2. do not copy them,
3. do not edit or delete them,
4. inform the instructor or TA if the files may cause confusion.

---

## 10. Academic Integrity

Using a shared lab computer does not change the course rules.

Students are still responsible for:

- writing their own code,
- understanding their final solution,
- submitting to the OJ by themselves,
- writing their own `submission.md`,
- writing their own `ai_reflection.md` if AI was used,
- disclosing meaningful human help when required,
- ensuring that AI tools are used only as allowed by the course policy.

A student must not claim another person's work, AI-generated work, or files left on a shared lab computer as their own.

---

## 11. Short Checklist

Before starting:

```text
Use my own folder.
Use my own accounts.
Check VS Code and terminal location.
Use Private / Incognito for web login.
```

While working:

```text
Use only my files.
Use AI only according to course policy.
Do not let AI read another student's files.
Test code in VS Code.
Submit to OJ by myself.
```

Before leaving:

```text
Save work.
Push learning log if required.
Log out from OJ, GitHub, and AI tools.
Close VS Code and browser.
Remove temporary files.
Do not leave passwords, tokens, or sessions behind.
```
