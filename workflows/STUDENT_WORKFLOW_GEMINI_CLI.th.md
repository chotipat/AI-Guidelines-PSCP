# Student Workflow for Gemini CLI

ไฟล์นี้อธิบายวิธีใช้ Gemini CLI อย่างรับผิดชอบในรายวิชานี้

Workflow ที่แนะนำคือ:

    VS Code + Gemini CLI

---

## 1. Gemini CLI คืออะไร

Gemini CLI เป็น AI coding agent จาก Google ที่ทำงานใน terminal

ต่างจาก Gemini web chat ปกติ

Gemini web chat ใช้คุยผ่าน browser หรือ chat window

Gemini CLI สามารถทำงานกับ code และ project folder ได้ เช่น:

- อ่าน project files
- อ่าน code files
- เสนอ code changes
- แก้ไฟล์
- รันคำสั่ง
- ใช้ tools เช่น file read, file write, grep และ terminal
- ใช้ MCP servers ถ้ามีการตั้งค่า
- ช่วย debug
- ช่วย review code
- ช่วยคิดหรือปรับ test cases
- ใช้ project context file เช่น `GEMINI.md`

เพราะ Gemini CLI ทำงานกับไฟล์ tools และคำสั่งได้ จึงต้องใช้ด้วยความระมัดระวัง

---

## 2. Gemini Tools ที่นักศึกษาอาจเจอ

| Tool | วิธีใช้ | ควรอ่าน workflow |
|---|---|---|
| Gemini web chat | ใช้ Gemini ใน browser แบบ chat ปกติ | `workflows/STUDENT_WORKFLOW_WEB_CHAT.md` |
| Gemini Code Assist in VS Code | Gemini ใน VS Code; agent mode อาจใช้ Gemini CLI และ tools | ใช้เฉพาะเมื่อผู้สอนอนุญาต |
| Gemini CLI | tool ใน terminal เริ่มด้วยคำสั่ง `gemini` | ไฟล์นี้ |

Gemini Code Assist agent mode ใน VS Code ใช้ได้เฉพาะเมื่อผู้สอนอนุญาตอย่างชัดเจน

---

## 3. VS Code ยังคงเป็น Editor ทางการ

นักศึกษาต้องใช้ VS Code เพื่อ:

- เขียน Python code
- รัน Python code
- ทดสอบ Python code
- เตรียม final code ก่อนส่ง OJ

Gemini CLI เป็นเพียงผู้ช่วย

OJ คือที่ส่ง code อย่างเป็นทางการ

---

## 4. Gemini CLI ช่วยอะไรได้

Gemini CLI ช่วยได้ เช่น:

- review first plan
- อธิบาย Python concept
- อธิบาย error message
- หา bug ใน code ที่นักศึกษาเขียนแล้ว
- เสนอ test cases
- ตรวจ input/output logic
- อธิบายว่าทำไม test case fail
- เสนอ small improvement พร้อมเหตุผล

ห้ามใช้ Gemini CLI เพื่อ:

- แก้โจทย์ทั้งข้อจากศูนย์
- generate accepted code เต็มโดยไม่มีความพยายามของนักศึกษา
- rewrite solution ทั้งหมดโดยไม่เข้าใจ
- ส่ง OJ
- เขียน `submission.md` หรือ `ai_reflection.md` แทน
- สร้าง fake results

---

## 5. ก่อนใช้ Gemini CLI

อ่านโจทย์เองก่อน และคิดเองก่อน

อย่างน้อยควรเขียน:

    Problem understanding:
    Input:
    Output:
    Constraints:
    First plan:

ถ้าโจทย์เป็น learning-log-required ให้เขียนใน `submission.md`

---

## 6. ติดตั้ง Gemini CLI

Gemini CLI ต้องใช้ Node.js 20.0.0 หรือใหม่กว่า

### macOS, Linux, or WSL

เปิด Terminal

