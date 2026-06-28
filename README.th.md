# แนวทางการใช้ AI สำหรับวิชา PSCP

Repository นี้จัดทำขึ้นเพื่ออธิบายแนวทางการใช้ AI อย่างรับผิดชอบในวิชา Problem Solving and Computer Programming ของ IT KMITL

Repository นี้ไม่เก็บโจทย์ OJ, เฉลยทางการ, hidden test cases หรือเอกสารของรายวิชาที่ไม่ควรเผยแพร่

Editor ทางการของวิชานี้คือ VS Code

นักศึกษาต้องใช้ VS Code ในการเขียน รัน และทดสอบโค้ด Python ก่อนส่งโค้ดสุดท้ายเข้า OJ ของรายวิชา

---

## 1. จุดประสงค์ของ Repository นี้

Repository นี้อธิบายว่านักศึกษาควรใช้เครื่องมือ AI ในรายวิชานี้อย่างไร

AI สามารถใช้เป็น:

- โค้ชช่วยคิดแก้ปัญหา
- ผู้ช่วยตรวจ pseudocode หรือ flowchart
- ผู้ช่วย debug
- ผู้ช่วยคิด test cases
- ผู้ช่วยปรับภาษาใน reflection

AI ต้องไม่ถูกใช้แทนความคิดของนักศึกษา

เป้าหมายหลักคือให้นักศึกษาพัฒนาทักษะการแก้ปัญหาและการเขียนโปรแกรม ไม่ใช่เพียงเพื่อให้ได้คำตอบ Accepted จาก OJ

---

## 2. ไฟล์ใน Repository นี้

| ไฟล์ | จุดประสงค์ |
|---|---|
| `README.md` | นโยบายหลักและกติกาการส่งงานของรายวิชา |
| `README.th.md` | README ภาษาไทยสำหรับนักศึกษา |
| `instructions/COURSE_AI_INSTRUCTIONS.md` | คำสั่งหลักสำหรับ AI coach เช่น ChatGPT, Claude, Gemini web chat และเครื่องมือคล้ายกัน |
| `instructions/COURSE_AI_INSTRUCTIONS.th.md` | คำอธิบายภาษาไทยของคำสั่ง AI coach |
| `instructions/AGENTS.md` | กฎกลางสำหรับ coding agents เช่น Codex และ Claude Code |
| `instructions/CLAUDE.md` | Claude Code instruction wrapper ที่ import `AGENTS.md` |
| `workflows/STUDENT_WORKFLOW_WEB_CHAT.md` | Workflow สำหรับ AI ที่ใช้ผ่าน browser หรือ chat |
| `workflows/STUDENT_WORKFLOW_WEB_CHAT.th.md` | Workflow ภาษาไทยสำหรับ AI ที่ใช้ผ่าน browser หรือ chat |
| `workflows/STUDENT_WORKFLOW_CODING_TOOLS.md` | Workflow ทั่วไปสำหรับ AI coding tools |
| `workflows/STUDENT_WORKFLOW_CODING_TOOLS.th.md` | Workflow ภาษาไทยทั่วไปสำหรับ AI coding tools |
| `workflows/STUDENT_WORKFLOW_CHATGPT_CODEX.md` | Workflow สำหรับ ChatGPT Codex, OpenAI Codex, Codex CLI และ Codex app |
| `workflows/STUDENT_WORKFLOW_CHATGPT_CODEX.th.md` | Workflow ภาษาไทยสำหรับ ChatGPT Codex, OpenAI Codex, Codex CLI และ Codex app |
| `workflows/STUDENT_WORKFLOW_CLAUDE_CODE.md` | Workflow สำหรับ Claude Code CLI และ Claude desktop app / Claude Cowork เมื่อผู้สอนอนุญาต |
| `workflows/STUDENT_WORKFLOW_CLAUDE_CODE.th.md` | Workflow ภาษาไทยสำหรับ Claude Code CLI และ Claude desktop app / Claude Cowork เมื่อผู้สอนอนุญาต |
| `templates/SUBMISSION_TEMPLATE.md` | Template สำหรับสร้าง `submission.md` เมื่อโจทย์กำหนดให้ส่ง learning log |
| `templates/SUBMISSION_TEMPLATE.th.md` | Template ภาษาไทยสำหรับ `submission.md` |
| `templates/AI_REFLECTION_TEMPLATE.md` | Template สำหรับสร้าง `ai_reflection.md` เมื่อใช้ AI กับโจทย์ที่ต้องส่ง learning log |
| `templates/AI_REFLECTION_TEMPLATE.th.md` | Template ภาษาไทยสำหรับ `ai_reflection.md` |
| `examples/SUBMISSION_TEMPLATE_sample_no_AI.md` | ตัวอย่าง `submission.md` เมื่อไม่ได้ใช้ AI |
| `examples/SUBMISSION_TEMPLATE_sample_no_AI.th.md` | ตัวอย่างภาษาไทยของ `submission.md` เมื่อไม่ได้ใช้ AI |
| `examples/SUBMISSION_TEMPLATE_sample_AI.md` | ตัวอย่าง `submission.md` เมื่อใช้ AI |
| `examples/SUBMISSION_TEMPLATE_sample_AI.th.md` | ตัวอย่างภาษาไทยของ `submission.md` เมื่อใช้ AI |
| `examples/AI_REFLECTION_TEMPLATE_sample.md` | ตัวอย่าง `ai_reflection.md` |
| `examples/AI_REFLECTION_TEMPLATE_sample.th.md` | ตัวอย่างภาษาไทยของ `ai_reflection.md` |

