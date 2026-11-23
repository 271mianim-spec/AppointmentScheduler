# Appointment_Scheduler-Student
﻿SMART APPOINTMENT SCHEDULER - STUDENT STARTER
=============================================


CONTENTS (all in ONE folder when extracted)
  Appointment.java             - PROVIDED; do not edit
  AppointmentScheduler.java    - FIVE TODO methods to complete
  SchedulerMain.java           - PROVIDED console menu and startup/save I/O
  data/seed_schedule.txt       - starting schedule; do not edit
  BST_Appointment_Scheduler_Student_Directions.docx - assignment


SETUP
1. Extract this ZIP to a new folder.
2. In VS Code, File > Open Folder, and select THAT folder directly.
   The data folder must be in the same folder as the three .java files.
3. Run SchedulerMain.java (or in the terminal: javac *.java && java SchedulerMain).
4. Expected first message: Loaded 5 appointments from data/seed_schedule.txt


ONLY EDIT AppointmentScheduler.java.
The menu and initial file loading work before any TODO methods are completed.
Saving will not overwrite an earlier saved file until write() is implemented.
When working, save writes data/saved_schedule.txt; the next run loads that first.


ALL TIMES ARE 24-HOUR HH:MM. This is a single-day calendar, 08:00 to 17:00.


Questions:

1. Explain how floor() and ceiling() allow your scheduling program to detect overlapping appointments. 
Why is checking these two appointments sufficient, rather than checking every appointment in the calendar?

The only appointments that will ultimately cause a conflict are the appointments before and after the desired time.
Using floor and ceiling lets you obtain these two appointments, which gives you all the information needed to 
determine if it's available or not

2. Why is a TreeSet (balanced binary search tree) more efficient than an unsorted ArrayList for finding the 
appointments immediately before and after a requested time? Compare their Big O time complexities and explain 
why this matters as the schedule grows.

A balanced binary search tree lets the appointments be sorted by start time, which is easier to navigate and search through
compared to an unsorted ArrayList. With a balanced binary search tree, the Big O notation is log(n) while an unsorted ArrayList
is O(n). As the schedule grows the performance effect this has will increase


3. Why is it unnecessary to save the exact shape of TreeSet’s internal tree?

A balanced binary search tree automatically sorts itself, making storing the exact shape unnecessary and less performant