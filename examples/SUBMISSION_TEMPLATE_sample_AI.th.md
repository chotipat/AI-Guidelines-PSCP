# submission.md

## 1. OJ Information

- OJ problem number: oj002
- OJ problem title: Count Even Numbers
- OJ submission ID: 234567
- OJ status: Accepted

---

## 2. Independent Work Before AI

- เวลาที่ใช้คิดเองก่อนใช้ AI: 15 นาที
- สิ่งที่เข้าใจจากโจทย์: รับจำนวน n และ list ของจำนวนเต็ม n ตัว แล้วนับว่ามีกี่ตัวที่เป็นเลขคู่
- Input: บรรทัดแรกเป็น n บรรทัดถัดไปเป็นจำนวนเต็ม n ตัว
- Output: จำนวนเลขคู่
- Constraints: n เป็นจำนวนเต็มบวก
- First plan: loop ผ่านตัวเลขทั้งหมด ถ้า `x % 2 == 0` ให้เพิ่ม counter

---

## 3. Final Approach

อ่านค่า n และ list ของตัวเลข จากนั้นวนลูปนับจำนวนที่หารด้วย 2 ลงตัว แล้วแสดงผล counter

---

## 4. Test Cases

### Test Case 1

- เหตุผลที่เลือก: มีทั้งเลขคู่และเลขคี่
- Input: `5` และ `1 2 3 4 5`
- Expected output: `2`
- Actual output: `2`
- Result: Passed

### Test Case 2

- เหตุผลที่เลือก: ทุกตัวเป็นเลขคู่
- Input: `4` และ `2 4 6 8`
- Expected output: `4`
- Actual output: `4`
- Result: Passed

### Test Case 3

- เหตุผลที่เลือก: ไม่มีเลขคู่
- Input: `3` และ `1 3 5`
- Expected output: `0`
- Actual output: `0`
- Result: Passed

---

## 5. What I Learned

ได้เรียนรู้ว่าควรคิด edge cases เช่น ไม่มีเลขคู่ หรือทุกตัวเป็นเลขคู่ ก่อนส่ง OJ
