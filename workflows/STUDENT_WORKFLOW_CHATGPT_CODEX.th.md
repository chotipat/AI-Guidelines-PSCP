# Student Workflow for ChatGPT Codex

ไฟล์นี้อธิบายวิธีที่นักศึกษาควรใช้ ChatGPT Codex / OpenAI Codex / Codex CLI อย่างรับผิดชอบในรายวิชานี้

เอกสารนี้เขียนสำหรับนักศึกษาที่ยังไม่คุ้นเคยกับ Codex

อ่านไฟล์นี้ก่อนใช้ Codex กับโจทย์ OJ ทุกข้อ

สำหรับเครื่อง Lab ที่ใช้ร่วมกัน ให้แทน `<student-id>` ด้วยเลขประจำตัวนักศึกษาของตนเอง เช่น `pscp-66123456/` และใช้เฉพาะ folder ของตนเองเท่านั้น

---

## 1. Codex คืออะไร

Codex เป็น AI coding tool จาก OpenAI

Codex แตกต่างจาก ChatGPT web chat ปกติ

ChatGPT web chat ปกติมักตอบข้อความใน browser

Codex สามารถทำงานกับ code ได้โดยตรงมากกว่า

ขึ้นอยู่กับ version หรือ interface ที่ใช้ Codex อาจสามารถ:

- อ่าน code files
- เสนอการแก้ไข
- แก้ไฟล์
- รันคำสั่ง
- รัน Python code
- ตรวจ project folder
- ช่วย debug code

เพราะ Codex สามารถทำงานกับไฟล์และคำสั่งได้ จึงต้องใช้อย่างระมัดระวัง

---

## 2. ไฟล์นี้ครอบคลุม Codex แบบใด

Workflow นี้ครอบคลุม:

- ChatGPT Codex
- OpenAI Codex
- Codex CLI
- Codex app เฉพาะเมื่อผู้สอนอนุญาตอย่างชัดเจน
- Codex ใน IDE หรือ coding environment ถ้ามีให้ใช้

สำหรับรายวิชานี้ workflow ที่แนะนำคือ:

```text
VS Code + Codex CLI
```

หมายความว่า:

1. นักศึกษาเขียนและทดสอบ code ใน VS Code
2. นักศึกษาเปิด terminal ของ VS Code
3. นักศึกษารัน Codex CLI จาก terminal ของ VS Code
4. Codex ช่วย review, debug หรือทดสอบ code

Codex app ใช้ได้เฉพาะเมื่อผู้สอนอนุญาตอย่างชัดเจน

แม้ใช้ Codex app นักศึกษายังต้อง:

- ใช้ VS Code เป็น editor ทางการ
- ทดสอบ code สุดท้ายใน VS Code
- ส่ง code สุดท้ายเข้า OJ ด้วยตนเอง
- ทำตามนโยบายการใช้ AI ของรายวิชา
- ใช้ไฟล์ `AGENTS.md` ที่รายวิชาเตรียมไว้ ถ้า app รองรับ project instructions หรือ project context

ถ้าใช้ ChatGPT เป็น browser chat ปกติ ให้อ่าน:

```text
workflows/STUDENT_WORKFLOW_WEB_CHAT.md
```

AI coding tools อื่น ๆ ไม่อยู่ใน workflow ของรายวิชา เว้นแต่ผู้สอนประกาศ workflow เพิ่มเติมแยกต่างหาก

---

## 3. กฎของรายวิชา: VS Code ยังคงเป็น Editor ทางการ

VS Code คือ editor ทางการของรายวิชานี้

นักศึกษาต้องใช้ VS Code เพื่อเขียน รัน ทดสอบ และเตรียม code สุดท้ายก่อนส่งเข้า OJ

Codex เป็นเพียงผู้ช่วย

Codex ไม่ใช่ editor ทางการ

Codex ไม่ใช่ที่ส่งคำตอบ

