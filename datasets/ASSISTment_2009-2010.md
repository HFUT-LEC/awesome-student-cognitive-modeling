# ASSISTment_2009-2010

## Dataset Description
This dataset was collected during the school year 2009−2010 using the ASSISTments online education website.   
https://sites.google.com/site/assistmentsdata/home/2009-2010-assistment-data/skill-builder-data-2009-2010  

### Special Notes
- The dataset consists of 16988 distinct questions answered by 4163 students which gives a total number of 255382 exercises.
- It can be downloaded automatically in our models.
- These pieces of information might be what you paid extra attention to in your model.
  - Concept Text
  - Repeatable Answer Record
  - The time students take to answer questions

## Column Description
| Attribute   | Note                                                                              |
|:-------------|:-----------------------------------------------------------------------------------|
| order id | Non-chronological id, refer to original problem log |
| assignment id | Each assignment is specific to single teacher/class. |
| user id | Id of the student |
| problem id | Id of the problem |
| original | Main problem or Scaffolding problem |
| correct | Correct on the fisrt attempt or Incorrect on the first attempt, or asked for help |
| attempt count | Number of attempts of the student |
| ms first reponse | The time in the milliseconds for the student’s first response |
| tutor mode | tutor or test |
| answer type | choose_1 or algebra or fill_in or open_response |
| sequence id | Id of the problem set |
| student class id | Class id |
| position | Assignment position on the class assignments page |
| problem set type | Linear or Random or Mastery |
| base sequence id | If the sequence has been copied, this points to the original copy |
| skill id | ID of the skill associated with the problem. In this skill builder dataset, records will be duplicated so that each record with one skill. |
| skill name | Name of the skill |
| teacher id | ID of the teacher |
| school id | ID of the school |
| hint count | Number of student attempts |
| hint total | Number of possible hints on the problem |
| overlap time | Time in milliseconds |
| template id | The template ID of the ASSISTment. ASSISTments with the same template ID have similar questions. |
| answer id | The answer ID for multi-choice questions. |
| answer text | The answer text for fill-in questions. |
| first action | The type of first action: attemp or ask for a hint. |
| bottom hint | Whether or not the student asks for all hints. |
| opportunity | The number of opportunities the student has to practice on this skill. |
| opportunity original | The number of opportunities the student has to practice on this skill counting only original problems. |

