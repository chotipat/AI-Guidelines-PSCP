# Student Workflow for Web Chat AI Tools

This file explains how students should use web-based AI chat tools responsibly in this course.

Use this workflow if you use AI through a browser or chat interface, such as:

- ChatGPT
- Claude
- Gemini
- other web-based AI chat tools

This workflow applies to both free and paid accounts if the tool is used mainly as a chat assistant.

This workflow does not cover AI coding tools that work inside VS Code, an IDE, a terminal, CLI, or coding-agent environment.

For Codex, follow `workflows/STUDENT_WORKFLOW_CHATGPT_CODEX.md`. For Claude Code, follow `workflows/STUDENT_WORKFLOW_CLAUDE_CODE.md`. Other AI coding tools are not part of the course workflow unless the instructor announces a separate workflow.

---

## 1. Main Rule

AI may be used as a learning assistant, but it must not replace your own thinking.

Before asking AI, you must first try to understand the problem by yourself.

AI may help you:

- understand a problem,
- review your first plan,
- find possible bugs,
- suggest test cases,
- explain Python concepts,
- improve grammar or clarity after you have written your own work.

AI must not be used to submit work that you do not understand.

You are responsible for your final code, OJ submission, test cases, and explanation.

---

## 2. What Counts as Web Chat AI?

Web Chat AI means an AI tool that you use mainly by typing messages in a browser or chat window.

Examples:

- ChatGPT in a browser
- Claude in a browser
- Gemini in a browser
- other similar chat-based AI tools

In this workflow, the student must copy and paste information into the chat by themselves.

The AI does not directly read your VS Code project, edit your files, run terminal commands, or submit to the OJ.

If the AI tool can directly read files, edit code, run commands, or work inside your coding environment, it is not covered by this workflow.

---

## 3. Important Limitation of Web Chat AI

Web Chat AI cannot see your OJ, VS Code, GitHub repository, or local files unless you copy and paste information into the chat.

AI may misunderstand the problem or give incorrect code.

Therefore, you must always check AI suggestions by yourself.

Before using AI suggestions, compare them with:

- the OJ problem statement,
- your own understanding,
- your local test results,
- the OJ result.

---

## 4. Files You Should Know

Before using AI, read these files:

| File | Purpose |
|---|---|
| `README.md` | Main course policy and submission rules |
| `instructions/COURSE_AI_INSTRUCTIONS.md` | Instructions to paste into AI so it acts as a coach |
| `templates/SUBMISSION_TEMPLATE.md` | Blank template for `submission.md` |
| `templates/AI_REFLECTION_TEMPLATE.md` | Blank template for `ai_reflection.md` |
| `examples/SUBMISSION_TEMPLATE_sample_no_AI.md` | Example submission when AI was not used |
| `examples/SUBMISSION_TEMPLATE_sample_AI.md` | Example submission when AI was used |
| `examples/AI_REFLECTION_TEMPLATE_sample.md` | Example AI reflection |

---

## 5. Check Whether the OJ Problem Is Learning-Log Required

For every assigned OJ problem, first check whether the problem is marked as learning-log required by the instructor or in the OJ.

| Case | What to Submit |
|---|---|
| Normal OJ problem | Submit code to the OJ only |
| Learning-log-required OJ problem | Submit code to the OJ and create a GitHub learning log |

If the problem is not learning-log required, you do not need to submit `submission.md` or `ai_reflection.md`, even if you used AI.

However, you must still understand your code and be able to explain your AI use if asked.

---

## 6. Required Steps Before Using Web Chat AI

Use this section every time you use ChatGPT, Claude, Gemini, or another web chat AI tool.

This applies to both normal OJ problems and learning-log-required OJ problems.

### Step 1: Think by Yourself First

Before asking AI, you must first try to understand the problem by yourself.

Write your own notes first, such as:

```text
Problem understanding:
Input:
Output:
Constraints:
First plan:
```

If the problem is learning-log required, write this in `submission.md`.

If the problem is not learning-log required, this may be your private note.

### Step 2: Start a New AI Chat

