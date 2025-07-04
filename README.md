# 📘 Peer Tutoring Management System

A fully functional web based Peer Tutoring Management System. 
This platform connects students who need help in academic subjects with peer tutors from the same school.
**Please Note: Please Note: This platform is only a prototype and not currently in use at any school.**

🔗 **Live Demo**: [https://peer-tutoring-management-system.onrender.com](https://peer-tutoring-management-system.onrender.com)  
⚠️ Note: The site may take up to **90 seconds to load** as it's deployed on a free Render instance.

----

## 📚 Features

  - Student & Tutor form submissions
  - Automated matchmaking algorithm based on:
  - Subject compatibility
  - Grade level
  - Period availability
  - Subject specialization (e.g. University > Mixed > College)
  - Email notifications:
  - Successful match confirmations
  - Standby status for unmatched users
  - Notifications on match removals
  - Secure login for school guidance staff
  - Matches dashboard with:
  - Match details
  - Remove options (student, tutor, both)
  - Seasonal Easter Eggs (e.g. Christmas, Halloween)

---

## 🏠 Landing Page

Upon visiting the platform, users can access:

- **Student Form**
- **Tutor Form**
- **Guidance Entry Login** for staff

🔁 Each visit features a random inspirational quote about education.  
📱 The UI adapts for mobile and small screens using a responsive design.

---

## 📝 Form Pages

Users (students or tutors) must provide:

- Full Name
- Email
- Phone Number
- School
- Grade
- Free Period
- Subject (from supported list)

### 🏫 Supported Schools (Examples)

- Alexander Mackenzie High School
- Bayview Secondary School
- Unionville High School  
_(and many more...)_

### 📖 Supported Subjects

#### Math:
- MCR3U, MAP4C, MBF3C, MPM2D, MTH1W

#### English:
- NBE3U/C, ENG2D, ENL1W

#### Science:
- SPH3U, SBI3U/C, SNC2D, SNC1W

#### Others:
- Computer Science, Business, History, Geography, French
_(and many more...)_

---

## 🔗 Matchmaking Logic

- Matches students and tutors from the **same school**
- Ensures **same subject or subject category**
- Compares course **type (University > Mixed > College)**
- Periods must align
- Science subjects use a custom logic to ensure correct discipline
- Grade 11+ tutors can assist students from lower grades

---

## ✉️ Email Notifications

The system sends automatic emails for:

- ✅ Successful matches
- ⏳ Pending/Standby notices
- 🔁 Changes in match status
- ❌ Removals from sessions

> ⚠️ If a user doesn’t receive an email, they may have entered the wrong address. Supervisors should be contacted to resolve.

---

## 🎉 Easter Eggs

Icons are displayed for seasonal and cultural events:

| Date(s)               | Occasion                      | Icon |
|-----------------------|-------------------------------|------|
| Jan 21 – Feb 21       | Chinese New Year              | 🐉   |
| Feb 14                | Valentine's Day               | ❤️    |
| Mar 19 – Mar 22       | Persian New Year              | 💚🤍❤️ |
| Apr 14 – Apr 22       | Earth Week                    | 🌎   |
| May 5 – May 7         | Teacher Appreciation          | 🍎   |
| July 1                | Canada Day                    | 🍁   |
| Oct 31                | Halloween                     | 🎃   |
| Nov 11                | Remembrance Day               | 🌺   |
| Dec 25 – Jan 7        | Holiday Season (Christmas)    | 🎄   |

---

## 🔐 Guidance Entry (Admin Panel)

Accessible from the landing page, this portal allows authorized staff to:

- Log in with a **School Code** and **6-digit PIN** (`220244`)

  (Please Note: In order to receive your school code, please contact the author. A valid staff ID will be required).
- View all current matches for their school
- Remove matches using:
  - Remove Student
  - Remove Tutor
  - Remove Match
  - Remove Both

Each removal triggers an appropriate email to the student and tutor.

---

## 🧪 Testing Methodology

The Peer Tutoring Management System has been tested against the following scenarios to ensure reliable operation:

- ✅ Tutor and student **should match** if:
  - They are from the **same school**
  - They are available in the **same period**
  - They selected the **same course** or a compatible one
  - The tutor is taking a **higher or equivalent level** course than the student

- ❌ Tutor and student **should not match** if:
  - They are from **different schools**
  - They selected **different periods**

- 🧬 Science-specific logic:
  - Physics, Biology, and Chemistry must match by discipline and level
  - Grade 11 tutors can help students from Grades 9–10 in science subjects

- 📬 Email logic:
  - Emails are sent on **successful match**
  - “Standby” emails are sent if no match is found
  - Notifications are sent when a match is **modified or removed**

- 🔐 Admin login:
  - Login is **restricted** to authorized staff using valid school code and 6-digit code

- 🗑️ Remove functionality:
  - Remove Student: Student removed, tutor retained
  - Remove Tutor: Tutor removed, student waits for new tutor
  - Remove Match: Breaks the match, both remain in the system
  - Remove Both: Deletes student and tutor entries entirely

- 🖱️ UI/UX:
  - All buttons function as expected
  - Page navigation and logo redirection tested

---

## 📄 License

This project was developed for **educational purposes** by students at YRDSB.

- You may **view**, **use**, and **share** this code for learning or non-commercial purposes.
- Please contact the authors if you'd like to:
  - Reuse the code in other projects
  - Make derivative works
  - Deploy the system commercially

© 2025 Koosha Shamdani. All rights reserved.
