# ASSISTment_2012-2013

## Dataset Description
The data is gathered from skill builder problem sets where students need to work on similar exercises to achieve mastery, which contains data for the school year 2012-2013.  
https://sites.google.com/site/assistmentsdata/datasets/2012-13-school-data-with-affect

### Special Notes
- It consists of 2711813 interactions, 29018 students, and 53091 questions.
- These pieces of information might be what you paid extra attention to in your model.
  - Concept Text
  - Repeatable Answer Record
  - The time when students start answering a question and the duration of time spent on answering the question.

## Column Description
| Attribute  | Note |
|:-----------------|:----------- |
| problem_log_id  | Unique ID of the logged actions.|
| skill| Skill name associated with the problem (different skills are in different rows).|
| problem_id| The ID of the problem.|
| user_id| The ID of the student doing the problem.|
| assignment_id   | Two different assignments can have the same sequence id. Each assignment is specific to a single teacher/class.|
| assistment_id   | The ID of the ASSISTment. An ASSISTment consists of one or more problems.|
| start_time| Timestamp when the problem starts.|
| end_time| Timestamp when the problem ends.|
| problem_type    | choose_1: Multiple choice (radio buttons)  <br/>algebra: Math evaluated string (text box)  <br/>fill_in: Simple string-compared answer (text box)  <br/>open_response: Records student answer, but their response is always marked correct|
| original| 1 = Main problem  <br/>0 = Scaffolding problem|
| correct| 1 = Correct on first attempt  <br/>Decimal values are calculated as a partial credit based on the number of hints and attempts needed to solve (based on teacher setting)  <br/>0 = Student either saw the answer, exhausted partial credit from too many hints/attempts, or (based on teacher setting) answered incorrectly on the first attempt|
| bottom_hint| Whether or not the student asks for all hints.|
| hint_count| Number of hints on this problem.|
| actions| Every action on this problem.|
| attempt_count| Number of student attempts on this problem.|
| ms_first_response | The time in milliseconds for the student's first response.|
| tutor_mode| Tutor, test mode, pre-test, or post-test.|
| sequence_id| The content id of the problem set. Different assignments that are assigned the same problem set will have the same sequence id. Again the terminology is confused as years ago when ASSISTments was starting we called problem sets sequences. But a problem set in our modern use of the term is really stored as a sequence. Most sequences are simple, but it's possible to build a problem set that is a hierarchical tree of problem sets. |
| student_class_id | The class ID.|
| position| Assignment position on the class assignments page.|
| type| This is the type of the head section of the problem set.|
| base_sequence_id | This is to account for if a sequence has been copied. This will point to the original copy, or be the same as sequence_id if it hasn't been copied.|
| skill_id| ID of the skill associated with the problem (different skills are in different rows).|
| teacher_id| The ID of the teacher who assigned the problem.|
| school_id       | The ID of the school where the problem was assigned.|
| overlap_time    | The time in milliseconds for the student's overlap time.|
| template_id     | The template ID of the ASSISTments. ASSISTments with the same template ID have similar questions.|
| answer_id       | The answer ID for multi-choice questions.|
| answer_text     | The answer text for fill-in questions.|
| first_action    | The type of first action: attempt or ask for a hint.|