Start a new AI chat for one OJ problem.

Do not mix many OJ problems in one AI chat.

### Step 3: Paste the Course AI Instructions

Before asking about the OJ problem, paste the content of:

```text
instructions/COURSE_AI_INSTRUCTIONS.md
```

Use a message like this:

```text
Please follow these course AI instructions.

Act as a problem-solving coach, not as a final-answer generator.

[Paste instructions/COURSE_AI_INSTRUCTIONS.md here]
```

### Step 4: Give AI Your Own Attempt

After pasting the course instructions, give AI your own attempt.

Do not only paste the problem and ask for the answer.

Use a prompt like this:

```text
I am solving an OJ problem for my Problem Solving and Computer Programming course.

Please do not give me the full code immediately.

Here is my current understanding:
...

Input:
...

Output:
...

Important constraints:
...

My first plan:
...

Please help me check whether my understanding and plan are reasonable.
```

---

## 7. Workflow for a Normal OJ Problem

Use this workflow when the problem is not learning-log required.

1. Read the OJ problem.
2. Think by yourself first.
3. Code and test in VS Code.
4. If you use Web Chat AI, follow Section 6 first.
5. Submit your final code to the OJ.

For a normal OJ problem, you do not need to submit `submission.md` or `ai_reflection.md`, unless the instructor specifically asks for it.

---

## 8. Workflow for a Learning-Log-Required Problem Without AI

Use this workflow when the problem is learning-log required and you do not use AI.

1. Create a learning log folder, such as `oj2198/`.
2. Copy `templates/SUBMISSION_TEMPLATE.md` and rename it as `submission.md`.
3. Fill in your own problem understanding, first plan, final approach, tests, and OJ information.
4. Code and test in VS Code.
5. Submit to the OJ.
6. Push the learning log folder to GitHub.

The folder should contain:

```text
oj2198/
└── submission.md
```

---

## 9. Workflow for a Learning-Log-Required Problem With AI

Use this workflow when the problem is learning-log required and you use Web Chat AI.

1. Create a learning log folder, such as `oj0301/`.
2. Copy `templates/SUBMISSION_TEMPLATE.md` and rename it as `submission.md`.
3. Before your first AI prompt, fill in at least problem information, independent time spent, current understanding, and first plan.
4. Follow the required AI steps in Section 6.
5. Code and test in VS Code.
6. Submit to the OJ.
7. Complete `submission.md`.
8. Copy `templates/AI_REFLECTION_TEMPLATE.md` and rename it as `ai_reflection.md`.
9. Push the learning log folder to GitHub.

The folder should contain:

```text
oj0301/
├── submission.md
└── ai_reflection.md
```

---

## 10. Good Prompt Examples

Good AI questions usually include your own thinking.

### Understanding the Problem

```text
I do not fully understand this problem yet.

Here is what I currently understand:
...

Please ask me guiding questions and help me clarify the problem.

Do not give the full solution yet.
```

### Reviewing a First Plan

```text
Here is my first plan:

Step 1:
Step 2:
Step 3:

Please review this plan.

Tell me if there is a missing case or a possible problem.

Do not write the full code yet.
```

### Debugging

```text
My code does not pass the OJ.

Here is my code:
...

Here is one test case:

Input:
...

Expected output:
...

My actual output:
...

Please help me find the likely bug.

Explain the reason before suggesting code changes.
```

---

## 11. Bad Prompt Examples

Avoid prompts that ask AI to replace your own work.

Bad examples:

```text
Solve this problem for me.
```

```text
Give me the full accepted code.
```

```text
Write everything for my submission.md.
```

```text
Write my AI reflection for me.
```

```text
Here is the problem. Just give me the answer.
```

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
- course materials that are not allowed to be redistributed.

Your GitHub learning log should contain only your own work:

- `submission.md`,
- `ai_reflection.md`, if AI was used,
- your own test cases,
- OJ submission references,
- your own explanations.

---

## 13. Final Reminder

AI can help you think, debug, and test.

AI cannot replace your own understanding.

Your final OJ submission is your responsibility.