OJ ของรายวิชายังคงเป็นที่ส่ง code อย่างเป็นทางการ

---

## 4. Codex ช่วยอะไรได้บ้าง

Codex อาจช่วย:

- review แผนแรกของนักศึกษา
- อธิบาย concept ของ Python
- อธิบาย error message
- หา bug ใน code ที่นักศึกษาเขียนไว้แล้ว
- เสนอ test cases
- ตรวจ logic ของ input และ output
- อธิบายว่าทำไม test case จึงผิด
- เสนอการปรับ code เล็กน้อยหลังจากอธิบายเหตุผลแล้ว

Codex ต้องไม่มาแทนความคิดของนักศึกษา

นักศึกษาห้ามใช้ Codex เพื่อ:

- แก้โจทย์ OJ ทั้งข้อจากศูนย์
- สร้าง accepted code แบบสมบูรณ์โดยที่นักศึกษาไม่มีความพยายามของตนเองก่อน
- rewrite solution ทั้งหมดโดยไม่มีคำอธิบาย
- ส่งเข้า OJ
- เขียน `submission.md` แทนนักศึกษา
- เขียน `ai_reflection.md` แทนนักศึกษา
- แต่ง test results ปลอม
- แต่ง OJ results ปลอม

ถ้านักศึกษาอธิบาย code สุดท้ายไม่ได้ ก็ไม่ควรส่ง code นั้น

---

## 5. ก่อนใช้ Codex

ก่อนใช้ Codex กับโจทย์ OJ ใด ๆ ให้ทำขั้นตอนต่อไปนี้ก่อน

### Step 1: อ่านโจทย์ OJ ด้วยตนเอง

อ่าน problem statement ใน course OJ

อย่าถาม Codex ทันที

### Step 2: คิดด้วยตนเองก่อน

ก่อนใช้ Codex นักศึกษาต้องมีความพยายามของตนเองก่อน

อย่างน้อยควรรู้หรือเขียน:

```text
Problem understanding:
Input:
Output:
Constraints:
First plan:
```

ถ้าโจทย์เป็น learning-log required ให้เขียนส่วนนี้ใน `submission.md`

ถ้าโจทย์ไม่ใช่ learning-log required อาจเขียนเป็น private note หรือเขียนในกระดาษก็ได้

ความเข้าใจของนักศึกษาอาจยังไม่ครบหรืออาจผิดได้

ไม่เป็นไร

ประเด็นสำคัญคือ นักศึกษาได้ลองคิดก่อนใช้ Codex

---

## 6. ติดตั้ง Codex CLI

Codex CLI เป็น app/command-line tool

ต้องติดตั้งก่อนจึงจะใช้คำสั่ง `codex` ได้

ถ้า Codex CLI ติดตั้งอยู่แล้วในคอมพิวเตอร์ของนักศึกษาหรือเครื่อง lab ให้ข้ามหัวข้อนี้ได้

### Windows PowerShell

เปิด Windows PowerShell

รันคำสั่งนี้:

```powershell
powershell -ExecutionPolicy ByPass -c "irm https://chatgpt.com/codex/install.ps1 | iex"
```

หลังติดตั้ง ตรวจว่า Codex ใช้งานได้:

```powershell
codex
```

ครั้งแรกที่รัน Codex ระบบจะขอให้ sign in

ให้ sign in ด้วยบัญชี ChatGPT ถ้า plan ของนักศึกษารองรับ Codex

### macOS or Linux

เปิด Terminal แล้วรัน:

```bash
curl -fsSL https://chatgpt.com/codex/install.sh | sh
```

หลังติดตั้ง ตรวจว่า Codex ใช้งานได้:

```bash
codex
```

ครั้งแรกที่รัน Codex ระบบจะขอให้ sign in

ให้ sign in ด้วยบัญชี ChatGPT ถ้า plan ของนักศึกษารองรับ Codex

### If Installation Fails

อย่าลองรันคำสั่งสุ่มจาก internet

