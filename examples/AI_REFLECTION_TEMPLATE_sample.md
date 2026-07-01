# AI Reflection

This is a sample file. Do not copy this content into your own reflection.

Use it only to understand the expected level of detail.

---

## 1. OJ Information

OJ problem number/title:

```text
OJ2198 - Sum of Numbers
```

OJ submission ID, if submitted:

```text
128611
```

OJ status:

```text
Pass
```

---

## 2. AI Tool Used

Which AI tool did you use?

Example: ChatGPT, Claude, Gemini web chat, Claude Code, Codex, or another approved tool.

```text
ChatGPT
```

---

## 3. What I Asked AI to Help With

Briefly describe what you asked AI to help with.

Do not paste the full chat log.

Examples:

- I asked AI to explain the problem statement.
- I asked AI to review my first plan.
- I asked AI to help find a bug in my code.
- I asked AI to suggest test cases.
- I asked AI to explain why my OJ result was wrong.

```text
I asked AI to review my first plan for reading n numbers and calculating their sum. I also asked whether my input-reading method would work if the numbers were split across multiple lines.
```

---

## 4. What AI Helped Me Notice

Explain the useful idea, mistake, bug, edge case, or concept that AI helped you notice.

```text
AI helped me notice that if I use input().split() only once, my code may fail when the n numbers are written across multiple lines. AI suggested that I should keep reading numbers until I have collected n values.
```

---

## 5. What I Checked or Changed by Myself

Explain what you verified, tested, fixed, or decided by yourself before submitting to the OJ.

Examples:

- I tested additional cases in VS Code.
- I checked the input/output format.
- I compared AI's suggestion with the OJ problem statement.
- I changed my code after understanding the bug.
- I rejected part of AI's suggestion because it did not match the problem.

```text
I checked the OJ problem statement again and confirmed that the input may contain numbers on more than one line. I changed my code to keep reading until it had n integers. Then I tested a normal case, a case with negative numbers, and a case where the numbers were split across several lines.
```

---

## 6. What I Learned

Write 2-4 sentences about what you learned from this problem and from using AI.

Focus on your own learning, not only the final answer.

```text
I learned that input format is important and that numbers may not always appear on one line. I also learned that I should test cases that are different from the sample input. AI was useful for pointing out a possible input-reading bug, but I still had to verify it with my own tests.
```

---

## 7. Student Declaration

Write `Yes` for each statement.

| Statement | Yes/No |
|---|---|
| I wrote this reflection in my own words. | Yes |
| This reflection describes my real AI use. | Yes |
| I checked AI's suggestions before using them. | Yes |
| I can explain my final code. | Yes |
