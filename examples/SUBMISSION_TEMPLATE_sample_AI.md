# Problem Solving Submission

This is a sample file. Do not copy this content into your own submission.

Use it only to understand the expected level of detail.

This sample shows a problem with multi-line input/output where AI was used.

Because AI was used, the student must also complete `ai_reflection.md`.

---

## 1. OJ Information

OJ problem number/title:

```text
OJ002 - Sum of Numbers
```

OJ submission ID, if submitted:

```text
128611
```

OJ status:

```text
Pass
```

Independent time spent on this problem:

```text
30-60 minutes
```

Choose one:

```text
0-15 minutes
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

How to count this time:

- Count only the time you actively worked on this problem independently.
- Start counting from when you first read the problem.
- Do not include breaks, meals, classes, sleep, time spent on other problems, or time when you were not working on this problem.
- If you used AI, count only the independent time before your first AI prompt.
- If you asked a friend, TA, or instructor for help, count only the independent time before your first help request.
- If you used both AI and human help, count only the independent time before the first outside help of any kind.
- If you did not use AI or human help, count the time before writing this `submission.md`.
- An estimate is acceptable, but it must be honest.

---

## 2. My Understanding

Write the problem in your own words.

Also explain the input, output, and important constraints.

If you do not fully understand the problem yet, write what you currently understand. Your understanding may be incomplete or incorrect, but you must make a genuine attempt.

```text
The problem asks me to read n numbers and print their total sum.

Input:
The first line contains an integer n.
The next line contains n integers.

Output:
Print one integer, which is the sum of all n numbers.

Constraints:
I think n can be more than 1, so I should not write code for only one number. The numbers may include 0 or negative values, so the sum may decrease.
```

---

## 3. My First Plan

Write your first plan before getting help from AI, a friend, a TA, an instructor, or before finalizing your code.

If you used AI, write the plan you had before your first AI prompt.

If you asked a friend, TA, or instructor for help, write the plan you had before asking for help.

If you did not use AI or human help, write the plan you had before or while you started coding.

This can be rough. It may be incomplete or different from your final solution.

You may write pseudocode, a flowchart idea, or step-by-step thinking.

```text
Step 1: Read n
Step 2: Read numbers
Step 3: Use a loop to add each number to total
Step 4: Print total

At first, I was not sure whether the n numbers are always on one line or may be split across multiple lines.
```

---

## 4. My Final Approach

Briefly explain the final algorithm or method you actually used in your submitted code.

This section is different from Section 3:

- Section 3 is your first plan before AI, human help, or before the final code.
- Section 4 is the final method used in your actual solution.
- If your final approach is the same as your first plan, write that it is the same and briefly explain why.

Do not copy AI's explanation.

Do not copy another person's explanation.

```text
My final solution reads n first, then reads integers until it has n values. I used a running total variable and added each value one by one. This is close to my first plan, but I adjusted the input reading to handle the case where numbers may appear across multiple lines.
```

---

## 5. My Tests

Write at least 3 test cases that you tried or designed by yourself.

Try to choose test cases that are different from each other.

For each test case, explain why you chose it.

If the input or output has many lines, write them inside the text blocks.

### Test Case 1

Why I chose this case:

```text
This is a normal case with positive numbers.
```

Input:

```text
5
1 2 3 4 5
```

Expected output:

```text
15
```

Actual output:

```text
15
```

Result:

```text
Pass
```

### Test Case 2

Why I chose this case:

```text
This checks whether the program works when some numbers are negative.
```

Input:

```text
4
10 -3 2 -5
```

Expected output:

```text
4
```

Actual output:

```text
4
```

Result:

```text
Pass
```

### Test Case 3

Why I chose this case:

```text
This checks whether my code works when the numbers are written on multiple lines.
```

Input:

```text
6
1 2
3 4
5 6
```

Expected output:

```text
21
```

Actual output:

```text
21
```

Result:

```text
Pass
```

---

## 6. AI Use

Did you use AI for this problem?

```text
Yes
```

If yes, also complete:

```text
ai_reflection.md
```

If you only asked a friend, TA, or instructor and did not use AI, you do not need to complete `ai_reflection.md`.

---

## 7. Human Help / Collaboration

Did you ask a friend, TA, instructor, or another person for help on this problem?

```text
No
```

If yes, briefly explain what kind of help you received.

Allowed examples:

- explanation of the problem statement
- explanation of a programming concept
- hint about the approach
- debugging discussion
- test-case discussion
- help understanding an error message

Not allowed:

- copying another person's code
- submitting another person's solution
- asking another person to write the solution for you
- using another person's OJ submission
- asking another person to submit to the OJ for you

Who helped you?

```text
No one.
```

What did they help with?

```text
No human help was used.
```

What did you still do by yourself?

```text
I wrote my own first plan, wrote and tested the final code in VS Code, designed my own test cases, and submitted to the OJ by myself.
```

Did you copy any code from another person?

```text
No
```

---

## 8. Student Declaration

Write `Yes` for each statement.

| Statement | Yes/No |
|---|---|
| I wrote this submission in my own words. | Yes |
| I understand my final code. | Yes |
| I recorded the real OJ status. | Yes |
| I did not copy AI-generated text directly into this file. | Yes |
| I did not copy code from another person. | Yes |
| If I received human help, I disclosed it in this file. | Yes |
| I submitted the final code to the OJ by myself. | Yes |