ให้ถามผู้สอนหรือ TA

สำหรับรายวิชานี้ ให้ใช้เฉพาะวิธีติดตั้งที่ผู้สอนให้ หรือ official Codex documentation เท่านั้น

---

## 7. สร้าง Course Project Folder

สร้าง folder หลักหนึ่ง folder สำหรับรายวิชานี้

ชื่อ folder ที่แนะนำ:

```text
pscp
```

ภายใน `pscp-<student-id>` ให้เก็บ OJ working folders

ตัวอย่าง:

```text
pscp-<student-id>/
├── AGENTS.md
├── oj2198_work/
│   └── main.py
├── oj0301_work/
│   └── main.py
└── oj1994_work/
    └── main.py
```

สำหรับ OJ problem 0301 ให้สร้าง:

```text
pscp-<student-id>/oj0301_work/main.py
```

ใช้ `main.py` สำหรับเขียนและทดสอบ code ในเครื่อง

ห้าม upload `main.py` หรือ `solution.py` ไปยัง public GitHub learning log

สำหรับ GitHub learning log ให้ใช้เฉพาะ:

```text
submission.md
ai_reflection.md, if AI was used
```

---

## 8. เพิ่มไฟล์ Course `AGENTS.md`

Codex สามารถใช้ไฟล์ชื่อ:

```text
AGENTS.md
```

สำหรับรายวิชานี้ ผู้สอนเตรียมไฟล์พร้อมใช้ไว้ที่:

```text
instructions/AGENTS.md
```

นักศึกษาควร copy ไฟล์นี้ไปไว้ใน local course folder เป็น:

```text
pscp-<student-id>/AGENTS.md
```

นักศึกษาไม่ควรเขียน `AGENTS.md` เอง

นักศึกษาไม่ควร copy instruction สุ่มจาก internet มาใส่ใน `AGENTS.md`

นักศึกษาไม่จำเป็นต้อง copy เนื้อหาทั้งหมดของ `instructions/COURSE_AI_INSTRUCTIONS.md` ใส่ Codex ทุกครั้ง

ไฟล์ `instructions/AGENTS.md` ที่ให้ไว้มี course AI rules อยู่แล้ว

### Important

ให้เริ่ม Codex จาก folder `pscp-<student-id>` เสมอ

วิธีนี้ช่วยให้ Codex หาและทำตาม course `AGENTS.md` ได้

---

## 9. เปิด Project ใน VS Code

เปิด VS Code

เปิด folder:

```text
pscp
```

อย่าเปิดเฉพาะ `oj0301_work`

ให้เปิด folder หลัก `pscp-<student-id>` เพื่อให้เห็น:

```text
AGENTS.md
oj0301_work/
```

จากนั้นสร้างหรือเปิด:

```text
oj0301_work/main.py
```

เขียน code attempt แรกของตนเองใน `main.py`

---

## 10. เริ่ม Codex CLI จาก VS Code

ใน VS Code เปิด:

```text
Terminal > New Terminal
```

ตรวจว่า terminal อยู่ที่ folder `pscp-<student-id>`

ตรวจได้ด้วย:

```bash
pwd
```

บน Windows PowerShell ใช้ได้เช่นกัน:

```powershell
Get-Location
```

path ควรลงท้ายด้วย:

```text
pscp
```

จากนั้นรัน:

```bash
codex
```

ถ้า Codex ขอให้ sign in ให้ sign in ด้วยบัญชี ChatGPT

---

## 11. Prompt แรกที่ควรถาม Codex

อย่าขอให้ Codex แก้โจทย์ให้

ให้เริ่มจากความพยายามของตนเอง

ตัวอย่าง first prompt ที่ดี:

```text
I am solving an OJ problem for my PSCP course.

Follow AGENTS.md.

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
```

ให้เปลี่ยน `oj0301_work/main.py` เป็นชื่อ folder จริงของตนเอง

