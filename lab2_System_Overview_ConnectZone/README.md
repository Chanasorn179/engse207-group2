# 📌 ConnectZone  
> Community-based Social Media Platform | Designed for Interest Groups

ConnectZone คือแพลตฟอร์ม Social Media ขนาดเล็กที่ออกแบบมาเพื่อสร้าง **ชุมชนเฉพาะกลุ่ม (Interest-based Communities)** เช่น กลุ่มสายแมว, นักเขียนโปรแกรม, ช่างภาพ หรือสายเดินทาง  
แก้ปัญหา Social Network ขนาดใหญ่ที่มี **Feed ปะปนเยอะ** จนผู้ใช้ไม่เห็นเนื้อหาที่สนใจจริงๆ  

ระบบเน้น **ความเรียบง่าย, ใช้งานง่าย, รวดเร็ว, และปลอดภัยของข้อมูล (Privacy-first Design)**

---

## 👥 Target Users

| User Type | Description | Key Permissions |
|-----------|-------------|------------------|
| General User | ผู้ใช้งานทั่วไป | Post / Comment / Like, Join Circles, Follow others |
| Community Moderator | ผู้ดูแลกลุ่ม | Approve Members, Remove Posts, Manage Reports |
| System Administrator | ผู้ดูแลระบบกลาง | Ban Users, Monitor Reports, System Overview |

---

## 🌟 Key Features

### 👤 User Management
- Register / Login / Logout (Email + Password)
- Edit User Profile (Name, Bio, Profile Picture)
- Change Password
- Follow Users

---

### 📝 Content & Post
- Create Post (Text + Images ≤ 4 files)
- Edit/Delete own post
- Like / Unlike
- Comment on posts
- Privacy Settings (Public / Friends / Private)

---

### 🔄 Social Interaction & Community
- Create Circle (Group)
- Public / Private Group
- Join Group / Request Membership
- Content Moderation (Report, Ban, Remove content)

---

### 🔔 System Features
- Notification (Likes, Comments, Group Updates)
- Search (User, Post, Circle)
- Report & Flag Content
- Moderator Panel / Admin Dashboard

---

## 📋 Functional Requirements

| ID | Requirement Description |
|----|-------------------------|
| FR-01 | Register via Email + Password |
| FR-02 | User Login/Logout securely |
| FR-03 | Edit Profile (Name, Bio, Picture) |
| FR-04 | Change Password |
| FR-05 | Create Post (text + image) |
| FR-06 | Edit/Delete own post |
| FR-07 | Like/Unlike posts |
| FR-08 | Comment on post |
| FR-09 | Follow other users |
| FR-10 | Create Circle (Group) |
| FR-11 | Request to join Private group |
| FR-12 | Search users/groups |
| FR-13 | Notification system |
| FR-14 | Moderator/Admin can Ban users |
| FR-15 | Hide flagged content until reviewed |

---

## ⚙️ Quality Attributes (Non-Functional Requirements)

| Attribute | Scenario | Acceptance Criteria |
|-----------|----------|----------------------|
| Performance | เปิดหน้า News Feed | โหลด ≤ 2 sec |
| Scalability | Viral Event (3x Traffic) | Auto-Scale, Error < 1% |
| Security | Hacker เข้าหน้า Admin | Block (403), Log 100% |
| Availability | Server ล่ม 1 ตัว | Downtime < 1 min |
| Usability | ผู้ใช้ใหม่โพสต์รูปแรก | ≤ 3 คลิก หรือ <1 นาที |
| Modifiability | เพิ่มฟีเจอร์ Reaction | Deploy ได้ใน 3 วัน |

---

## ⛓️ Constraints

### 🛠️ Technical  
- รองรับ **Responsive Web App** (Mobile + Desktop)  
- สถาปัตยกรรม: **Microservices** หรือ **Modular Monolith**  
- Database ใช้ **PostgreSQL (User/Auth)** และ **MongoDB (Post/Feed)**

### ⏳ Time & Budget  
- MVP ภายใน **12 สัปดาห์ (1 เทอม)**  
- Cloud Budget ไม่เกิน **3,000 บาท/เดือน**

### ⚖ Legal / Policy  
- ต้องปฏิบัติตาม PDPA 🇹🇭  
- ระบบต้องมี Content Copyright Protection  

---

## 🧠 Key Decisions (Trade-offs)

### 1️⃣ Performance vs Security  
✦ Encryption ช่วยเพิ่ม Security แต่กระทบ Speed  
✔ ตัดสินใจ: Encrypt เฉพาะ Password และ Personal Data → Balance ระหว่าง Speed และ Security

### 2️⃣ Usability vs Authentication Security  
✦ 2FA & Password Complexity → ปลอดภัยมาก แต่ผู้ใช้รำคาญ  
✔ ตัดสินใจ: ให้ใช้งานง่าย (จำ Session, ไม่บังคับ 2FA สำหรับผู้ใช้ทั่วไป)

---

## 🏗 Recommended Architecture

```bash
[Frontend] React / Next.js
↓ API Gateway
[Auth Service] — JWT, Security
↓
[User Service] — PostgreSQL
[Feed Service] — MongoDB
[Circle Service]
[Notification Service]
[Moderation Service]
```

---


## ✨ Contributors

| รหัสนักศึกษา | ชื่อ-นามสกุล | Role |
| :--- | :--- | :--- |
| **67543210025-2** | นาย ชนสรณ์ บุตรถา | Dev A (Frontend) |
| **67543210033-6** | นาย ธาวัน ทิพคุณ | Dev B (Backend) |
| **67543210049-2** | นาย อติโรจน์ กุหลั่น | Team Leader |
| **67543210071-6** | นาย เบญจศรายุทธ น้อยอุบล | Tester |

---

> ⭐ _“Connect people, build communities, and empower interests.”_  
> 🚀 Developed with passion for real-world problem solving.


