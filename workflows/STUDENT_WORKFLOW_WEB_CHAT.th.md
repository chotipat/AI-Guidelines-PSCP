# Student Workflow for Web Chat AI Tools

ไฟล์นี้อธิบายวิธีใช้ AI tools ผ่าน browser หรือ chat interface อย่างรับผิดชอบในรายวิชานี้

ตัวอย่างเช่น ChatGPT web chat, Claude web chat, Gemini web chat หรือ AI chat tools อื่นที่ผู้สอนอนุญาต

---

## 1. Web Chat AI คืออะไร

Web chat AI คือเครื่องมือ AI ที่นักศึกษาคุยผ่าน browser หรือ chat window

โดยทั่วไป AI ประเภทนี้ไม่ได้ทำงานโดยตรงใน project folder ของนักศึกษา

นักศึกษาต้อง copy คำถาม code หรือ error ไปถามเอง และต้องนำคำแนะนำกลับมาตรวจสอบเองใน VS Code

---

## 2. กฎหลัก

ก่อนใช้ AI นักศึกษาต้องอ่านโจทย์เองและคิดเองก่อน

อย่างน้อยควรเขียน:

    Problem understanding:
    Input:
    Output:
    Constraints:
    First plan:

ถ้าโจทย์เป็น learning-log-required ให้เขียนใน `submission.md`

ห้ามเริ่มด้วย prompt เช่น:

    Solve this problem.
    Write the full accepted code.

ให้ใช้ AI เป็น coach ไม่ใช่ผู้ทำแทน

---

## 3. Prompt เริ่มต้นที่ดี

    I am solving an OJ problem for my PSCP course.

    Do not write the full solution.

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

---

## 4. การขอ Debug

ให้ถามจาก code ที่ตนเองเขียนแล้ว

    My code fails this test case.

    Input:
    ...

    Expected output:
    ...

    Actual output:
    ...

    Please explain the likely bug first.
    Do not rewrite the whole code.
    Suggest the smallest change only.

---

## 5. การขอ Test Cases

AI สามารถช่วยคิด test cases ได้

    Please suggest 3 useful test cases.
    Do not solve the problem.
    For each test case, explain why it is useful.

นักศึกษาต้องรัน test cases เองใน VS Code

---

## 6. สิ่งที่ห้ามทำ

ห้ามใช้ AI เพื่อ:

- เขียน accepted code เต็มให้ทันที
- ทำโจทย์ทั้งข้อโดยที่นักศึกษาไม่มี first plan
- เขียน `submission.md` แทนนักศึกษา
- เขียน `ai_reflection.md` แทนนักศึกษา
- สร้าง fake test results
- สร้าง fake OJ results

---

## 7. หลังใช้ AI

นักศึกษาต้อง:

1. แก้ code ใน VS Code ด้วยตนเอง
2. รันและทดสอบใน VS Code
3. ส่ง code เข้า OJ ด้วยตนเอง
4. ถ้าโจทย์ต้องส่ง learning log และใช้ AI ให้เขียน `ai_reflection.md`

---

## 8. สรุป

Web chat AI ช่วยอธิบาย ช่วย review และช่วย debug ได้

แต่นักศึกษาต้องคิด เขียน ทดสอบ และอธิบาย final code ด้วยตนเอง