ให้อ่าน `README.md` หรือ `README.th.md` ก่อน

ใช้ไฟล์ใน `templates/` เพื่อสร้างไฟล์ของตนเอง

สามารถอ่านตัวอย่างใน `examples/` เพื่อดูรูปแบบได้ แต่ห้ามคัดลอกเนื้อหาตัวอย่างไปเป็นงานของตนเอง

ไฟล์ `.th.md` มีไว้ให้นักศึกษาอ่านเป็นภาษาไทย

ไฟล์ English ยังคงเป็นไฟล์หลักสำหรับ AI tools และ coding agents

---

## 3. นโยบาย Editor ทางการ

VS Code คือ editor ทางการของรายวิชานี้

นักศึกษาต้องใช้ VS Code สำหรับ:

- เขียนโค้ด Python
- รันโค้ด Python
- ทดสอบโค้ดในเครื่อง
- เตรียมโค้ดสุดท้ายก่อนส่งเข้า OJ

เครื่องมือ AI เป็นเพียงผู้ช่วยภายใต้นโยบายของรายวิชา

AI-first editors เช่น Cursor ไม่ใช่ workflow ทางการ เว้นแต่ผู้สอนอนุญาตอย่างชัดเจน

ถ้าผู้สอนไม่ได้อนุญาต editor อื่นอย่างชัดเจน ให้ใช้ VS Code เท่านั้น

---

## 4. ควรอ่าน Workflow ไหน

ให้เลือก workflow ตามลักษณะการใช้ AI ไม่ใช่ตามว่า account เป็น free หรือ paid

| ถ้าใช้... | ให้อ่านไฟล์นี้ |
|---|---|
| ChatGPT, Claude, Gemini หรือ AI อื่นผ่าน browser/chat | `workflows/STUDENT_WORKFLOW_WEB_CHAT.md` |
| ChatGPT Codex, OpenAI Codex, Codex CLI หรือ Codex app | `workflows/STUDENT_WORKFLOW_CHATGPT_CODEX.md` |
| Claude Code CLI หรือ Claude desktop app / Claude Cowork เมื่อผู้สอนอนุญาต | `workflows/STUDENT_WORKFLOW_CLAUDE_CODE.md` |
| AI coding tools อื่น ๆ เมื่อผู้สอนอนุญาต | `workflows/STUDENT_WORKFLOW_CODING_TOOLS.md` |

ข้อสำคัญ:

- Free หรือ paid ไม่ใช่ประเด็นหลัก
- ประเด็นหลักคือ AI ใช้เป็น chat อย่างเดียว หรือ AI สามารถทำงานใน coding environment ได้
- ถ้า AI อ่านไฟล์ แก้โค้ด รันคำสั่ง หรือเสนอ code changes ใน VS Code หรือ terminal ได้ ให้ถือว่าเป็น coding tool
- GitHub Copilot ใน VS Code และ VS Code AI extensions อื่น ๆ ไม่ใช่ workflow ทางการ เว้นแต่ผู้สอนอนุญาต
- Cursor และ AI-first editors อื่น ๆ ไม่ใช่ workflow ทางการ เว้นแต่ผู้สอนอนุญาต เพราะรายวิชานี้กำหนดให้ใช้ VS Code