---

## 12. ถ้าต้องการให้ Codex Review Code

ใช้ prompt ลักษณะนี้:

```text
Please review oj0301_work/main.py.

Do not rewrite the whole file.

First explain:
1. what my code is trying to do,
2. whether it matches my first plan,
3. one possible bug or missing case.

Do not edit the file yet.
```

---

## 13. ถ้าต้องการให้ Codex Debug

ใช้ prompt ลักษณะนี้:

```text
My code fails this test case.

File:
oj0301_work/main.py

Input:
...

Expected output:
...

Actual output:
...

Please explain the likely bug first.

Do not rewrite the whole file.

Suggest the smallest change only.
```

---

## 14. ถ้าต้องการให้ Codex เสนอ Test Cases

ใช้ prompt ลักษณะนี้:

```text
Please suggest 3 useful test cases for this problem.

Do not solve the problem.

For each test case, include:
1. why this case is useful,
2. input,
3. expected output.

Do not use hidden OJ tests.
```

หลังจาก Codex เสนอ test cases แล้ว นักศึกษาต้องรันเองใน VS Code

---

## 15. ถ้าอนุญาตให้ Codex แก้ Code

Codex อาจขอแก้ไฟล์หรือเสนอ patch

ก่อนอนุญาตให้แก้ ให้ถามว่า:

```text
Explain what you plan to change before editing the file.
```

จากนั้น ถ้าการแก้ไขสมเหตุสมผล ให้ยอมให้แก้เฉพาะส่วนเล็ก ๆ

instruction ที่ดี:

```text
Apply only the smallest necessary change to oj0301_work/main.py.

Do not rewrite unrelated parts of the file.

After editing, explain what changed and why.
```

หลังจาก Codex แก้ไฟล์แล้ว:

1. เปิด `main.py` ใน VS Code
2. อ่าน code ที่ถูกแก้
3. ตรวจว่าตนเองเข้าใจ
4. รัน code ด้วยตนเอง
5. ทดสอบอย่างน้อย 3 cases ที่แตกต่างกัน

ถ้า Codex แก้เยอะเกินไป ให้ reject change หรือขอให้ทำให้ง่ายลง

---

## 16. การรัน Code

รัน code ใน VS Code terminal

ตัวอย่าง:

```bash
python oj0301_work/main.py
```

หรือ:

```bash
python3 oj0301_work/main.py
```

ทดสอบอย่างน้อย 3 cases ที่แตกต่างกัน

สำหรับแต่ละ case นักศึกษาควรรู้:

- ทำไมเลือก case นี้
- expected output
- actual output
- ผ่านหรือไม่

Codex อาจช่วยเสนอ tests ได้ แต่นักศึกษารับผิดชอบการรันและตรวจด้วยตนเอง

---

## 17. ส่งเข้า OJ ด้วยตนเอง

หลังทดสอบแล้ว ให้ส่ง final code เข้า course OJ ด้วยตนเอง

ห้ามให้ Codex ส่งแทน

ถ้าโจทย์เป็น learning-log required ให้บันทึก:

- OJ problem number/title
- OJ submission ID
- OJ status

---

## 18. โจทย์ที่เป็น Learning-Log-Required

ถ้า OJ problem เป็น learning-log required และใช้ Codex ให้ส่ง:

```text
submission.md
ai_reflection.md
```

### ใน `submission.md`

เขียนด้วยตนเอง:

- OJ information
- เวลาที่ใช้คิดเองก่อนใช้ AI
- problem understanding
- first plan
- final approach
- test cases อย่างน้อย 3 cases

ห้ามใส่ full source code ใน GitHub

ให้ใช้ OJ submission ID แทน

### ใน `ai_reflection.md`

เขียน reflection ด้วยตนเอง

ให้ระบุ:

