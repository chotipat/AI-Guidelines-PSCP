# Student Workflow for Web Chat AI Tools

This file explains how students should use web-based AI chat tools responsibly in this course.

Use this workflow if you use AI through a browser or chat interface, such as:

- ChatGPT
- Claude
- Gemini
- other web-based AI chat tools

This workflow applies to both free and paid accounts if the tool is used mainly as a chat assistant.

This workflow does not cover AI coding tools that work inside VS Code, an IDE, a terminal, CLI, or coding-agent environment.

Examples not covered in this file:

- Claude Code
- Claude Cowork
- Gemini CLI
- Cursor
- GitHub Copilot
- VS Code AI extensions
- AI coding agents
- terminal-based AI tools

For those tools, follow the coding-tool workflow specified by the instructor.

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
| `COURSE_AI_INSTRUCTIONS.md` | Instructions to paste into AI so it acts as a coach |
| `SUBMISSION_TEMPLATE.md` | Blank template for `submission.md` |
| `SUBMISSION_TEMPLATE_sample_no_AI.md` | Example submission when AI was not used |
| `SUBMISSION_TEMPLATE_sample_AI.md` | Example submission when AI was used |
| `AI_REFLECTION_TEMPLATE.md` | Blank template for `ai_reflection.md` |
| `AI_REFLECTION_TEMPLATE_sample.md` | Example AI reflection |

---

## 5. Check Whether the OJ Problem Is Learning-Log Required

For every assigned OJ problem, first check whether the problem is marked as learning-log required by the instructor or in the OJ.

There are two cases:

| Case | What to Submit |
|---|---|
| Normal OJ problem | Submit code to the OJ only |
| Learning-log-required OJ problem | Submit code to the OJ and create a GitHub learning log |

If the problem is not learning-log required, you do not need to submit `submission.md` or `ai_reflection.md`, even if you used AI.

However, you must still understand your code and be able to explain your AI use if asked.

---

## 6. Required Steps Before Using Web Chat AI

Use this section every time you use ChatGPT, Claude, Gemini, or another web chat AI tool.

This applies to both:

- normal OJ problems,
- learning-log-required OJ problems.

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

If you do not fully understand the problem yet, still write what you currently understand.

Your understanding may be incomplete or incorrect, but you must make a genuine attempt before using AI.

### Step 2: Start a New AI Chat

Start a new AI chat for one OJ problem.

Do not mix many OJ problems in one AI chat.

### Step 3: Paste `COURSE_AI_INSTRUCTIONS.md`

Before asking about the OJ problem, paste the content of `COURSE_AI_INSTRUCTIONS.md` into the chat.

Use a message like this:

```text
Please follow these course AI instructions.

Act as a problem-solving coach, not as a final-answer generator.

[Paste COURSE_AI_INSTRUCTIONS.md here]
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

### Step 5: Use AI as a Coach

Use AI to guide your thinking, not to replace your work.

Good uses of AI:

```text
Please explain the problem in simpler words.
```

```text
Please review my first plan and ask me questions if something is unclear.
```

```text
Please suggest useful test cases. Do not solve the whole problem for me.
```

```text
Please help me find the bug in my code. Explain the bug first.
```

```text
Please explain this Python concept using a small example.
```

Avoid prompts like:

```text
Solve this problem for me.
```

```text
Give me the full accepted code.
```

```text
Write my submission.md for me.
```

```text
Write my ai_reflection.md for me.
```

---

## 7. Workflow for a Normal OJ Problem

Use this workflow when the problem is not learning-log required.

### Step 1: Read the OJ Problem

Read the problem statement carefully in the course OJ.

Do not ask AI immediately.

### Step 2: Think by Yourself First

Try to understand the problem and make your first plan.

You may write a private note such as:

```text
Problem understanding:
Input:
Output:
Constraints:
First plan:
```

This note does not need to be submitted unless the instructor asks for it later.

### Step 3: Code and Test in VS Code

Write your Python code in VS Code.

Run your code locally before submitting.

### Step 4: If You Use AI, Follow Section 6 First

If you decide to use Web Chat AI, you must follow Section 6 first.

This means you must:

1. start a new AI chat,
2. paste `COURSE_AI_INSTRUCTIONS.md`,
3. provide your own understanding and first plan,
4. use AI as a coach, not as a final-answer generator.

### Step 5: Submit to the OJ

Submit your final code to the course OJ.

Even if AI helped you, you must understand the final code and be able to explain it when asked.

For a normal OJ problem, you do not need to submit `submission.md` or `ai_reflection.md`, unless the instructor specifically asks for it.

---

## 8. Workflow for a Learning-Log-Required Problem Without AI

Use this workflow when the problem is learning-log required and you do not use AI.

### Step 1: Create a Learning Log Folder

Create one folder in your GitHub learning log repository.

Use this naming format:

```text
oj001
oj002
oj003
```

Use the number assigned by the instructor or the OJ.

### Step 2: Create `submission.md`

Copy `SUBMISSION_TEMPLATE.md` into the folder and rename it as:

```text
submission.md
```

### Step 3: Fill in Your Own Thinking

Write your own:

- problem understanding,
- input, output, and constraints,
- first plan,
- final approach,
- test cases,
- OJ information.

If you do not fully understand the problem at first, still write what you currently understand.

Your first understanding may be incomplete or incorrect, but you must make a genuine attempt.

### Step 4: Code and Test in VS Code

Write your code in VS Code.

Test at least 3 different test cases that you designed by yourself.

Try to choose test cases that are different from each other.

For each test case, record:

- why you chose the case,
- input,
- expected output,
- actual output,
- pass or not pass.

### Step 5: Submit to the OJ

Submit the code to the OJ.

Record the OJ submission ID and OJ status in `submission.md`.

### Step 6: Complete `submission.md`

Finish all sections in `submission.md`.

Do not paste full code into `submission.md`.

Use the OJ submission ID instead.

### Step 7: Push to GitHub

Push the learning log folder to your GitHub repository.

For a learning-log-required problem without AI, the folder should contain:

```text
oj001/
└── submission.md
```

---

## 9. Workflow for a Learning-Log-Required Problem With AI

Use this workflow when the problem is learning-log required and you use Web Chat AI.

### Step 1: Create a Learning Log Folder

Create one folder in your GitHub learning log repository.

Example:

```text
oj002
```

### Step 2: Create `submission.md` Before Using AI

Copy `SUBMISSION_TEMPLATE.md` into the folder and rename it as:

```text
submission.md
```

Before your first AI prompt, fill in at least:

- OJ problem number/title,
- independent time spent on this problem,
- your current problem understanding,
- your first plan.

Your first plan does not need to be perfect.

It should show what you understood before using AI.

### Step 3: Follow the Required AI Steps in Section 6

Before asking AI about the problem, follow Section 6.

This means you must:

1. start a new AI chat for this problem,
2. paste `COURSE_AI_INSTRUCTIONS.md`,
3. provide your own understanding and first plan,
4. ask AI to act as a coach, not as a final-answer generator.

### Step 4: Code and Test in VS Code

Write or revise your code in VS Code.

Do not submit code that you cannot explain.

If AI gives code, you must understand it before using it.

You should be able to explain:

- what each important part does,
- why the algorithm works,
- how input is read,
- how output is produced,
- what cases you tested.

### Step 5: Test Your Code

Test your code in VS Code before submitting to the OJ.

Use at least 3 test cases that you designed or selected by yourself.

Try to choose cases that are different from each other.

For each test case, record:

- why you chose the case,
- input,
- expected output,
- actual output,
- pass or not pass.

### Step 6: Submit to the OJ

Submit your final code to the course OJ.

Record the OJ submission ID and OJ status in `submission.md`.

### Step 7: Complete `submission.md`

Finish all sections in `submission.md`.

Do not paste full code into `submission.md`.

Use the OJ submission ID instead.

### Step 8: Complete `ai_reflection.md`

Because AI was used, copy `AI_REFLECTION_TEMPLATE.md` into the same folder and rename it as:

```text
ai_reflection.md
```

Write your reflection in your own words.

Do not paste the full AI conversation.

Do not ask AI to write the reflection for you.

Your reflection should explain:

- OJ problem number/title,
- OJ submission ID,
- OJ status,
- which AI tool you used,
- what you asked AI to help with,
- what AI helped you notice,
- what you checked or changed by yourself,
- what you learned.

### Step 9: Push to GitHub

Push the learning log folder to your GitHub repository.

For a learning-log-required problem with AI, the folder should contain:

```text
oj002/
├── submission.md
└── ai_reflection.md
```

---

## 10. Good Prompt Examples

Good AI questions usually include your own thinking.

### Example 1: Understanding the Problem

```text
I do not fully understand this problem yet.

Here is what I currently understand:
...

Here is what I think the input means:
...

Here is what I think the output should be:
...

Please ask me guiding questions and help me clarify the problem.

Do not give the full solution yet.
```

### Example 2: Reviewing a First Plan

```text
Here is my first plan:

Step 1:
Step 2:
Step 3:

Please review this plan.

Tell me if there is a missing case or a possible problem.

Do not write the full code yet.
```

### Example 3: Debugging

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

### Example 4: Test Case Generation

```text
Please suggest test cases for this problem.

Do not solve the problem for me.

For each test case, explain why it is useful.
```

### Example 5: Python Concept Explanation

```text
Please explain this Python concept using a small example.

Do not solve the whole OJ problem for me.
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

```text
Make the code pass the OJ without explaining it.
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

## 13. Final Checklist Before Submitting a Learning Log

Before pushing your learning log to GitHub, check:

```text
[ ] I submitted my code to the OJ, or I recorded Not Submit honestly.
[ ] I recorded the correct OJ submission ID, if submitted.
[ ] I recorded the real OJ status.
[ ] I wrote submission.md in my own words.
[ ] I included at least 3 test cases that I thought about.
[ ] If I used AI, I also wrote ai_reflection.md.
[ ] I did not copy the sample template content as my own work.
[ ] I did not include full source code in GitHub.
[ ] I did not include official OJ problem statements.
[ ] I can explain my final code if asked.
```

---

## 14. Final Reminder

AI can help you think, debug, and test.

AI cannot replace your own understanding.

Your final OJ submission is your responsibility.