---

## 5. หมายเหตุสั้นสำหรับเครื่องมือเฉพาะ

รายละเอียด setup และวิธีใช้เต็มอยู่ในไฟล์ workflow ของแต่ละเครื่องมือ

ให้อ่าน workflow ที่ถูกต้องก่อนใช้เครื่องมือนั้น

### Codex

ถ้าใช้ ChatGPT Codex, OpenAI Codex, Codex CLI หรือ Codex app ให้อ่าน:

```text
workflows/STUDENT_WORKFLOW_CHATGPT_CODEX.md
```

สำหรับ Codex CLI workflow ที่แนะนำคือ:

```text
VS Code + Codex CLI
```

นักศึกษาควร copy:

```text
instructions/AGENTS.md
```

ไปไว้ใน local course folder เป็น:

```text
pscp/AGENTS.md
```

### Claude Code

ถ้าใช้ Claude Code ให้อ่าน:

```text
workflows/STUDENT_WORKFLOW_CLAUDE_CODE.md
```

สำหรับ Claude Code CLI workflow ที่แนะนำคือ:

```text
VS Code + Claude Code CLI
```

Claude Code อ่าน project instructions จาก:

```text
CLAUDE.md
```

นักศึกษาควร copy:

```text
instructions/AGENTS.md
instructions/CLAUDE.md
```

ไปไว้ใน local course folder เป็น:

```text
pscp/AGENTS.md
pscp/CLAUDE.md
```

### AI Coding Tools อื่น ๆ

AI coding tools อื่น ๆ ใช้ได้เฉพาะเมื่อผู้สอนอนุญาตอย่างชัดเจน

ถ้าได้รับอนุญาต ให้อ่าน:

```text
workflows/STUDENT_WORKFLOW_CODING_TOOLS.md
```

VS Code ยังคงเป็น editor ทางการ

OJ ของรายวิชายังคงเป็นที่ส่ง code อย่างเป็นทางการ

---

## 6. สิ่งที่นักศึกษาต้องเขียนเอง

สิ่งต่อไปนี้ต้องเขียนด้วยตนเอง AI อาจช่วย review, ถามคำถาม หรือเสนอแนะได้ แต่ AI ต้องไม่เขียนแทนนักศึกษาเพื่อส่งงาน

นักศึกษาต้องเขียนเอง:

1. ความเข้าใจโจทย์ของตนเอง
2. การวิเคราะห์ input, output และ constraints
3. pseudocode, flowchart idea หรือ first plan เริ่มต้น
4. คำอธิบาย algorithm ของตนเอง
5. final code ที่ส่งเข้า OJ และตนเองอธิบายได้
6. test cases และ test results ของตนเอง
7. `submission.md` เมื่อโจทย์กำหนดให้ส่ง learning log
8. `ai_reflection.md` เมื่อใช้ AI กับโจทย์ที่ต้องส่ง learning log

ห้ามส่ง:

- code ที่ AI สร้างและตนเองอธิบายไม่ได้
- problem analysis ที่ copy จาก AI โดยไม่ปรับและไม่เข้าใจ
- reflection ที่ AI แต่งขึ้นโดยไม่ตรงกับกระบวนการจริง
- pseudocode ที่ copy จาก AI โดยไม่เข้าใจ
- AI reflection ปลอม
- test results ปลอม
- OJ results ปลอม

นักศึกษาไม่ต้องส่ง AI conversation ทั้งหมด

แต่นักศึกษาต้องเขียนคำถามเอง อธิบายโจทย์ด้วยภาษาของตนเอง ให้ first plan ของตนเอง และตรวจสอบคำแนะนำของ AI ด้วยตนเอง

นักศึกษารับผิดชอบคำตอบสุดท้าย code สุดท้าย OJ submission และการอธิบายของตนเอง

---

## 7. Learning Log คืออะไร

Learning log คือ folder ใน GitHub สำหรับ OJ problem ที่ผู้สอนหรือ OJ ระบุว่าต้องส่ง learning log

