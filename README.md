# AI Guidelines for PSCP

This repository provides guidelines and templates for using AI responsibly in the Problem Solving and Computer Programming course at IT KMITL.

This repository does not contain OJ problems, official solutions, hidden test cases, or course-restricted materials.

Students must use VS Code for coding and submit final code to the course OJ.

---

## 1. Purpose of This Repository

This repository explains how students should use AI tools in this course.

AI may be used as:

- a problem-solving coach
- a pseudocode or flowchart reviewer
- a debugging assistant
- a test-case generator
- a reflection helper

AI must not be used as a replacement for the student's own thinking.

The main goal is to help students develop problem-solving and programming skills, not only to obtain accepted answers from the OJ.

---

## 2. Files in This Repository

| File | Purpose |
|---|---|
| `COURSE_AI_INSTRUCTIONS.md` | Main AI coach instructions for ChatGPT, Claude, and Gemini |
| `STUDENT_WORKFLOW_FREE.md` | Detailed workflow for students using free AI plans |
| `STUDENT_WORKFLOW_SUBSCRIPTION.md` | Detailed workflow for students using ChatGPT Plus, Claude Pro, Gemini Pro, Claude Code, Gemini CLI, or similar tools |
| `SUBMISSION_TEMPLATE.md` | Template for `submission.md`, required for every learning log |
| `AI_REFLECTION_TEMPLATE.md` | Template for `ai_reflection.md`, required when AI was used |

Read this `README.md` first.

Then read the workflow file that matches your AI plan:

- Free plan: read `STUDENT_WORKFLOW_FREE.md`
- Subscription plan or AI coding tool: read `STUDENT_WORKFLOW_SUBSCRIPTION.md`

---

## 3. What Students Must Write by Themselves

The following parts must be written by the student. AI may review, ask questions, or give suggestions, but AI must not write these parts for submission.

Students must write by themselves:

1. their own problem understanding,
2. input, output, and constraint analysis,
3. initial pseudocode or flowchart idea,
4. explanation of their own algorithm,
5. final submitted code to the OJ that they understand and can explain,
6. their own test cases and test results,
7. their own `submission.md`, when required,
8. their own `ai_reflection.md`, when AI was used.

Students are not allowed to submit:

- AI-generated code that they cannot explain,
- AI-generated problem analysis copied directly without revision,
- AI-generated reflection that does not describe their real process,
- AI-generated pseudocode copied without understanding,
- fake AI reflection,
- fake testing results,
- fake OJ results.

Students do not need to submit the full AI conversation.

However, when interacting with AI, students must write their own questions, explain the problem in their own words, provide their own pseudocode or algorithm idea, and verify AI suggestions by themselves.

The student is responsible for the final answer, final code, OJ submission, and explanation.

---

## 4. What Is a Learning Log?

A learning log is a GitHub folder for one OJ problem.

It records the student's problem-solving process and, if AI was used, the student's AI reflection.

A learning log may contain:

| File | Meaning |
|---|---|
| `submission.md` | The student's problem-solving record |
| `ai_reflection.md` | The student's reflection on AI use |

Use one folder per OJ problem.

Folder names must follow this format:

```text
oj001
oj002
oj003
...
```

Do not use other folder name formats.

---

