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

Required manual tests
Start the program. Verify that five appointments load and display chronologically.
Try 09:30 for 30 minutes: REJECT (overlaps 09:00–09:40).
Try 09:40 for 20 minutes: ACCEPT (fits between two appointments).
Try 10:00 for 30 minutes: REJECT (overlaps 10:15–11:00).
Try 07:30 for 30 minutes and 16:30 for 45 minutes: REJECT (outside business hours).
Try to book another appointment at 10:15 AM. The request should be rejected because that starting time is already occupied.
Find the next appointment at/after 09:40; then cancel that appointment by start time.
Save, exit, and restart. Confirm your changes remain and the initial seed is not reloaded.