Learning log ใช้บันทึกกระบวนการแก้ปัญหาของนักศึกษา และถ้ามีการใช้ AI กับโจทย์นั้น ให้บันทึก reflection การใช้ AI ด้วย

Learning log อาจมี:

| ไฟล์ | ความหมาย |
|---|---|
| `submission.md` | บันทึกกระบวนการแก้ปัญหาของนักศึกษา |
| `ai_reflection.md` | reflection การใช้ AI ต้องมีเฉพาะเมื่อใช้ AI |

ใช้หนึ่ง folder ต่อหนึ่ง OJ problem ที่ต้องส่ง learning log

ชื่อ folder ต้องใช้รูปแบบนี้:

```text
oj001
oj002
oj003
...
```

ห้ามใช้รูปแบบชื่อ folder อื่น

---

## 8. Workflow โดยรวมสำหรับ OJ ทุกข้อ

สำหรับ OJ ทุกข้อ ให้ทำตามกระบวนการนี้

### Step 1: อ่านโจทย์ใน OJ

อ่าน problem statement ใน course OJ

อย่าถาม AI ทันที

### Step 2: คิดด้วยตนเองก่อน

ก่อนใช้ AI นักศึกษาต้องคิดด้วยตนเองก่อน

ควรเตรียม note เริ่มต้น เช่น:

```text
Problem understanding:
Input:
Output:
Constraints:
First plan:
```

ยังไม่จำเป็นต้องเป็น code เต็ม

จุดประสงค์คือแสดงว่านักศึกษาพยายามเข้าใจโจทย์และวางแผนก่อนใช้ AI

ถ้าโจทย์ต้องส่ง learning log ต้องเขียนส่วนนี้ใน `submission.md`

### Step 3: เลือก workflow ให้ตรงกับเครื่องมือ AI

ถ้าไม่ใช้ AI ให้เขียน code ใน VS Code ต่อได้เลย

ถ้าใช้ AI ผ่าน browser/chat ให้อ่าน:

```text
workflows/STUDENT_WORKFLOW_WEB_CHAT.md
```

ถ้าใช้ Codex ให้อ่าน:

```text
workflows/STUDENT_WORKFLOW_CHATGPT_CODEX.md
```

ถ้าใช้ Claude Code ให้อ่าน:

```text
workflows/STUDENT_WORKFLOW_CLAUDE_CODE.md
```

ถ้าใช้ AI coding tool อื่นที่ผู้สอนอนุญาต ให้อ่าน:

```text
workflows/STUDENT_WORKFLOW_CODING_TOOLS.md
```

และทำตามคำสั่งเพิ่มเติมจากผู้สอน

### Step 4: เขียน code ใน VS Code

เขียน Python code ใน VS Code

ใช้ pseudocode, flowchart idea หรือ first plan ของตนเองเป็นแนวทาง

### Step 5: ทดสอบในเครื่อง

รัน code ใน VS Code ก่อนส่ง OJ

ตรวจสอบ:

- normal cases
- cases หลายรูปแบบ
- exact output format
- cases ที่พลาดง่าย

### Step 6: ส่งเข้า OJ

ส่ง final code เข้า course OJ

ผล OJ คือผลทางการของความถูกต้อง

### Step 7: ส่ง learning log เฉพาะเมื่อถูกกำหนด

สร้างและ push learning log ไปที่ GitHub repository ของตนเองเฉพาะเมื่อ OJ problem นั้นถูกระบุว่า learning-log required

ถ้าโจทย์ไม่ต้องส่ง learning log ก็ไม่ต้องสร้าง GitHub folder แม้จะใช้ AI ก็ตาม

แต่นักศึกษายังต้องเข้าใจและอธิบาย final code และการใช้ AI ได้เมื่อถูกถาม

---

## 9. ต้องส่งอะไรบ้าง

มีที่ส่งงานได้ 2 ที่:

1. course OJ
2. public GitHub learning log repository ของนักศึกษา

### 9.1 OJ Submission

OJ ทุกข้อที่มอบหมายต้องส่ง final code เข้า course OJ

### 9.2 GitHub Learning Log Submission

ต้องส่ง GitHub learning log เฉพาะ OJ problems ที่ระบุว่า learning-log required