## 5. Overall Workflow for Every OJ Problem

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
Edge cases:
Initial pseudocode or flowchart idea:
```

This is not necessarily full code.

Writing code at this step is optional.

The purpose of this step is to show that the student tried to understand and plan the solution before using AI.

If the problem requires a learning log, this initial thinking must be written in `submission.md`.

If the student uses AI, this initial thinking must be written in `submission.md` before asking AI.

### Step 3: Decide Whether to Use AI

If the student does not use AI, continue coding in VS Code.

If the student uses AI, read the workflow file that matches the situation:

- Free plan: `STUDENT_WORKFLOW_FREE.md`
- Subscription plan or AI coding tool: `STUDENT_WORKFLOW_SUBSCRIPTION.md`

### Step 4: Code in VS Code

Write Python code in VS Code.

Use your own pseudocode or flowchart idea as a guide.

### Step 5: Test Locally

Run the code in VS Code before submitting to the OJ.

Check:

- normal cases,
- boundary cases,
- edge cases,
- exact output format.

### Step 6: Submit to the OJ

Submit the final code to the course OJ.

The OJ result is the official result for correctness.

### Step 7: Submit Learning Log Files if Required

Create and push learning log files to your own GitHub repository when required by Section 6.

---

## 6. What Must Be Submitted?

There are two possible submission places:

1. the course OJ,
2. the student's own public GitHub learning log repository.

### 6.1 OJ Submission

For every assigned OJ problem, students must submit final code to the course OJ.

### 6.2 GitHub Learning Log Submission

Students must submit a GitHub learning log in the following cases:

| Situation | GitHub learning log required? | `submission.md` required? | `ai_reflection.md` required? |
|---|---:|---:|---:|
| Normal OJ practice, no AI used, not marked as learning log | No | No | No |
| OJ problem marked as learning log required, no AI used | Yes | Yes | No |
| Any OJ problem where AI was used | Yes | Yes | Yes |

Important rules:

- If AI was used, students must submit both `submission.md` and `ai_reflection.md`.
- `submission.md` is used to show what the student understood, tried, tested, and submitted.
- `ai_reflection.md` is used to explain how AI was used and what the student verified independently.
- If no AI was used and the problem is not marked as learning log required, students only submit to the OJ.

---

## 7. When to Use `SUBMISSION_TEMPLATE.md`

Use `SUBMISSION_TEMPLATE.md` to create a file named:

```text
submission.md
```

`submission.md` is required when:

1. the OJ problem is marked as learning log required, or
2. the student used AI for that problem.

### When to Start `submission.md`

Start `submission.md` before using AI.

If AI is not used, start `submission.md` while solving the problem if the problem is marked as learning log required.

Before using AI, students must fill in at least:

```text
Problem understanding:
Input:
Output:
Constraints:
Edge cases:
Initial pseudocode or flowchart idea:
Time spent before using AI:
```

If the student does not understand the problem yet, they should honestly write what is unclear.

Example:

```text
Problem understanding:
I do not fully understand the problem yet. I think the input may contain ..., but I am not sure about ...

Input:
Not clear yet.

Output:
Not clear yet.

