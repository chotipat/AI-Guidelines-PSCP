# แนวทางการใช้ AI สำหรับวิชา PSCP

Repository นี้จัดทำขึ้นเพื่ออธิบายแนวทางและ template สำหรับการใช้ AI อย่างรับผิดชอบในวิชา Problem Solving and Computer Programming ของ IT KMITL

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
- ผู้ช่วยสร้าง test cases
- ผู้ช่วยปรับ reflection

AI ต้องไม่ถูกใช้แทนความคิดของนักศึกษา

เป้าหมายหลักคือช่วยให้นักศึกษาพัฒนาทักษะการแก้ปัญหาและการเขียนโปรแกรม ไม่ใช่เพียงเพื่อให้ได้คำตอบ Accepted จาก OJ

---

## 2. ไฟล์ใน Repository นี้

| ไฟล์ | จุดประสงค์ |
|---|---|
| `README.md` | นโยบายหลักและกติกาการส่งงานของรายวิชา |
| `README.th.md` | README ภาษาไทยของนโยบายหลักและกติกาการส่งงานของรายวิชา |
| `instructions/COURSE_AI_INSTRUCTIONS.md` | คำสั่งหลักสำหรับ AI coach เช่น ChatGPT, Claude, Gemini web chat และเครื่องมือ AI ที่คล้ายกัน |
| `instructions/AGENTS.md` | กฎกลางของรายวิชาสำหรับ coding agents โดย Codex สามารถใช้ไฟล์นี้ได้โดยตรง |
| `instructions/CLAUDE.md` | Claude Code instruction wrapper ที่พร้อมใช้ ให้ copy ไฟล์นี้พร้อมกับ `instructions/AGENTS.md` ไปไว้ใน `pscp/` ก่อนใช้ Claude Code |
| `workflows/STUDENT_WORKFLOW_WEB_CHAT.md` | Workflow สำหรับ AI tools ที่ใช้ผ่าน browser หรือ chat interface |
| `workflows/STUDENT_WORKFLOW_WEB_CHAT.th.md` | Workflow ภาษาไทยสำหรับ AI tools ที่ใช้ผ่าน browser หรือ chat interface |
| `workflows/STUDENT_WORKFLOW_CHATGPT_CODEX.md` | Workflow เฉพาะสำหรับ ChatGPT Codex, OpenAI Codex, Codex CLI และการใช้ Codex app แบบ optional |
| `workflows/STUDENT_WORKFLOW_CHATGPT_CODEX.th.md` | Workflow ภาษาไทยเฉพาะสำหรับ ChatGPT Codex, OpenAI Codex, Codex CLI และการใช้ Codex app แบบ optional |
| `workflows/STUDENT_WORKFLOW_CLAUDE_CODE.md` | Workflow เฉพาะสำหรับ Claude Code CLI และการใช้ Claude desktop app / Claude Cowork แบบ optional |
| `workflows/STUDENT_WORKFLOW_CLAUDE_CODE.th.md` | Workflow ภาษาไทยเฉพาะสำหรับ Claude Code CLI และการใช้ Claude desktop app / Claude Cowork แบบ optional |
| `templates/SUBMISSION_TEMPLATE.md` | Template เปล่าสำหรับสร้าง `submission.md` ใช้เฉพาะโจทย์ OJ ที่กำหนดให้ส่ง learning log |
| `templates/AI_REFLECTION_TEMPLATE.md` | Template เปล่าสำหรับสร้าง `ai_reflection.md` ใช้เฉพาะเมื่อมีการใช้ AI กับโจทย์ที่ต้องส่ง learning log |
| `examples/SUBMISSION_TEMPLATE_sample_no_AI.md` | ตัวอย่าง `submission.md` ที่เขียนเสร็จแล้ว เมื่อไม่ได้ใช้ AI |
| `examples/SUBMISSION_TEMPLATE_sample_AI.md` | ตัวอย่าง `submission.md` ที่เขียนเสร็จแล้ว เมื่อใช้ AI |
| `examples/AI_REFLECTION_TEMPLATE_sample.md` | ตัวอย่าง `ai_reflection.md` ที่เขียนเสร็จแล้ว |
| `examples/SUBMISSION_TEMPLATE_sample_no_AI.th.md` | ตัวอย่างภาษาไทยของ `submission.md` เมื่อไม่ได้ใช้ AI |
| `examples/SUBMISSION_TEMPLATE_sample_AI.th.md` | ตัวอย่างภาษาไทยของ `submission.md` เมื่อใช้ AI |
| `examples/AI_REFLECTION_TEMPLATE_sample.th.md` | ตัวอย่างภาษาไทยของ `ai_reflection.md` ที่เขียนเสร็จแล้ว |

