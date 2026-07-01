# แนวทางปฏิบัติการใช้เครื่องคอมพิวเตอร์ร่วมกันในห้อง Lab

เอกสารนี้ใช้สำหรับนักศึกษาที่ใช้เครื่องคอมพิวเตอร์ร่วมกันในห้อง Lab สำหรับวิชา Problem Solving and Computer Programming

เครื่องในห้อง Lab เป็นเครื่องใช้ร่วมกัน นักศึกษาหลายคนอาจใช้เครื่องเดียวกันคนละเวลา

นักศึกษาต้องดูแล account, ไฟล์งาน, AI session และ OJ submission ของตนเองให้ปลอดภัย และต้องเคารพความเป็นส่วนตัวและงานของนักศึกษาคนอื่น

---

## 1. หลักการสำคัญ

เมื่อใช้เครื่อง Lab ที่เป็นเครื่องใช้ร่วมกัน นักศึกษาต้อง:

1. ใช้ account ของตนเองเท่านั้น
2. ใช้ working folder ของตนเองเท่านั้น
3. ปกป้อง password, token และ login session ของตนเอง
4. ไม่ทิ้งไฟล์หรือ account เปิดค้างไว้หลังใช้งาน
5. ตรวจสอบว่าเครื่องมือ AI ไม่ได้อ่านไฟล์ของนักศึกษาคนอื่น
6. ส่งเฉพาะงานของตนเองเข้า OJ
7. logout และเก็บงานให้เรียบร้อยก่อนออกจากเครื่อง

เครื่อง Lab ไม่ใช่เครื่องส่วนตัว

นักศึกษาต้องรับผิดชอบในการตรวจว่าเครื่องพร้อมใช้อย่างปลอดภัยก่อนเริ่มงาน และต้องจัดการให้เรียบร้อยก่อนออกจากเครื่อง

---

## 2. Working Folder ที่ต้องใช้

นักศึกษาต้องใช้ working folder ส่วนตัวของตนเอง

ชื่อ folder ที่แนะนำ:

```text
pscp-<student-id>
```

ให้แทน `<student-id>` ด้วยเลขประจำตัวนักศึกษาของตนเอง

ไม่ต้องใส่เครื่องหมาย `< >` ในชื่อ folder จริง

ตัวอย่าง:

```text
pscp-66123456
```

ถ้าเป็นงานชั่วคราวระหว่างทำโจทย์ OJ ให้ใช้ problem-specific working folder เช่น:

```text
pscp-66123456/
├── oj2198_work/
├── oj0301_work/
└── oj1994_work/
```

ถ้าเป็นโจทย์ที่ต้องส่ง learning log ให้ใช้ folder ตาม OJ problem ID:

```text
pscp-66123456/
├── oj2198/
│   ├── submission.md
│   └── ai_reflection.md
└── oj0301/
    └── submission.md
```

ชื่อ folder แบบ `oj<problem-id>` ต้องใช้เลขโจทย์ OJ แบบ 4 หลัก

ตัวอย่าง:

```text
oj2198
oj0301
oj1994
```

ห้ามใช้ `oj001`, `oj002` หรือ `oj003` เว้นแต่เลขเหล่านั้นเป็น OJ problem ID จริง

---

## 3. ก่อนเริ่มใช้เครื่อง Lab

ก่อนเริ่มทำงาน นักศึกษาต้องตรวจว่า:

- ไม่มี VS Code project ของนักศึกษาคนอื่นเปิดค้างอยู่
- ไม่มี terminal session ของนักศึกษาคนอื่นค้างอยู่
- ไม่มี account GitHub, OJ, ChatGPT, Claude, Gemini, Codex หรือ Claude Code ของคนอื่น login ค้างอยู่
- ไม่มีไฟล์ของนักศึกษาคนอื่นเปิดอยู่ใน VS Code
- folder ปัจจุบันไม่ใช่ folder ของนักศึกษาคนอื่น

ขั้นตอนที่แนะนำ:

1. ปิด browser tabs เดิม
2. ปิด VS Code windows เดิมที่ไม่ใช่ของตนเอง
3. เปิดเฉพาะ folder ของตนเอง
4. ใช้ Private / Incognito browser window เมื่อต้อง login web services
5. ตรวจตำแหน่งใน terminal ก่อนรันคำสั่ง

