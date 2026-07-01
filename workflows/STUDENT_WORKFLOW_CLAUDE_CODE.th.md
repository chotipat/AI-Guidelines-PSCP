# Student Workflow for Claude Code

ไฟล์นี้อธิบายวิธีใช้ Claude Code อย่างรับผิดชอบในรายวิชานี้

Workflow ที่แนะนำคือ:

    VS Code + Claude Code CLI

สำหรับเครื่อง Lab ที่ใช้ร่วมกัน ให้แทน `<student-id>` ด้วยเลขประจำตัวนักศึกษาของตนเอง เช่น `pscp-66123456/` และใช้เฉพาะ folder ของตนเองเท่านั้น

---

## 1. Claude Code คืออะไร

Claude Code เป็น AI coding tool จาก Anthropic

ต่างจาก Claude web chat ปกติ

Claude web chat ใช้คุยผ่าน browser หรือ chat window

Claude Code สามารถทำงานกับ code และ project folder ได้มากกว่า เช่น:

- อ่าน code files
- อ่าน project folder
- เสนอ code changes
- แก้ไฟล์
- รันคำสั่ง
- ช่วย debug
- ช่วย review code
- ช่วยคิด test cases

เพราะ Claude Code ทำงานกับไฟล์และคำสั่งได้ จึงต้องใช้ด้วยความระมัดระวัง

---

## 2. Claude Tools ที่นักศึกษาอาจเจอ

| Tool | วิธีใช้ | ควรอ่าน workflow |
|---|---|---|
| Claude web chat | ใช้ Claude ใน browser แบบ chat ปกติ | `workflows/STUDENT_WORKFLOW_WEB_CHAT.md` |
| Claude desktop app | app ที่ download มา อาจมี Claude chat, Claude Code หรือ Claude Cowork ขึ้นกับ account/features | ใช้เฉพาะเมื่อผู้สอนอนุญาต |
| Claude Code CLI | tool ใน terminal เริ่มด้วยคำสั่ง `claude` | ไฟล์นี้ |

Workflow ที่แนะนำคือ:

    VS Code + Claude Code CLI

---

## 3. VS Code ยังคงเป็น Editor ทางการ

นักศึกษาต้องใช้ VS Code เพื่อเขียน รัน และทดสอบ Python code

Claude Code เป็นเพียงผู้ช่วย ไม่ใช่ editor ทางการ และไม่ใช่ที่ส่งคำตอบ

OJ ของรายวิชายังคงเป็นที่ส่ง code อย่างเป็นทางการ

---

## 4. Claude Code ช่วยอะไรได้

Claude Code ช่วยได้ เช่น:

- review first plan
- อธิบาย Python concept
- อธิบาย error message
- หา bug ใน code ที่นักศึกษาเขียนแล้ว
- เสนอ test cases
- ตรวจ input/output logic
- อธิบายว่าทำไม test case fail
- เสนอ small improvement พร้อมเหตุผล

ห้ามใช้ Claude Code เพื่อ:

- แก้โจทย์ทั้งข้อจากศูนย์
- generate accepted code เต็มโดยไม่มีความพยายามของนักศึกษา
- rewrite solution ทั้งหมดโดยไม่เข้าใจ
- ส่ง OJ
- เขียน `submission.md` หรือ `ai_reflection.md` แทน
- สร้าง fake results

---

## 5. ก่อนใช้ Claude Code

อ่านโจทย์เองก่อน และคิดเองก่อน

อย่างน้อยควรเขียน:

    Problem understanding:
    Input:
    Output:
    Constraints:
    First plan:

ถ้าโจทย์เป็น learning-log-required ให้เขียนใน `submission.md`

---

## 6. ติดตั้ง Claude Code CLI

### Windows PowerShell

เปิด Windows PowerShell แล้วรัน:

    irm https://claude.ai/install.ps1 | iex

ตรวจว่าใช้งานได้:

    claude

### macOS, Linux, or WSL

เปิด Terminal แล้วรัน:

    curl -fsSL https://claude.ai/install.sh | bash

ตรวจว่าใช้งานได้:

    claude

ถ้าติดตั้งไม่สำเร็จ อย่าใช้คำสั่งสุ่มจาก internet ให้ถามผู้สอนหรือ TA

---

## 7. เตรียม Project Folder

สร้าง folder หลัก:

    pscp-<student-id>/

โครงสร้างที่แนะนำ:

    pscp-<student-id>/
    ├── AGENTS.md
    ├── CLAUDE.md
    ├── oj2198_work/
    │   └── main.py
    └── oj0301_work/
        └── main.py

---

## 8. เพิ่ม Course Instructions สำหรับ Claude Code

Claude Code อ่าน instruction จาก:

    CLAUDE.md

Repository เตรียมไฟล์ไว้ที่:

    instructions/CLAUDE.md

ไฟล์นี้ import กฎกลางจาก:

    instructions/AGENTS.md

ให้นักศึกษา copy ทั้งสองไฟล์ไปไว้ใน local folder:

    pscp-<student-id>/AGENTS.md
    pscp-<student-id>/CLAUDE.md

`CLAUDE.md` ใช้:

    @AGENTS.md

เพื่อดึงกฎกลางจาก `AGENTS.md`

ให้เริ่ม Claude Code จาก folder `pscp-<student-id>` เสมอ

---

## 9. Prompt เริ่มต้นที่ดี

    I am solving an OJ problem for my PSCP course.

    Follow CLAUDE.md.

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
    Do not run commands yet.

---

## 10. คำสั่งและการแก้ไฟล์

ก่อนอนุญาตให้ Claude Code แก้ไฟล์ ให้ถาม:

    Explain what you plan to change before editing the file.

ถ้าให้แก้ ให้สั่ง:

    Apply only the smallest necessary change.
    Do not rewrite unrelated code.
    After editing, explain what changed and why.

---

## 11. หลังใช้ Claude Code

นักศึกษาต้อง:

1. อ่าน code ที่เปลี่ยน
2. เข้าใจทุกส่วน
3. รันทดสอบใน VS Code
4. ส่ง OJ ด้วยตนเอง
5. เขียน reflection เองถ้าโจทย์ต้องส่ง learning log และใช้ AI

---

## 12. สรุป

Claude Code ช่วยเรียนรู้ review debug และ test ได้

แต่ห้ามใช้แทนการแก้ปัญหาของนักศึกษาเอง
