#  NEXUS: AI Task Planning & Scheduling Agent

A beginner-friendly personal productivity assistant that turns messy, everyday thoughts into an organized, conflict-free daily timetable.

---

## What is NEXUS?

Planning a busy day is hard. When you have classes, upcoming tests, coding assignments, and project deadlines, it is easy to feel overwhelmed and wonder: **"What should I work on right now?"**

**NEXUS** fixes this. 

You do not need to fill out tedious forms or click twenty buttons. You simply write how your day looks in casual, natural English:

> *"I have college classes from 9 AM to 4 PM. I have an exam next Tuesday at 11 AM, need to study 2 hours for DBMS, and have to finish my Java assignment by tomorrow."*

NEXUS reads your message, extracts your tasks, finds your free hours, avoids overlapping classes, schedules 15-minute rest breaks, and sends a clear summary directly to your email inbox.

---

##  How It Works 

**Reads Your Raw Thoughts (No Forms Needed):**
   * You type your schedule naturally (e.g., *"Exam at 10 AM, need 2 hours for DSA, and classes from 9 to 4"*).
   * The AI brain reads the text and separates **fixed events** (classes, exams) from **flexible tasks** (homework, revision).

 **Solves the Timeline (Zero Double-Booking):**
   * Locks your classes and exams in place first.
   * Finds the open free hours before and after your commitments.
   * Fits your highest-priority tasks into those open windows without overlapping.
   * Automatically adds a **15-minute rest break** after any study session to prevent burnout.

 **Saves & Updates Live (SQLite Database):**
   * Stores every task and its current status (`PENDING` or `COMPLETED`).
   * When you finish a task, enter its ID and click **Complete**—NEXUS instantly recalculates the rest of your day.

 **Sends You an Email Digest:**
   * Dispatches a clean HTML briefing straight to your inbox with color-coded priority badges and your immediate next action.
##  Live Output & How It Works

<div align="center">
  <img src="https://github.com/user-attachments/assets/17aaa9ef-e1d9-427b-ac4d-fb7239c2d2ec" width="950" alt="NEXUS Output Screenshot" />
</div>

---

### Understanding the Screen (In Simple Words)

1. **What You Type (Input Box):**
   * You write what you want to do in everyday English: *"I have to solve DSA problems and practice it on LeetCode."*[cite: 11]
   * No complex forms or manual time inputs needed[cite: 11].

2. **The Output Timetable (Zero Confusion):**
   * **Organized Time Slots:** The agent arranged tasks sequentially from **08:00 AM** without overlapping[cite: 11].
   * **Smart Rest Breaks:** Notice the **15-minute breaks** (*Rest & Re-energize*) placed after each study session to prevent burnout[cite: 11].
   * **Clear Next Step:** The top-right box tells you exactly what to begin with right now[cite: 11].

3. **Autonomous Email Digest:**
   * Dispatches an alert confirming `Email successfully sent!` straight to your inbox[cite: 11].

4. **Task Tracker & Dynamic Rescheduling:**
   * Keeps track of all your tasks in an internal database with IDs and statuses[cite: 11].
   * When an item is finished, simply enter its Task ID (e.g., **3**) and click **Mark as Completed & Recalculate**[cite: 11].
   * The status changes to `COMPLETED` and the agent automatically recalculates the remaining time for the day[cite: 11].
