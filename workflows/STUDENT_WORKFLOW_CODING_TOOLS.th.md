# Student Workflow for AI Coding Tools

ไฟล์นี้เป็น workflow ทั่วไปสำหรับ AI coding tools ที่สามารถอ่านไฟล์ แก้ code หรือรันคำสั่งได้

ใช้ไฟล์นี้เมื่อผู้สอนอนุญาตให้ใช้ coding tool ที่ไม่มี workflow เฉพาะ

---

## 1. AI Coding Tool คืออะไร

AI coding tool คือ AI ที่อาจทำงานกับ coding environment ได้ เช่น:

- อ่าน project folder
- อ่านไฟล์ code
- เสนอ code changes
- แก้ไฟล์
- รันคำสั่งใน terminal
- ช่วย debug จากไฟล์จริง

เครื่องมือประเภทนี้มีความเสี่ยงมากกว่า web chat เพราะสามารถเปลี่ยนไฟล์หรือรันคำสั่งได้

---

## 2. VS Code ยังคงเป็น Editor ทางการ

แม้ใช้ AI coding tool นักศึกษายังต้อง:

- เขียน code ใน VS Code
- รัน code ใน VS Code
- ทดสอบ code ใน VS Code
- ส่ง code เข้า OJ ด้วยตนเอง

AI coding tool เป็นเพียงผู้ช่วย

---

## 3. ก่อนใช้ AI Coding Tool

ต้องมีความพยายามของตนเองก่อน เช่น:

    Problem understanding:
    Input:
    Output:
    Constraints:
    First plan:

ถ้าโจทย์ต้องส่ง learning log ให้เขียนสิ่งนี้ใน `submission.md`

---

## 4. Prompt ที่ควรใช้

    I am solving an OJ problem for my PSCP course.

    Do not write the full solution.

    Review my current plan and code.

    Explain before editing files.
    Ask before running commands.
    Prefer the smallest necessary change.

---

## 5. ก่อนให้ AI แก้ไฟล์

ถามก่อนเสมอ:

    Explain what you plan to change before editing the file.

ถ้าอนุญาตให้แก้ ให้สั่งว่า:

    Apply only the smallest necessary change.
    Do not rewrite unrelated parts of the file.
    After editing, explain what changed and why.

---

## 6. คำสั่งที่ต้องระวัง

ระวังคำสั่งที่:

- ลบไฟล์
- reset Git history
- install packages
- upload files
- expose secrets
- modify folders ที่ไม่เกี่ยวข้อง
- commit หรือ push โดยไม่ได้ตั้งใจ

ถ้าไม่เข้าใจ command ให้ถาม:

    Explain what this command does before running it.

---

## 7. สิ่งที่ห้ามทำ

ห้ามใช้ AI coding tool เพื่อ:

- แก้โจทย์ทั้งข้อจากศูนย์
- เขียน accepted code เต็มทันที
- rewrite ทั้งไฟล์โดยไม่จำเป็น
- ส่ง OJ แทนนักศึกษา
- เขียน `submission.md` หรือ `ai_reflection.md` แทน
- สร้าง fake result

---

## 8. หลังใช้ AI Coding Tool

นักศึกษาต้อง:

1. เปิด code ที่ถูกแก้ใน VS Code
2. อ่านและเข้าใจทุกส่วน
3. รัน test cases เอง
4. ส่ง OJ เอง
5. เขียน reflection เองถ้าโจทย์ต้องส่ง learning log และมีการใช้ AI

---

## 9. สรุป

AI coding tools มีประโยชน์ แต่ต้องควบคุมอย่างระมัดระวัง

ให้นักศึกษาเป็นคนคิดและตัดสินใจขั้นสุดท้ายเสมอ