| สถานการณ์ | ส่ง OJ? | ต้องมี GitHub learning log? | ต้องมี `submission.md`? | ต้องมี `ai_reflection.md`? |
|---|---:|---:|---:|---:|
| OJ ปกติ ไม่ใช้ AI | ใช่ | ไม่ | ไม่ | ไม่ |
| OJ ปกติ ใช้ AI | ใช่ | ไม่ | ไม่ | ไม่ |
| OJ ที่ต้องส่ง learning log ไม่ใช้ AI | ใช่ | ใช่ | ใช่ | ไม่ |
| OJ ที่ต้องส่ง learning log ใช้ AI | ใช่ | ใช่ | ใช่ | ใช่ |

กฎสำคัญ:

- GitHub learning log ต้องส่งเฉพาะเมื่อโจทย์ถูกระบุว่า learning-log required
- ทุกโจทย์ที่เป็น learning-log-required ต้องมี `submission.md`
- ถ้าใช้ AI กับโจทย์ learning-log-required ต้องมี `ai_reflection.md`
- สำหรับโจทย์ที่ไม่ใช่ learning-log ไม่ต้องส่ง `submission.md` หรือ `ai_reflection.md` แม้จะใช้ AI
- แต่นักศึกษาอาจถูกสุ่มถามให้อธิบาย problem understanding, algorithm, code, test cases และการใช้ AI

---

## 10. ความรับผิดชอบเมื่อใช้ AI กับโจทย์ที่ไม่ต้องส่ง learning log

นักศึกษาสามารถใช้ AI กับ OJ problems ที่ไม่ได้กำหนด learning log ได้

สำหรับโจทย์เหล่านี้ ไม่ต้องส่ง GitHub learning log

แต่การใช้ AI ไม่ได้ลดความรับผิดชอบของนักศึกษา

นักศึกษาต้องยังอธิบายได้:

1. เข้าใจโจทย์อย่างไร
2. algorithm คืออะไร
3. code ทำงานอย่างไร
4. test cases คืออะไร
5. AI ช่วยอะไร ถ้าใช้ AI
6. ตรวจสอบอะไรด้วยตนเอง

ผู้สอนอาจสุ่มถามให้อธิบาย solution หรือการใช้ AI

ถ้านักศึกษาอธิบาย code ที่ส่งไม่ได้ อาจถือว่างานนั้นไม่แสดงความเข้าใจของนักศึกษาเอง

---

## 11. เมื่อไรต้องใช้ `submission.md`

ใช้:

```text
templates/SUBMISSION_TEMPLATE.md
```

เพื่อสร้างไฟล์ชื่อ:

```text
submission.md
```

อ่านตัวอย่างใน `examples/` ได้ก่อนเขียน แต่ห้าม copy ตัวอย่างเป็นงานของตนเอง

`submission.md` ต้องใช้เฉพาะโจทย์ที่ระบุว่า learning-log required

### ควรเริ่ม `submission.md` เมื่อไร

ให้เริ่มเขียน `submission.md` ก่อนใช้ AI

ถ้าไม่ใช้ AI ให้เริ่มเขียนระหว่างแก้โจทย์ที่ต้องส่ง learning log

ก่อนใช้ AI นักศึกษาต้องกรอกอย่างน้อย:

```text
Problem understanding:
Input:
Output:
Constraints:
First plan:
Independent time spent on this problem:
```

ถ้ายังเข้าใจโจทย์ไม่ครบ ให้เขียนเท่าที่เข้าใจในตอนนั้น

คำตอบอาจยังไม่สมบูรณ์หรืออาจผิดได้ แต่ต้องเป็นความพยายามจริงก่อนใช้ AI

ห้ามเขียนแค่ว่า "not clear yet" ให้เขียนความเข้าใจปัจจุบันที่ดีที่สุด แม้อาจผิดก็ตาม

### ควรจบ `submission.md` เมื่อไร

ให้จบ `submission.md` หลังจาก:

1. เขียน code ใน VS Code
2. ทดสอบในเครื่อง
3. ส่ง OJ ถ้ามีการส่ง
4. รู้ OJ status ปัจจุบัน

### Code ใน `submission.md`

ห้าม copy full code ลงใน `submission.md`

ให้ใช้ OJ submission ID แทน

code ที่ส่งควรตรวจได้ใน OJ

---

## 12. เมื่อไรต้องใช้ `ai_reflection.md`

