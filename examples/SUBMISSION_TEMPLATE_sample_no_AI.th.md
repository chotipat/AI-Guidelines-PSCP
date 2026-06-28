# submission.md

## 1. OJ Information

- OJ problem number: oj001
- OJ problem title: Sum of Two Numbers
- OJ submission ID: 123456
- OJ status: Accepted

---

## 2. Independent Work Before AI

- เวลาที่ใช้คิดเองก่อนใช้ AI: ไม่ได้ใช้ AI
- สิ่งที่เข้าใจจากโจทย์: รับจำนวนเต็มสองจำนวน แล้วแสดงผลรวม
- Input: จำนวนเต็มสองจำนวน
- Output: ผลรวมของสองจำนวน
- Constraints: ค่าอยู่ในช่วงที่ Python int รองรับได้
- First plan: อ่าน input แปลงเป็น int บวกกัน แล้ว print ผลลัพธ์

---

## 3. Final Approach

ใช้ `input().split()` เพื่อแยกตัวเลขสองตัว แปลงเป็น integer แล้วนำมาบวกกัน จากนั้นแสดงผลรวม

---

## 4. Test Cases

### Test Case 1

- เหตุผลที่เลือก: case ปกติ
- Input: `2 3`
- Expected output: `5`
- Actual output: `5`
- Result: Passed

### Test Case 2

- เหตุผลที่เลือก: มีเลขศูนย์
- Input: `0 7`
- Expected output: `7`
- Actual output: `7`
- Result: Passed

### Test Case 3

- เหตุผลที่เลือก: มีเลขลบ
- Input: `-2 5`
- Expected output: `3`
- Actual output: `3`
- Result: Passed

---

## 5. What I Learned

ได้ฝึกการอ่าน input หลายค่าจากบรรทัดเดียว และการตรวจ test cases พื้นฐาน