ให้อ่าน `README.md` หรือ `README.th.md` ก่อน

ใช้ `templates/SUBMISSION_TEMPLATE.md` เพื่อสร้าง `submission.md` ของตนเอง

ใช้ `templates/AI_REFLECTION_TEMPLATE.md` เพื่อสร้าง `ai_reflection.md` ของตนเอง เมื่อใช้ AI กับโจทย์ที่ต้องส่ง learning log

สามารถอ่านตัวอย่างใน `examples/` เพื่อดูระดับรายละเอียดที่คาดหวังได้ แต่ห้ามคัดลอกเนื้อหาตัวอย่างไปเป็นงานของตนเอง

ไฟล์ `.th.md` ภาษาไทยมีให้สำหรับ README, เอกสาร workflow และตัวอย่าง

ไฟล์ instruction ภาษาอังกฤษยังคงเป็นไฟล์หลักสำหรับ AI tools และ coding agents

---

## 3. นโยบาย Editor ทางการ

VS Code คือ editor ทางการของรายวิชานี้

นักศึกษาต้องใช้ VS Code สำหรับ:

- เขียนโค้ด Python
- รันโค้ด Python
- ทดสอบโค้ดในเครื่อง
- เตรียมโค้ดสุดท้ายก่อนส่งเข้า OJ

เครื่องมือ AI อาจใช้ได้เฉพาะในฐานะผู้ช่วยภายใต้นโยบายการใช้ AI ของรายวิชา

AI-first editors เช่น Cursor ไม่ใช่ workflow ทางการ เว้นแต่ผู้สอนอนุญาตอย่างชัดเจน

ถ้าผู้สอนไม่ได้อนุญาต editor อื่นอย่างชัดเจน นักศึกษาควรใช้ VS Code เท่านั้น

---

## 4. ควรอ่าน Workflow ไหน

ให้เลือก workflow ตามลักษณะการใช้ AI ไม่ใช่ตามว่า account เป็น free หรือ paid

| ถ้าใช้... | ให้อ่าน workflow นี้ |
|---|---|
| ChatGPT, Claude, Gemini หรือ AI อื่นผ่าน browser/chat interface | `workflows/STUDENT_WORKFLOW_WEB_CHAT.md` |
| ChatGPT Codex, OpenAI Codex, Codex CLI หรือ Codex app | `workflows/STUDENT_WORKFLOW_CHATGPT_CODEX.md` |
| Claude Code CLI หรือ Claude desktop app / Claude Cowork หากผู้สอนอนุญาตอย่างชัดเจน | `workflows/STUDENT_WORKFLOW_CLAUDE_CODE.md` |

ข้อสำคัญ:

- Free หรือ paid account ไม่ใช่ประเด็นหลัก
- ประเด็นหลักคือ AI ถูกใช้เป็น chat assistant เท่านั้น หรือสามารถทำงานใน coding environment ได้
- ถ้า AI อ่านไฟล์ แก้โค้ด รันคำสั่ง หรือเสนอ code changes โดยตรงใน VS Code หรือ terminal ได้ ให้ถือว่าเป็น coding tool
- GitHub Copilot ใน VS Code และ VS Code AI extensions อื่น ๆ ไม่ใช่ workflow ทางการ เว้นแต่ผู้สอนอนุญาตอย่างชัดเจน
- Cursor และ AI-first editors อื่น ๆ ไม่ใช่ workflow ทางการ เว้นแต่ผู้สอนอนุญาตอย่างชัดเจน เพราะ VS Code เป็น editor ที่รายวิชากำหนดให้ใช้

