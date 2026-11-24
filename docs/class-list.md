# Class List (v0.1)

First draft of the classes, taken from the Requirements Document. We will use these names in our diagrams. The list will be updated while we prepare the design drafts.

| Class | Responsibility | Requirements |
|---|---|---|
| `Course` | A course and its exam (duration, difficulty, needed classroom features) | FR 1, 5, 9, 12, 13 |
| `Student` | A student and the courses they take | FR 1, 2 |
| `Classroom` | A classroom, its capacity and features | FR 1, 10, 11 |
| `ExamPeriod` | The exam days and the time slots | FR 4 |
| `TimeSlot` | One time interval on one exam day | FR 4, 29 |
| `Invigilator` | A staff member who supervises exams (optional) | FR 14, 15 |
| `ExamSchedule` | The created schedule | FR 7, 26 |
| `ScheduledExam` | The exam of one course: its time slot and classrooms | FR 7, 19, 28, 29 |
| `ClassroomAllocation` | One classroom of an exam and the students in it | FR 33, 34 |
| `DataImporter` | Reads and checks the input files | FR 1, 3, 6, 23, 24 |
| `DataRepository` | Saves and loads the data | FR 27 |
| `ScheduleGenerator` | Creates the schedule following the rules | FR 7, 8, 28–39, 50–52 |
| `ScheduleValidator` | Checks a schedule against the rules | FR 40, NFR 8 |
| `ScheduleUpdater` | Updates the schedule when the data changes | FR 26, 42 |
| `InvigilatorAssigner` | Assigns invigilators if a list is given (optional) | FR 16, 43–49 |
| `ScheduleExporter` | Exports and prints the schedule | FR 20, 21, 54 |

The user interface classes will be added by Eljan with the screen sketches (T6).

**Parts:** Tuana – data classes, `ScheduleGenerator`, `ScheduleValidator` · Umut – `DataImporter`, `DataRepository`, `ScheduleUpdater` · Orhan – `Invigilator`, `InvigilatorAssigner`, `ScheduleExporter` · Eljan – user interface