ใช้คำสั่งนี้เพื่อตรวจตำแหน่งปัจจุบัน:

```bash
pwd
ls
```

ต้องแน่ใจว่าอยู่ใน folder ของตนเอง เช่น:

```text
pscp-66123456/
```

---

## 4. ระหว่างทำงานในห้อง Lab

นักศึกษาต้อง:

- ทำงานเฉพาะใน folder ของตนเอง
- เขียนและทดสอบ code ใน VS Code
- ส่ง final code เข้า OJ ด้วยตนเอง
- ใช้ GitHub account ของตนเองเท่านั้น
- ใช้ AI account ของตนเองเท่านั้น
- เก็บ password, token และ API key ให้เป็นความลับ
- ตรวจสอบก่อน copy code, error message หรือเนื้อหาไฟล์ไปให้ AI

นักศึกษาห้าม:

- เปิด folder ของนักศึกษาคนอื่น
- อ่าน code ของนักศึกษาคนอื่น
- copy ไฟล์ของนักศึกษาคนอื่น
- แก้ไขหรือลบไฟล์ของนักศึกษาคนอื่น
- ส่ง solution ของนักศึกษาคนอื่น
- ใช้ account ที่คนอื่น login ค้างไว้
- อนุญาตให้ AI อ่าน folder ที่อาจมีไฟล์ของนักศึกษาคนอื่น

---

## 5. การใช้ AI บนเครื่อง Lab ที่ใช้ร่วมกัน

AI ใช้ได้เฉพาะตามนโยบายการใช้ AI ของรายวิชา

บนเครื่อง Lab ที่ใช้ร่วมกัน workflow ที่ปลอดภัยที่สุดคือ:

```text
VS Code + web chat ใน Private / Incognito browser window
```

ตัวอย่าง web chat tools:

```text
ChatGPT
Claude
Gemini web chat
```

เมื่อใช้ AI web chat นักศึกษาต้อง:

1. login ด้วย account ของตนเอง
2. ไม่ save password ใน browser
3. หลีกเลี่ยงการกด "remember me" บนเครื่องใช้ร่วมกัน
4. paste เฉพาะ code, error message หรือคำอธิบายที่เป็นของตนเอง
5. ไม่ upload folder ที่อาจมีไฟล์ของนักศึกษาคนอื่น
6. logout และปิด Private / Incognito window หลังใช้งาน

นักศึกษาห้ามส่ง code ที่ AI สร้างให้โดยที่ตนเองอธิบายไม่ได้

นักศึกษายังต้องเขียน รัน ทดสอบ และส่ง final code ด้วยตนเอง

---

## 6. การใช้ Codex หรือ Claude Code บนเครื่อง Lab

Codex CLI และ Claude Code CLI สามารถอ่านไฟล์ แก้ไฟล์ และรันคำสั่งได้

ดังนั้นต้องระมัดระวังเป็นพิเศษเมื่อใช้บนเครื่องใช้ร่วมกัน

นักศึกษาสามารถใช้ Codex CLI หรือ Claude Code CLI บนเครื่อง Lab ได้เฉพาะเมื่อผู้สอนอนุญาต

ก่อนใช้ Codex หรือ Claude Code นักศึกษาต้องตรวจว่าอยู่ใน folder ใด:

```bash
pwd
ls
```

current directory ต้องอยู่ใน folder ของนักศึกษาเอง เช่น:

```text
pscp-66123456/
```

นักศึกษาห้ามสั่งให้ Codex หรือ Claude Code:

- scan ทั้งเครื่อง
- ตรวจ folder ของนักศึกษาคนอื่น
- แก้ไฟล์นอก folder ของตนเอง
- อ่าน token, password หรือ private files
- ส่ง OJ แทน
- เขียน `submission.md` หรือ `ai_reflection.md` แทนนักศึกษา

เมื่อใช้ Claude Code นักศึกษาควร copy course instruction files ไปไว้ใน folder ของตนเองเท่านั้น:

```text
pscp-66123456/AGENTS.md
pscp-66123456/CLAUDE.md
```

เมื่อใช้ Codex นักศึกษาควร copy:

```text
pscp-66123456/AGENTS.md
```

ห้ามวาง course AI instruction files ไว้ใน folder ของนักศึกษาคนอื่น

---

## 7. ความปลอดภัยของ GitHub, OJ และ Browser