AI coding tools อื่น ๆ, VS Code AI extensions และ AI-first editors ไม่อยู่ใน workflow ของรายวิชา เว้นแต่ผู้สอนประกาศ workflow เพิ่มเติมแยกต่างหาก

---

## 5. หมายเหตุสั้นสำหรับเครื่องมือเฉพาะ

รายละเอียดการ setup และกติกาการใช้งานอยู่ในไฟล์ workflow ของแต่ละเครื่องมือ

ให้อ่าน workflow ที่ถูกต้องก่อนใช้แต่ละเครื่องมือ

### Codex

ถ้าใช้ ChatGPT Codex, OpenAI Codex, Codex CLI หรือ Codex app ให้อ่าน:

```text
workflows/STUDENT_WORKFLOW_CHATGPT_CODEX.md
```

สำหรับ Codex CLI workflow ที่แนะนำในรายวิชาคือ:

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

สำหรับ Claude Code CLI workflow ที่แนะนำในรายวิชาคือ:

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

### เครื่องมือที่ไม่อยู่ใน Workflow ของรายวิชา

AI coding tools อื่น ๆ, VS Code AI extensions และ AI-first editors ไม่อยู่ใน workflow ของรายวิชา เว้นแต่ผู้สอนประกาศ workflow เพิ่มเติมแยกต่างหาก

VS Code ยังคงเป็น editor ทางการ

OJ ของรายวิชายังคงเป็นที่ส่ง code อย่างเป็นทางการ

---

## 6. สิ่งที่นักศึกษาต้องเขียนเอง

ส่วนต่อไปนี้ต้องเขียนโดยนักศึกษาเอง AI อาจช่วย review, ถามคำถาม หรือให้ข้อเสนอแนะได้ แต่ AI ต้องไม่เขียนส่วนเหล่านี้แทนนักศึกษาเพื่อส่งงาน

นักศึกษาต้องเขียนเอง:

1. ความเข้าใจโจทย์ของตนเอง
2. การวิเคราะห์ input, output และ constraints
3. pseudocode, flowchart idea หรือ first plan เริ่มต้น
4. คำอธิบาย algorithm ของตนเอง
5. final code ที่ส่งเข้า OJ ซึ่งนักศึกษาเข้าใจและอธิบายได้
6. test cases และ test results ของตนเอง
7. `submission.md` ของตนเอง เมื่อโจทย์ OJ เป็น learning-log-required
8. `ai_reflection.md` ของตนเอง เมื่อมีการใช้ AI กับโจทย์ที่เป็น learning-log-required

นักศึกษาห้ามส่ง:

- code ที่ AI สร้างและนักศึกษาอธิบายไม่ได้
- problem analysis ที่คัดลอกจาก AI โดยตรงโดยไม่ปรับและไม่เข้าใจ
- reflection ที่ AI สร้างซึ่งไม่อธิบายกระบวนการจริงของนักศึกษา
- pseudocode ที่คัดลอกจาก AI โดยไม่เข้าใจ
- AI reflection ปลอม
- testing results ปลอม
- OJ results ปลอม

นักศึกษาไม่ต้องส่ง AI conversation ทั้งหมด

อย่างไรก็ตาม เมื่อติดต่อกับ AI นักศึกษาต้องเขียนคำถามของตนเอง อธิบายโจทย์ด้วยภาษาของตนเอง ให้ first plan ของตนเอง และตรวจสอบคำแนะนำของ AI ด้วยตนเอง

นักศึกษารับผิดชอบคำตอบสุดท้าย โค้ดสุดท้าย OJ submission และการอธิบายทั้งหมด

---

## 7. Learning Log คืออะไร

Learning log คือ GitHub folder สำหรับ OJ problem หนึ่งข้อที่ผู้สอนหรือ OJ ระบุว่าเป็น learning-log-required

Learning log บันทึกกระบวนการแก้ปัญหาของนักศึกษา และถ้ามีการใช้ AI กับโจทย์ที่เป็น learning-log-required ก็ให้บันทึก reflection การใช้ AI ของนักศึกษาด้วย