ใช้:

```text
templates/AI_REFLECTION_TEMPLATE.md
```

เพื่อสร้างไฟล์ชื่อ:

```text
ai_reflection.md
```

`ai_reflection.md` ต้องใช้เฉพาะเมื่อใช้ AI กับโจทย์ที่ต้องส่ง learning log

ถ้าใช้ AI กับโจทย์ที่ไม่ต้องส่ง learning log ไม่ต้องส่ง `ai_reflection.md` แต่ยังต้องเข้าใจและอธิบาย solution ได้เมื่อถูกถาม

`ai_reflection.md` ควรอธิบาย:

1. OJ problem number/title
2. OJ submission ID
3. OJ status
4. ใช้ AI tool อะไร
5. ใช้ไฟล์ instruction ใด เช่น `COURSE_AI_INSTRUCTIONS.md`, `AGENTS.md`, `CLAUDE.md`
6. อ่านและทำตาม workflow ใด
7. ถาม AI ให้ช่วยอะไร
8. AI ช่วยให้สังเกตอะไร
9. ตรวจหรือแก้อะไรด้วยตนเอง
10. ได้เรียนรู้อะไร

reflection ต้องอธิบายกระบวนการจริง

ห้ามให้ AI แต่ง reflection ปลอมแทน

AI อาจช่วยตรวจ grammar, formatting หรือ clarity ได้หลังจากนักศึกษาเขียน reflection เองแล้ว

---

## 13. โครงสร้าง GitHub Repository ของนักศึกษา

นักศึกษาควรสร้าง public GitHub repository หนึ่งอันสำหรับ learning-log-required records

ชื่อ repository ที่แนะนำ:

```text
pscp-ai-learning-log
```

โครงสร้างที่แนะนำ:

```text
pscp-ai-learning-log/
├── README.md
├── oj001/
│   ├── submission.md
│   └── ai_reflection.md
├── oj002/
│   └── submission.md
└── oj003/
    ├── submission.md
    └── ai_reflection.md
```

ใช้หนึ่ง folder ต่อหนึ่ง OJ problem ที่ต้องส่ง learning log

ชื่อ folder ต้องใช้รูปแบบนี้เท่านั้น:

```text
oj001
oj002
oj003
...
```

Repository ควรเป็น public เพื่อให้ผู้สอนตรวจได้สะดวก

แต่ห้ามใส่:

- official OJ problem statements
- official solutions
- hidden test cases
- private data
- access tokens หรือ API keys
- screenshots ที่มีข้อมูลส่วนตัว
- course materials ที่ไม่อนุญาตให้เผยแพร่
- full source code files เช่น `solution.py`

Repository ควรมีเฉพาะ problem-solving records ของนักศึกษาเอง, test cases ของตนเอง, OJ submission references และ AI reflections ของตนเอง

---

## 14. ในแต่ละ Learning Log Folder ควรมีอะไร

แต่ละ learning log folder อาจมี:

| ไฟล์ | ต้องมีเมื่อไร | จุดประสงค์ |
|---|---|---|
| `submission.md` | ต้องมีทุกโจทย์ที่เป็น learning-log-required | บันทึกกระบวนการแก้ปัญหาและ OJ submission reference |
| `ai_reflection.md` | ต้องมีเฉพาะเมื่อใช้ AI กับโจทย์นั้น | reflection ว่า AI ช่วยอะไร และนักศึกษาตรวจสอบอะไรเอง |

ห้ามใส่ `solution.py` ใน GitHub learning log

ให้ใช้ OJ submission ID ใน `submission.md` แทน

### ตัวอย่าง 1: ต้องส่ง Learning Log และไม่ได้ใช้ AI

```text
oj001/
└── submission.md
```

### ตัวอย่าง 2: ต้องส่ง Learning Log และใช้ AI

```text
oj002/
├── submission.md
└── ai_reflection.md
```

### ตัวอย่าง 3: ไม่ต้องส่ง Learning Log

ไม่ต้องมี GitHub folder

ส่งเฉพาะ OJ เท่านั้น

---

## 15. สรุปสุดท้าย

AI ช่วยคิด debug และทดสอบได้

แต่นักศึกษายังต้องรับผิดชอบในการเข้าใจ เขียน ทดสอบ และอธิบาย solution ของตนเอง
