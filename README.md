# 🌿 Lab Assignment: EcoWorld Collaboration

## 📝 สถานการณ์
คุณและเพื่อนต้องสร้าง Landing Page ให้กับโครงการ **"EcoWorld"** ภายในเวลาจำกัด โดยต้องทำงานบน GitHub Repository เดียวกัน แบ่งงานกันทำคนละส่วน และต้องมีการเชิญเพื่อนเข้าทีม (Collaborator)

---

## 👥 การจับคู่และบทบาท (Roles)

### 🟢 Student A (Project Owner)
* **หน้าที่:** สร้าง Repo, เชิญเพื่อน (Invite), ดูแลส่วน **Header**
* **ชื่อ:** Kittituch Thampa รหัส: 1660702885

### 🔵 Student B (Collaborator)
* **หน้าที่:** รับ Invite, เข้าร่วมทีม, ดูแลส่วน **Content & Footer**
* **ชื่อ:** Pattapon Srithaveesinsup รหัส: 1660708536

---

## 🚀 ขั้นตอนการทำงาน (Step-by-Step)

### Phase 1: Setup Team (Student A เริ่มก่อน)
1.  **Student A:** สร้าง Repository ใหม่ชื่อ `lab-ecoworld` (เลือก Public)
2.  **Student A:** ไปที่ Settings -> Collaborators -> **Add people** -> ใส่ Username ของ Student B
3.  **Student B:** เช็ค Email หรือ Notification เพื่อกด **Accept Invite**
4.  **ทั้งคู่:** Clone Repository ลงเครื่องตัวเอง
    * `git clone [URL]`

### Phase 2: Create Base Files (Student A)
1.  **Student A:** นำไฟล์ `index.html` (ที่อาจารย์ให้) ใส่ใน Folder
2.  `git add .` -> `git commit -m "Init Project"` -> `git push`
3.  **Student B:** `git pull` เพื่อดึงไฟล์ลงมา (แล้วแก้ไฟล์ README ใส่ชื่อตัวเอง)

### Phase 3: Coding (ทำพร้อมกัน แยก Branch)
1.  **Student A:**
    * สร้าง Branch: `git checkout -b feature/header`
    * แก้ไข `index.html` ในส่วนบน (ใส่ `<h1>`, `<nav>`)
    * Commit และ Push ขึ้น GitHub
2.  **Student B:**
    * สร้าง Branch: `git checkout -b feature/content`
    * แก้ไข `index.html` ในส่วนเนื้อหา (ใส่ `<h2>`, `<p>`) และ Footer
    * Commit และ Push ขึ้น GitHub

### Phase 4: Merge & Resolve (รวมร่าง)
1.  **Student A:** สร้าง Pull Request (feature/header -> main) และกด **Merge**
2.  **Student B:** สร้าง Pull Request (feature/content -> main)
    * ⚠️ **จะเกิด Conflict** เพราะแก้ไฟล์เดียวกัน
    * ให้กด **Resolve conflicts** บนหน้าเว็บ เลือกรวมโค้ดทั้งสองส่วนเข้าด้วยกัน
    * กด **Mark as resolved** -> **Commit merge** -> **Merge pull request**
3.  **ทั้งคู่:** กลับมาที่เครื่อง สั่ง `git checkout main` และ `git pull` เพื่อดูผลลัพธ์สุดท้าย

---

## ✅ Checklist ส่งงาน
- [ ] Repo มี Collaborator ครบ 2 คน
- [ ] ไฟล์ index.html สมบูรณ์ (มีทั้ง Header และ Content)
- [ ] ประวัติ Commit แสดงให้เห็นว่าต่างคนต่างทำ
