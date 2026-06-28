# Problem Solving Submission

This is a sample file. Do not copy this content into your own submission.

Use it only to understand the expected level of detail.

This sample shows a simple problem where AI was not used.

---

## 1. OJ Information

OJ problem number/title:

```text
OJ001 - Even or Odd
```

OJ submission ID, if submitted:

```text
128450
```

OJ status:

```text
Pass
```

Independent time spent on this problem:

```text
15-30 minutes
```

Choose one:

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

How to count this time:

- Count only the time you actively worked on this problem.
- Start counting from when you first read the problem.
- Do not include breaks, meals, classes, sleep, time spent on other problems, or time when you were not working on this problem.
- If you used AI, count only the time before your first AI prompt.
- If you did not use AI, count the time before writing this `submission.md`.
- An estimate is acceptable, but it must be honest.

---

## 2. My Understanding

Write the problem in your own words.

Also explain the input, output, and important constraints.

If you do not fully understand the problem yet, write what you currently understand. Your understanding may be incomplete or incorrect, but you must make a genuine attempt.

```text
The problem asks me to read one integer and decide whether it is even or odd.

Input:
The program receives one integer n.

Output:
The program should print "Even" if n is divisible by 2. Otherwise, it should print "Odd".

Constraints:
The input is an integer. I should also consider 0 and negative numbers because modulo still works with them in Python.
```

---

## 3. My First Plan

Write your first plan before getting help from AI or before finalizing your code.

If you used AI, write the plan you had before your first AI prompt.

If you did not use AI, write the plan you had before or while you started coding.

This can be rough. It may be incomplete or different from your final solution.

You may write pseudocode, a flowchart idea, or step-by-step thinking.

```text
Step 1: Read integer n
Step 2: Check whether n % 2 == 0
Step 3: If true, print "Even"
Step 4: Otherwise, print "Odd"
```

---

## 4. My Final Approach

Briefly explain the final algorithm or method you actually used in your submitted code.

This section is different from Section 3:

- Section 3 is your first plan before AI or before the final code.
- Section 4 is the final method used in your actual solution.
- If your final approach is the same as your first plan, write that it is the same and briefly explain why.

Do not copy AI's explanation.

```text
My final approach is the same as my first plan. I used the modulo operator to check the remainder when n is divided by 2. If the remainder is 0, the number is even. Otherwise, it is odd.
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
This is a normal positive even number.
```

Input:

```text
4
```

Expected output:

```text
Even
```

Actual output:

```text
Even
```

Result:

```text
Pass
```

### Test Case 2

Why I chose this case:

```text
This checks zero because zero is a special value but should still be even.
```

Input:

```text
0
```

Expected output:

```text
Even
```

Actual output:

```text
Even
```

Result:

```text
Pass
```

### Test Case 3

Why I chose this case:

```text
This checks a negative odd number.
```

Input:

```text
-3
```

Expected output:

```text
Odd
```

Actual output:

```text
Odd
```

Result:

```text
Pass
```

---

## 6. AI Use

Did you use AI for this problem?

```text
No
```

If yes, also complete:

```text
ai_reflection.md
```

---

## 7. Student Declaration

Write `Yes` for each statement.

| Statement | Yes/No |
|---|---|
| I wrote this submission in my own words. | Yes |
| I understand my final code. | Yes |
| I recorded the real OJ status. | Yes |
| I did not copy AI-generated text directly into this file. | Yes |
