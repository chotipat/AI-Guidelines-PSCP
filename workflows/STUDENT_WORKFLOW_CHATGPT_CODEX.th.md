# Student Workflow for ChatGPT Codex / OpenAI Codex / Codex CLI

ไฟล์นี้อธิบายวิธีใช้ Codex อย่างรับผิดชอบในรายวิชานี้

Workflow ที่แนะนำคือ:

    VS Code + Codex CLI

---

## 1. Codex คืออะไร

Codex เป็น AI coding agent ที่สามารถช่วยอ่าน code, review, debug, เสนอ patch หรือช่วยรันคำสั่งได้ ขึ้นอยู่กับ interface ที่ใช้

เพราะ Codex อาจทำงานกับไฟล์และคำสั่งได้ จึงต้องใช้ด้วยความระมัดระวัง

---

## 2. VS Code ยังคงเป็น Editor ทางการ

นักศึกษาต้องใช้ VS Code สำหรับ:

- เขียน code
- รัน code
- ทดสอบ code
- เตรียม final code ก่อนส่ง OJ

Codex เป็นเพียงผู้ช่วย

---

## 3. เตรียม Folder

สร้าง folder หลัก:

    pscp/

copy ไฟล์:

    instructions/AGENTS.md

ไปเป็น:

    pscp/AGENTS.md

โครงสร้างที่แนะนำ:

    pscp/
    ├── AGENTS.md
    ├── oj001_work/
    │   └── main.py
    └── oj002_work/
        └── main.py

ให้เปิด folder `pscp` ใน VS Code

---

## 4. ก่อนใช้ Codex

ต้องมีความพยายามของตนเองก่อน เช่น:

    Problem understanding:
    Input:
    Output:
    Constraints:
    First plan:

ห้ามเริ่มด้วยการให้ Codex solve ทั้งข้อ

---

## 5. Prompt เริ่มต้นที่ดี

    I am solving an OJ problem for my PSCP course.

    Follow AGENTS.md.

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

---

## 6. การให้ Codex Review Code

    Please review oj002_work/main.py.

    Do not rewrite the whole file.

    First explain what my code is trying to do.
    Then point out one possible bug or missing case.

    Do not edit the file yet.
    Do not run commands yet.

---

## 7. การให้ Codex Debug

    My code fails this test case.

    Input:
    ...

    Expected output:
    ...

    Actual output:
    ...

    Please explain the likely bug first.
    Suggest the smallest change only.
    Do not rewrite the whole file.

---

## 8. การให้ Codex แก้ไฟล์

ก่อนแก้ให้ถาม:

    Explain what you plan to change before editing the file.

ถ้าเห็นสมควร ให้สั่ง:

    Apply only the smallest necessary change.
    Do not rewrite unrelated code.
    After editing, explain what changed and why.

---

## 9. สิ่งที่ห้ามทำ

ห้ามใช้ Codex เพื่อ:

- เขียน accepted code เต็มจากศูนย์
- rewrite ทั้งไฟล์โดยไม่จำเป็น
- ส่ง OJ แทน
- เขียน `submission.md` หรือ `ai_reflection.md` แทน
- สร้าง fake test results หรือ fake OJ results

---

## 10. หลังใช้ Codex

นักศึกษาต้อง:

1. อ่าน code ที่เปลี่ยน
2. เข้าใจทุกบรรทัด
3. รันทดสอบใน VS Code
4. ส่ง OJ ด้วยตนเอง
5. เขียน reflection เองถ้าโจทย์ต้องส่ง learning log และใช้ AI

---

## 11. สรุป

ใช้ Codex เพื่อเรียนรู้ review debug และ test

อย่าใช้ Codex แทนการแก้ปัญหาของตนเอง