Initial pseudocode or flowchart idea:
I cannot write full pseudocode yet, but I think the first step might be ...
```

### When to Finish `submission.md`

Finish `submission.md` after:

1. coding in VS Code,
2. testing locally,
3. submitting to the OJ, if submitted,
4. knowing the current OJ status.

`submission.md` should include:

- OJ problem number or title,
- OJ submission ID, if submitted,
- OJ status,
- student's problem understanding,
- input, output, and constraints,
- edge cases,
- initial pseudocode or flowchart idea,
- final algorithm explanation,
- local test cases and results,
- time spent before using AI, if AI was used,
- total time spent on the problem before writing this submission.

### OJ Status Options

Use one of the following:

```text
Pass
Not Pass
Not Submit
```

Meaning:

- `Pass`: the OJ accepted the solution or all required tests passed.
- `Not Pass`: the solution was submitted but did not pass all required tests.
- `Not Submit`: the student has not submitted to the OJ yet.

If the OJ shows the number of passed test cases, include it.

Example:

```text
OJ status: Not Pass
OJ submission ID: 184401
Passed test cases: 7
Total test cases: 10
Notes: Wrong answer on hidden cases
```

If the OJ does not show the number of test cases, write:

```text
Passed test cases: not shown by OJ
Total test cases: not shown by OJ
```

### Time Spent Options

Use these options for time spent fields:

```text
15-30 minutes
30-60 minutes
1-3 hours
3-6 hours
6-24 hours
1-3 days
4-7 days
1-4 weeks
More than 4 weeks
```

There is no option below 15 minutes because students are expected to think by themselves for at least 15 minutes before using AI.

### Time Fields

Use these two fields in `submission.md`:

```text
Time spent before using AI:
Total time spent on this problem before writing this submission:
```

If AI was used:

```text
Time spent before using AI: 30-60 minutes
Total time spent on this problem before writing this submission: 1-3 hours
```

If AI was not used:

```text
Time spent before using AI: Not applicable because I did not use AI
Total time spent on this problem before writing this submission: 1-3 hours
```

### Code in `submission.md`

Do not copy the full code into `submission.md`.

Use the OJ submission ID instead.

The submitted code should be checked in the OJ.

### Academic Integrity for `submission.md`

`submission.md` must be written by the student in their own words.

Do not ask AI to write `submission.md` for you.

AI may help review clarity or grammar after the student has written the content, but AI must not generate the content for the student.

---

## 8. When to Use `AI_REFLECTION_TEMPLATE.md`

Use `AI_REFLECTION_TEMPLATE.md` to create a file named:

```text
ai_reflection.md
```

`ai_reflection.md` is required only when AI was used for that problem.

If AI was used, `submission.md` is also required.

### When to Start `ai_reflection.md`

Start `ai_reflection.md` after the first time you use AI for that problem.

You may take brief notes while working.

### When to Finish `ai_reflection.md`

Finish `ai_reflection.md` after:

1. testing your code in VS Code,
2. submitting to the OJ, if submitted,
3. knowing the current OJ status.

### What `ai_reflection.md` Should Explain

Your `ai_reflection.md` should explain:

1. which AI tool you used,
2. what you asked AI to help with,
3. what AI helped you notice,
4. what you tested or verified by yourself,
5. what you changed before submitting,
6. current OJ status,
7. what you learned.

The reflection must describe your real process.

Do not ask AI to invent the reflection for you.

AI may help with grammar, formatting, or clarity after you write your own reflection.

AI must not:

- invent what happened,
- exaggerate your work,
- claim that you tested something you did not test,
- claim that you understood something you cannot explain,
- write a reflection that does not match your actual process.

---

## 9. Recommended Student GitHub Repository Structure

Each student should create one public GitHub repository for learning log records.

Recommended repository name:

```text
pscp-ai-learning-log
```

Recommended structure:

```text
pscp-ai-learning-log/
├── README.md
├── oj001/
│   ├── submission.md
│   └── ai_reflection.md
├── oj002/
│   └── submission.md
└── oj003/
    ├── submission.md
    └── ai_reflection.md
```

Use one folder per OJ problem.

Folder names must follow this format only:

```text
oj001
oj002
oj003
...
```

The repository should be public so that the instructor can review it easily.

However, students must not include:

- official OJ problem statements,
- official solutions,
- hidden test cases,
- private data,
- access tokens or API keys,
- screenshots containing personal information,
- course materials that are not allowed to be redistributed.

The repository should contain only the student's own problem-solving records, own test cases, own OJ submission references, and own AI reflections.

---

## 10. What to Put in Each OJ Folder

Each OJ folder may contain:

| File | When required | Purpose |
|---|---|---|
| `submission.md` | Required for learning-log-required problems and all AI-used problems | Problem-solving record and OJ submission reference |
| `ai_reflection.md` | Required only if AI was used | Reflection on how AI helped and what the student verified independently |

Do not include `solution.py` in the GitHub learning log.

Use the OJ submission ID in `submission.md` instead.

### Example 1: Learning Log Required, No AI Used

```text
oj001/
└── submission.md
```

### Example 2: AI Used

```text
oj002/
├── submission.md
└── ai_reflection.md
```

### Example 3: No AI Used and No Learning Log Required

No GitHub folder is required.

Only OJ submission is required.

---

## 11. Final Reminder

AI can help you think, debug, and test.

You are still responsible for understanding, writing, testing, and explaining your own solution.