ตรวจ Node.js version:

    node --version

ติดตั้ง Gemini CLI:

    npm install -g @google/gemini-cli

ตรวจว่าใช้งานได้:

    gemini

### Windows PowerShell

เปิด Windows PowerShell

ตรวจ Node.js version:

    node --version

ติดตั้ง Gemini CLI:

    npm install -g @google/gemini-cli

ตรวจว่าใช้งานได้:

    gemini

### Optional: ใช้ npx

ถ้าผู้สอนอนุญาต อาจ run โดยไม่ติดตั้งถาวรได้

macOS, Linux, or WSL:

    npx @google/gemini-cli

Windows PowerShell:

    npx @google/gemini-cli

ถ้าติดตั้งไม่สำเร็จ อย่าใช้ package ชื่อคล้าย ๆ กัน ให้ถามผู้สอนหรือ TA

---

## 7. Sign in หรือ Authentication

ครั้งแรกที่รัน:

    gemini

Gemini CLI อาจถามวิธี sign in หรือ authentication

ให้ใช้วิธีที่ผู้สอนกำหนด

ห้ามใส่ API keys, credentials หรือ tokens ใน public GitHub repository

ห้าม commit `.env` ที่มี keys หรือ tokens

---

## 8. เตรียม Project Folder

สร้าง folder หลัก:

    pscp/

โครงสร้างที่แนะนำ:

    pscp/
    ├── AGENTS.md
    ├── GEMINI.md
    ├── oj001_work/
    │   └── main.py
    └── oj002_work/
        └── main.py

---

## 9. เพิ่ม Course Instructions สำหรับ Gemini CLI

Gemini CLI อ่าน project context จาก:

    GEMINI.md

Repository เตรียมไฟล์ไว้ที่:

    instructions/GEMINI.md

ไฟล์นี้ import กฎกลางจาก:

    instructions/AGENTS.md

ให้นักศึกษา copy ทั้งสองไฟล์ไปไว้ใน local folder:

    pscp/AGENTS.md
    pscp/GEMINI.md

`GEMINI.md` ใช้:

    @AGENTS.md

เพื่อดึงกฎกลางจาก `AGENTS.md`

ให้เริ่ม Gemini CLI จาก folder `pscp` เสมอ

---

## 10. Prompt เริ่มต้นที่ดี

    I am solving an OJ problem for my PSCP course.

    Follow GEMINI.md.

    Use VS Code workflow.

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

## 11. คำสั่งและ Auto Modes

Gemini CLI อาจรันคำสั่งและใช้ tools ได้

คำสั่งปลอดภัยทั่วไปคือ:

    python oj002_work/main.py

หรือ:

    python3 oj002_work/main.py

ระวังคำสั่งที่ลบไฟล์ reset Git ติดตั้ง package upload files เปิดเผย secrets หรือแก้ folder ที่ไม่เกี่ยวข้อง

ถ้าไม่เข้าใจ command ให้ถาม:

    Explain what this command does before running it.

### ห้ามใช้ YOLO หรือ Auto-Accept Mode

ห้ามใช้:

    gemini --yolo

ห้ามเปิด auto-accept mode

โหมดเหล่านี้อาจทำให้ Gemini CLI approve tool calls อัตโนมัติ

ในรายวิชานี้ นักศึกษาควรตรวจและอนุมัติ action ด้วยตนเอง

---

## 12. หลังใช้ Gemini CLI

นักศึกษาต้อง:

1. อ่าน code ที่เปลี่ยน
2. เข้าใจทุกส่วน
3. รันทดสอบใน VS Code
4. ส่ง OJ ด้วยตนเอง
5. เขียน reflection เองถ้าโจทย์ต้องส่ง learning log และใช้ AI

---

## 13. สรุป

Gemini CLI ช่วยเรียนรู้ review debug และ test ได้

แต่ห้ามใช้แทนการแก้ปัญหาของนักศึกษาเอง