Learning log อาจมี:

| ไฟล์ | ความหมาย |
|---|---|
| `submission.md` | บันทึกกระบวนการแก้ปัญหาของนักศึกษา |
| `ai_reflection.md` | reflection ของนักศึกษาเกี่ยวกับการใช้ AI ต้องมีเฉพาะเมื่อใช้ AI |

ใช้หนึ่ง folder ต่อหนึ่ง OJ problem ที่เป็น learning-log-required

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

สำหรับ OJ ทุกข้อที่ได้รับมอบหมาย ให้ทำตามกระบวนการโดยรวมนี้

### Step 1: อ่านโจทย์ OJ

อ่าน problem statement ใน course OJ

อย่าถาม AI ทันที

### Step 2: คิดด้วยตนเองก่อน

ก่อนใช้ AI นักศึกษาต้องคิดด้วยตนเองก่อน

นักศึกษาควรเตรียม note การแก้ปัญหาเริ่มต้นของตนเอง ซึ่งอาจมี:

```text
Problem understanding:
Input:
Output:
Constraints:
First plan:
```

ส่วนนี้ยังไม่จำเป็นต้องเป็นโค้ดเต็ม

การเขียนโค้ดในขั้นนี้เป็น optional

จุดประสงค์ของขั้นนี้คือแสดงว่านักศึกษาพยายามเข้าใจโจทย์และวางแผนการแก้ปัญหาก่อนใช้ AI

ถ้าโจทย์เป็น learning-log-required ต้องเขียนความคิดเริ่มต้นนี้ใน `submission.md`

### Step 3: เลือก AI Workflow ให้ถูกต้อง ถ้ามีการใช้ AI

ถ้านักศึกษาไม่ใช้ AI ให้เขียนโค้ดต่อใน VS Code

ถ้านักศึกษาใช้ AI ผ่าน browser/chat interface ให้ทำตาม:

```text
workflows/STUDENT_WORKFLOW_WEB_CHAT.md
```

ถ้านักศึกษาใช้ Codex ให้ทำตาม:

```text
workflows/STUDENT_WORKFLOW_CHATGPT_CODEX.md
```

ถ้านักศึกษาใช้ Claude Code ให้ทำตาม:

```text
workflows/STUDENT_WORKFLOW_CLAUDE_CODE.md
```

AI coding tools อื่น ๆ ไม่อยู่ใน workflow ของรายวิชา เว้นแต่ผู้สอนประกาศ workflow เพิ่มเติมแยกต่างหาก

### Step 4: เขียนโค้ดใน VS Code

เขียน Python code ใน VS Code

ใช้ pseudocode, flowchart idea หรือ first plan ของตนเองเป็นแนวทาง

### Step 5: ทดสอบในเครื่อง

รันโค้ดใน VS Code ก่อนส่งเข้า OJ

ตรวจสอบ:

- normal cases
- cases หลายประเภท
- exact output format
- cases ที่อาจพลาดง่าย

### Step 6: ส่งเข้า OJ

ส่ง final code เข้า course OJ

ผล OJ คือผลทางการด้านความถูกต้อง

### Step 7: ส่ง Learning Log เฉพาะเมื่อถูกกำหนด

สร้างและ push learning log ไปยัง GitHub repository ของตนเองเฉพาะเมื่อ OJ problem นั้นถูกระบุว่าเป็น learning-log-required

ถ้าโจทย์ไม่ใช่ learning-log-required ไม่ต้องส่ง GitHub learning log แม้จะใช้ AI ก็ตาม

อย่างไรก็ตาม นักศึกษายังต้องรับผิดชอบในการเข้าใจและอธิบาย final code และการใช้ AI ของตนเองเมื่อถูกถาม

---

## 9. ต้องส่งอะไรบ้าง

มีที่ส่งงานได้ 2 ที่:

1. course OJ
2. public GitHub learning log repository ของนักศึกษา

### 9.1 OJ Submission

สำหรับ OJ problem ทุกข้อที่ได้รับมอบหมาย นักศึกษาต้องส่ง final code เข้า course OJ

### 9.2 GitHub Learning Log Submission