- ว่าใช้ Codex
- ใช้ course `AGENTS.md` หรือไม่
- ทำตาม workflow นี้หรือไม่
- ถาม Codex ให้ช่วยอะไร
- Codex ช่วยให้สังเกตอะไร
- นักศึกษาตรวจหรือแก้อะไรด้วยตนเอง
- นักศึกษาได้เรียนรู้อะไร

ห้ามวาง Codex conversation ทั้งหมด

ห้ามให้ Codex เขียน reflection แทน

---

## 19. โจทย์ OJ ปกติ

ถ้าโจทย์ไม่ใช่ learning-log required:

- ส่ง code เข้า OJ เท่านั้น
- ไม่ต้องมี GitHub learning log
- ไม่ต้องมี `submission.md`
- ไม่ต้องมี `ai_reflection.md`

อย่างไรก็ตาม นักศึกษายังต้องเข้าใจ final code ของตนเอง

ผู้สอนอาจถามให้อธิบาย:

- problem understanding
- algorithm
- code
- test cases
- Codex ช่วยอะไร
- นักศึกษาตรวจสอบอะไรด้วยตนเอง

---

## 20. สิ่งที่ไม่ควรใส่ใน Folder `pscp-<student-id>`

ห้ามใส่สิ่งเหล่านี้ใน folder `pscp-<student-id>`:

- API keys
- access tokens
- private files
- hidden OJ tests
- official solutions
- unrelated personal files
- course-restricted materials ที่ไม่ควรถูก copy

สำหรับ OJ work folders ให้เก็บเฉพาะสิ่งที่จำเป็นสำหรับการเขียนและทดสอบ code

ตัวอย่าง:

```text
pscp-<student-id>/oj0301_work/main.py
```

ไฟล์ optional เช่น `input.txt` ใช้ได้เฉพาะสำหรับการทดสอบในเครื่องของตนเอง

ห้าม upload source code files ไปยัง public GitHub learning log

---

## 21. ตัวอย่าง Prompt ที่ดีสำหรับ Codex

### Plan Review

```text
Please review my first plan.

Do not write the full code.

Tell me:
1. what seems correct,
2. what may be missing,
3. one question I should think about next.
```

### Code Review

```text
Please review oj0301_work/main.py.

Do not edit the file yet.

Explain one possible issue and suggest one small next step.
```

### Debugging

```text
My code fails this test case.

Input:
...

Expected output:
...

Actual output:
...

Please explain the likely bug first.

Do not rewrite the whole code.
```

### Small Fix

```text
Suggest the smallest code change needed.

Explain why it works.

Do not rewrite unrelated parts of the file.
```

### Test Cases

```text
Please suggest 3 useful test cases.

Do not solve the problem.

For each test case, explain why it is useful.
```

---

## 22. Prompt ที่ไม่ควรใช้กับ Codex

หลีกเลี่ยง prompt เช่น:

```text
Solve this OJ problem.
```

```text
Write the full accepted code.
```

```text
Make my code pass the OJ.
```

```text
Rewrite the whole file.
```

```text
Edit everything until it works.
```

```text
Submit this to the OJ.
```

```text
Write my submission.md.
```

```text
Write my ai_reflection.md.
```

---

## 23. ถ้า Codex ให้ความช่วยเหลือมากเกินไป

บางครั้ง Codex อาจให้ full solution เร็วเกินไป

อย่าคัดลอกทันที

ให้ตอบว่า:

```text
Please stop giving the full solution.

Explain only the main idea and ask me guiding questions.

I want to write the code myself.
```

จากนั้นให้นักศึกษาเขียน code ของตนเองใน VS Code

นักศึกษาอาจใช้คำอธิบายเพื่อเพิ่มความเข้าใจได้ แต่ห้ามส่ง code ที่ตนเองอธิบายไม่ได้

---

## 24. ถ้า Codex แก้ Code มากเกินไป

ถ้า Codex เปลี่ยนหลายบรรทัดเกินไป ให้ขอลดขนาดการแก้ไข

Prompt:

```text
This change is too large.

Please explain the smallest necessary change only.

Do not rewrite unrelated code.
```

นักศึกษาอาจ reject การแก้ของ Codex แล้วเขียน version ที่ง่ายกว่าด้วยตนเองได้

---

## 25. คำสั่ง: ต้องระวัง

Codex อาจรันคำสั่งได้

สำหรับรายวิชานี้ คำสั่งที่มักปลอดภัย เช่น:

```bash
python oj0301_work/main.py
```

หรือ:

```bash
python3 oj0301_work/main.py
```

ให้ระวังคำสั่งที่:

- ลบไฟล์
- reset Git history
- install packages
- upload files
- เปิดเผย secrets
- แก้ folder อื่นที่ไม่เกี่ยวข้อง

สำหรับโจทย์ PSCP ระดับเริ่มต้น ส่วนใหญ่ไม่จำเป็นต้อง install package

ถ้าไม่เข้าใจคำสั่ง อย่าอนุญาตให้รัน

ให้ถามว่า:

```text
Explain what this command does before running it.
```

---

## 26. Optional: การใช้ Codex App

Codex app มีให้ใช้บน macOS และ Windows

อย่างไรก็ตาม สำหรับรายวิชานี้ Codex app ไม่ใช่ workflow หลักที่แนะนำ

workflow หลักที่แนะนำคือ:

```text
VS Code + Codex CLI
```

นักศึกษาใช้ Codex app ได้เฉพาะเมื่อผู้สอนอนุญาตอย่างชัดเจน

ถ้าผู้สอนอนุญาตให้ใช้ Codex app นักศึกษายังต้องทำตามกฎต่อไปนี้:

1. เลือก folder `pscp-<student-id>` เป็น project folder
2. ตรวจว่าไฟล์ `AGENTS.md` ที่รายวิชาให้ไว้อยู่ใน folder `pscp-<student-id>`
3. ใช้ Codex เป็นเพียง coach, reviewer, debugger หรือ test-case helper
4. ห้ามขอให้ Codex แก้โจทย์ OJ ทั้งข้อจากศูนย์
5. ห้ามให้ Codex ส่งเข้า OJ
6. เขียน รัน และทดสอบ final code ใน VS Code
7. ส่ง final code เข้า OJ ด้วยตนเอง
8. ถ้าโจทย์เป็น learning-log required ให้ทำ `submission.md` และ `ai_reflection.md`

สำหรับงาน PSCP ระดับเริ่มต้น Codex app อาจทรงพลังเกินความจำเป็น

ใช้อย่างระมัดระวัง

---

## 27. Quick Self-Check

Checklist นี้ใช้ตรวจตนเองเท่านั้น

นักศึกษาไม่ต้องส่ง checklist นี้

ก่อนส่งเข้า OJ ให้ตรวจว่า:

```text
[ ] I used VS Code to write, run, and test my code.
[ ] I wrote my own problem understanding before using Codex.
[ ] I wrote my own first plan before using Codex.
[ ] I used the course AGENTS.md file.
[ ] I used Codex as a coach, reviewer, debugger, or test-case helper.
[ ] I reviewed any Codex-generated code or edits.
[ ] I tested at least 3 different cases by myself.
[ ] I understand my final code.
[ ] I can explain what Codex helped with.
```

ถ้าโจทย์เป็น learning-log required ให้ทำ:

```text
submission.md
ai_reflection.md
```

---

## 28. สรุปสุดท้าย

Codex มีพลังมากเพราะสามารถทำงานกับ code และคำสั่งได้

สิ่งนี้ทำให้ Codex มีความเสี่ยงเช่นกัน ถ้าใช้อย่างไม่ระมัดระวัง

ใช้ Codex เพื่อเรียนรู้ review debug และ test

อย่าใช้ Codex เพื่อแทนการแก้ปัญหาด้วยตนเอง

final OJ submission เป็นความรับผิดชอบของนักศึกษา
