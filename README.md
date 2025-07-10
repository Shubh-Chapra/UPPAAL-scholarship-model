# UPPAAL Scholarship Portal Model

This project models a **Scholarship Application Portal** using **UPPAAL**, built as part of the Logic in Computer Science course at BITS Pilani.

## 📌 Objective
- Allow students to login, view personal info, and apply for scholarships (Merit or MCN).
- Fetch transcripts and interact with an approval committee.
- Ensure system correctness through formal verification.

## 🧩 Model Components
- `Student`: Handles login, scholarship application, and logout
- `Portal`: Middle layer for coordination
- `Academic_Server`: Fetches transcripts
- `Scholarship_Approval_Committee`: Decides scholarship approval based on CGPA

## ✅ Verification Performed
### Safety Checks:
- Only one scholarship application per student
- No deadlock
- Mutual exclusion: Cannot receive both scholarships
- Logout state implies user not on homepage

### Liveness Checks:
- Student returns to homepage
- Eligible CGPA results in approval
- Transcript requests are eventually fulfilled

## 📁 Files
- `scholarship_model.xml`: The full UPPAAL model
- `Project_Report.pdf`: Description and assumptions
- `screenshots/`: Optional images of model and query results

---

### 📌 How to Run
Open the `.xml` file in the UPPAAL GUI and use the **Verifier** tab to test queries.

---

## 👥 Team Members
- Shubh Chapra  
- Hamza Najfi  
- Aayush Kumar  
- Samarth Kothari  
- Aakarsh Mishra
# UPPAAL-scholarship-model