นักศึกษาต้องส่ง GitHub learning log เฉพาะ OJ problems ที่ถูกระบุว่าเป็น learning-log-required

| สถานการณ์ | ส่ง OJ? | ต้องมี GitHub learning log? | ต้องมี `submission.md`? | ต้องมี `ai_reflection.md`? |
|---|---:|---:|---:|---:|
| OJ ปกติ ไม่ใช้ AI | ใช่ | ไม่ | ไม่ | ไม่ |
| OJ ปกติ ใช้ AI | ใช่ | ไม่ | ไม่ | ไม่ |
| OJ ที่เป็น learning-log-required ไม่ใช้ AI | ใช่ | ใช่ | ใช่ | ไม่ |
| OJ ที่เป็น learning-log-required ใช้ AI | ใช่ | ใช่ | ใช่ | ใช่ |

กฎสำคัญ:

- GitHub learning log ต้องส่งเฉพาะเมื่อ OJ problem ถูกระบุว่าเป็น learning-log-required
- สำหรับทุก learning-log-required problem นักศึกษาต้องส่ง `submission.md`
- ถ้าใช้ AI กับ learning-log-required problem นักศึกษาต้องส่ง `ai_reflection.md` ด้วย
- สำหรับ non-learning-log problems นักศึกษาไม่ต้องส่ง `submission.md` หรือ `ai_reflection.md` แม้จะใช้ AI
- อย่างไรก็ตาม นักศึกษาอาจถูกสุ่มถามให้อธิบาย problem understanding, algorithm, code, test cases และการใช้ AI

---

## 10. ความรับผิดชอบเมื่อใช้ AI กับโจทย์ที่ไม่ต้องส่ง Learning Log

นักศึกษาสามารถใช้ AI กับ OJ problems ที่ไม่ได้ถูกระบุว่าเป็น learning-log-required ได้

สำหรับโจทย์เหล่านี้ นักศึกษาไม่ต้องส่ง GitHub learning log

อย่างไรก็ตาม การใช้ AI ไม่ได้ลดความรับผิดชอบของนักศึกษา

นักศึกษาต้องยังสามารถอธิบายได้ว่า:

1. เข้าใจโจทย์อย่างไร
2. algorithm คืออะไร
3. code ทำงานอย่างไร
4. test cases คืออะไร
5. AI ช่วยอย่างไร ถ้ามีการใช้ AI
6. นักศึกษาตรวจสอบอะไรด้วยตนเอง

ผู้สอนอาจสุ่มถามให้นักศึกษาอธิบาย solution หรือการใช้ AI

ถ้านักศึกษาอธิบาย code ที่ส่งไม่ได้ อาจถือว่าการส่งนั้นไม่ได้แสดงความเข้าใจของนักศึกษาเอง

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

นักศึกษาอาจอ่านตัวอย่างใน `examples/` ก่อนเขียน `submission.md` ของตนเอง

ห้ามคัดลอกเนื้อหาตัวอย่างไปเป็นงานของตนเอง

`submission.md` ต้องใช้เฉพาะเมื่อ OJ problem ถูกระบุว่าเป็น learning-log-required

### ควรเริ่ม `submission.md` เมื่อไร

ให้เริ่มเขียน `submission.md` ก่อนใช้ AI

ถ้าไม่ใช้ AI ให้เริ่มเขียน `submission.md` ระหว่างแก้โจทย์ที่เป็น learning-log-required

ก่อนใช้ AI นักศึกษาต้องกรอกอย่างน้อย:

```text
Problem understanding:
Input:
Output:
Constraints:
First plan:
Independent time spent on this problem:
```

ถ้านักศึกษายังเข้าใจโจทย์ไม่ครบ ต้องเขียนสิ่งที่ตนเองเข้าใจในตอนนั้น

คำตอบอาจยังไม่สมบูรณ์หรืออาจผิดได้ แต่นักศึกษาต้องพยายามด้วยตนเองอย่างจริงใจก่อนใช้ AI

ห้ามเขียนแค่ "not clear yet" ให้เขียนความเข้าใจปัจจุบันที่ดีที่สุด แม้อาจผิดก็ตาม