นักศึกษาต้องปกป้อง account ของตนเอง

ห้าม save password บนเครื่อง Lab

นักศึกษาต้อง logout จาก:

- OJ
- GitHub
- ChatGPT
- Claude
- Gemini
- Codex
- Claude Code
- email หรือ account ส่วนตัวอื่น ๆ

ควรใช้ Private / Incognito mode เมื่อเป็นไปได้

ห้ามทิ้ง access tokens, API keys, `.env` files, SSH keys หรือ browser sessions ไว้บนเครื่อง Lab

ถ้านักศึกษาลืม logout account ของตนเอง ให้รีบ logout ทันทีเมื่อพบ และแจ้งผู้สอนหรือ TA หากจำเป็น

---

## 8. Checklist ก่อนออกจากเครื่อง

ก่อนออกจากเครื่อง Lab นักศึกษาต้อง:

1. save งานของตนเอง
2. push learning-log files ไปยัง GitHub ถ้าต้องส่ง
3. submit final code เข้า OJ ถ้าพร้อม
4. ปิด VS Code
5. logout จาก OJ
6. logout จาก GitHub
7. logout จาก AI tools
8. ปิด browser windows ทั้งหมด
9. ลบไฟล์ชั่วคราวจาก Desktop, Downloads และ Trash ถ้าไม่ต้องใช้แล้ว
10. ตรวจว่าไม่มี password, token หรือ private files เหลืออยู่

คำสั่งตรวจสุดท้ายที่แนะนำ:

```bash
pwd
ls
```

ตรวจว่าไม่มีไฟล์ส่วนตัวเหลือในตำแหน่ง shared location เว้นแต่ผู้สอนสั่งให้เก็บไฟล์ไว้ที่นั่น

---

## 9. ถ้าพบ Account หรือไฟล์ของนักศึกษาคนอื่น

ถ้าพบ account ของนักศึกษาคนอื่น login ค้างอยู่:

1. ห้ามใช้ account นั้น
2. ห้ามอ่านข้อความส่วนตัวหรือไฟล์ส่วนตัว
3. logout ถ้ามั่นใจว่าทำได้อย่างปลอดภัย
4. แจ้งผู้สอนหรือ TA

ถ้าพบไฟล์ของนักศึกษาคนอื่น:

1. ห้ามเปิด
2. ห้าม copy
3. ห้ามแก้ไขหรือลบ
4. แจ้งผู้สอนหรือ TA ถ้าไฟล์นั้นอาจทำให้เกิดความสับสน

---

## 10. Academic Integrity

การใช้เครื่อง Lab ร่วมกันไม่ได้เปลี่ยนกติกาของรายวิชา

นักศึกษายังต้องรับผิดชอบในการ:

- เขียน code ของตนเอง
- เข้าใจ final solution ของตนเอง
- ส่ง OJ ด้วยตนเอง
- เขียน `submission.md` ด้วยตนเอง
- เขียน `ai_reflection.md` ด้วยตนเองถ้าใช้ AI
- เปิดเผยความช่วยเหลือจากคนอื่นเมื่อจำเป็น
- ใช้ AI เฉพาะตามที่นโยบายรายวิชาอนุญาต

นักศึกษาห้ามอ้างว่างานของคนอื่น งานที่ AI สร้าง หรือไฟล์ที่ค้างอยู่บนเครื่อง Lab เป็นงานของตนเอง

---

## 11. Checklist แบบสั้น

ก่อนเริ่ม:

```text
ใช้ folder ของตนเอง
ใช้ account ของตนเอง
ตรวจตำแหน่ง VS Code และ terminal
ใช้ Private / Incognito เมื่อต้อง login web
```

ระหว่างทำงาน:

```text
ใช้เฉพาะไฟล์ของตนเอง
ใช้ AI ตามนโยบายรายวิชาเท่านั้น
ไม่ให้ AI อ่านไฟล์ของนักศึกษาคนอื่น
ทดสอบ code ใน VS Code
ส่ง OJ ด้วยตนเอง
```

ก่อนออกจากเครื่อง:

```text
save งาน
push learning log ถ้าต้องส่ง
logout จาก OJ, GitHub และ AI tools
ปิด VS Code และ browser
ลบไฟล์ชั่วคราว
ไม่ทิ้ง password, token หรือ session ไว้
```
