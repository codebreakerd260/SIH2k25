**🚀 SIEC Hackathon Management Portal**

A lightweight **digital portal** to conduct, organize, and manage internal hackathons at Sreyas Institute of Engineering & Technology.  
 Built to streamline **registrations, submissions, mentoring, and evaluations** for SIEC Internal Hackathon 2025\.

---

## **🎯 Vision**

Make hackathon management **simple, transparent, and scalable** for 800–1000 students, 150 teams, and supporting staff (mentors, admins).

---

## **🛠️ Tech Stack**

- **Frontend/Backend** → Next.js (TypeScript)

- **Database** → MongoDB Atlas (fast JSON workflow, mock data ready)

- **Deployment** → Vercel (1-click, CI/CD)

---

## **👤 User Roles & Access Control**

- **Team Leader** → Login with `email + teamCode`. Can submit & edit round forms.

- **Team Members** → View progress using `teamCode` (read-only).

- **Mentors** → Access all team submissions. Provide scores & comments.

- **Admins** → Full control. Shortlist/eliminate, assign presentation order, finalize winners.

---

## **📂 Hackathon Flow**

### **Round 1 (Ideation)**

- Problem Statement (chosen from SIH)

- Solution & Approach

- Tech Stack / Hardware

### **Round 2 (Progress)**

- Struggles & challenges

- Mentor request (support needed)

- Repo link

### **Round 3 (Final Submission)**

- PPT link

- Live demo link

- Final repo link

---

## **📊 Evaluation Flow**

### **Mentors**

- Score teams (per round) using consistent rubric.

- Add qualitative feedback.

- Scores remain **private** (visible only to mentors & admins).

### **Admins**

- See aggregated mentor scores (averages, breakdowns).

- Add **final admin score & comments**.

- Decide:

  - Shortlist / Eliminate

  - Presentation Order

  - Winners, Runner-up, Top Teams

---

## **🏗️ Data Model (MongoDB Collections)**

### **Teams**

{  
 "id": "TEAM001",  
 "teamName": "CodeBreakers",  
 "leader": { "name": "Aarav", "email": "aarav@example.com", "rollNo": "24VE1A0532" },  
 "members": \[ { "name": "Diya", "email": "diya@example.com", "rollNo": "24VE1A0561" } \]  
}

### **Submissions**

{  
 "teamId": "TEAM001",  
 "round": 2,  
 "fields": {  
 "struggles": "API integration issues",  
 "mentorRequest": "Database optimization help",  
 "repoLink": "https://github.com/team1/project"  
 }  
}

### **Scores**

{  
 "teamId": "TEAM001",  
 "round": 2,  
 "mentorScores": \[  
 {  
 "mentorId": "MENTOR007",  
 "criteria": { "innovation": 7, "feasibility": 8, "presentation": 6 },  
 "comments": "Solid approach, needs polish."  
 }  
 \],  
 "adminScore": {  
 "criteria": { "innovation": 9, "feasibility": 8, "presentation": 8 },  
 "finalComment": "Well-deserved finalist."  
 }  
}

---

## **⚡ Deployment Plan (2.5 Days)**

- **Day 1** → Setup project, connect DB, scaffold routes, seed mock data.

- **Day 2** → Build team flow (login, submissions, dashboards).

- **Day 3 (Buffer)** → Add mentor scoring, admin controls, polish UI.

---

## **✅ Benefits**

- Single platform for all hackathon activities.

- Mentoring & evaluation become structured and transparent.

- Easy scalability for future SIEC hackathons.

- Feedback loop for students (post-hackathon).

---

⚡ **Tagline:**

_From forms & WhatsApp chaos → to one clean digital portal for SIEC hackathons._

---