### ควรจบ `submission.md` เมื่อไร

ให้จบ `submission.md` หลังจาก:

1. เขียนโค้ดใน VS Code
2. ทดสอบในเครื่อง
3. ส่ง OJ ถ้ามีการส่ง
4. รู้ OJ status ปัจจุบัน

### Code ใน `submission.md`

ห้ามคัดลอกโค้ดเต็มลงใน `submission.md`

ให้ใช้ OJ submission ID แทน

โค้ดที่ส่งควรตรวจสอบได้ใน OJ

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

`ai_reflection.md` ต้องใช้เฉพาะเมื่อมีการใช้ AI กับโจทย์ที่เป็น learning-log-required

ถ้าใช้ AI กับ non-learning-log problem ไม่ต้องส่ง `ai_reflection.md` แต่นักศึกษายังต้องเข้าใจและอธิบาย solution ได้เมื่อถูกถาม

`ai_reflection.md` ควรอธิบาย:

1. OJ problem number/title
2. OJ submission ID
3. OJ status
4. ใช้ AI tool ใด
5. ใช้ `instructions/COURSE_AI_INSTRUCTIONS.md`, `instructions/AGENTS.md`, `instructions/CLAUDE.md` หรือไฟล์ instruction อื่นที่ได้รับอนุญาตหรือไม่
6. อ่านและทำตาม workflow ที่เกี่ยวข้องหรือไม่
7. ถาม AI ให้ช่วยอะไร
8. AI ช่วยให้สังเกตอะไร
9. นักศึกษาตรวจหรือแก้อะไรด้วยตนเอง
10. นักศึกษาได้เรียนรู้อะไร

Reflection ต้องอธิบายกระบวนการจริงของนักศึกษา

ห้ามให้ AI แต่ง reflection แทน

AI อาจช่วยเรื่อง grammar, formatting หรือ clarity ได้หลังจากนักศึกษาเขียน reflection เองแล้ว

---

## 13. โครงสร้าง GitHub Repository ที่แนะนำสำหรับนักศึกษา

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

ใช้หนึ่ง folder ต่อหนึ่ง OJ problem ที่เป็น learning-log-required

ชื่อ folder ต้องใช้รูปแบบนี้เท่านั้น:

```text
oj001
oj002
oj003
...
```

Repository ควรเป็น public เพื่อให้ผู้สอนตรวจได้สะดวก

อย่างไรก็ตาม นักศึกษาห้ามใส่:

- official OJ problem statements
- official solutions
- hidden test cases
- private data
- access tokens หรือ API keys
- screenshots ที่มีข้อมูลส่วนตัว
- course materials ที่ไม่อนุญาตให้เผยแพร่ซ้ำ
- full source code files เช่น `solution.py`

Repository ควรมีเฉพาะ problem-solving records ของนักศึกษาเอง, test cases ของนักศึกษาเอง, OJ submission references ของนักศึกษาเอง และ AI reflections ของนักศึกษาเอง

---

## 14. ควรใส่อะไรในแต่ละ Learning Log Folder

แต่ละ learning log folder อาจมี:

| ไฟล์ | ต้องมีเมื่อไร | จุดประสงค์ |
|---|---|---|
| `submission.md` | ต้องมีทุก learning-log-required problem | บันทึกกระบวนการแก้ปัญหาและ OJ submission reference |
| `ai_reflection.md` | ต้องมีเฉพาะเมื่อใช้ AI กับ learning-log-required problem นั้น | Reflection ว่า AI ช่วยอย่างไร และนักศึกษาตรวจสอบอะไรด้วยตนเอง |

ห้ามใส่ `solution.py` ใน GitHub learning log

ให้ใช้ OJ submission ID ใน `submission.md` แทน

### ตัวอย่าง 1: Learning Log Required, ไม่ใช้ AI

```text
oj001/
└── submission.md
```

### ตัวอย่าง 2: Learning Log Required, ใช้ AI

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

AI ช่วยให้คิด debug และ test ได้

แต่นักศึกษายังคงรับผิดชอบในการเข้าใจ เขียน ทดสอบ และอธิบาย solution ของตนเอง
