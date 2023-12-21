# Junyi

## Dataset Description
This dataset was collected from Junyi Academy, which is an education website of providing learning materials and exercises on various scientific courses on 2015.   
https://pslcdatashop.web.cmu.edu/DatasetInfo?datasetId=1198


### Special Notes
- It contains 1048574 interactions, 247546 students and 2834 questions in the dataset.
- These pieces of information might be what you paid extra attention to in your model.
  - Exercise Relation(prerequisite)
  - Concept Relation(tree and prerequisite)
  - Repeatable Answer Record


## Column Description

| Attribute            | Note |
|:----------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| user_id              | An number represents an user |
| exercise             | Exercise name |
| problem_type         | Some exercises would record what template of problem this student encounters at this time |
| problem_number       | How many times this student practices this exercise (e.g., the number would be 1 if the student tries to answer this exercise at the first time)                                                                 |
| topic_mode           | Whether the student is assigned this exercise by clicking the topic icon (This function has been closed now) |
| suggested            | Whether the exercise is suggested by the system according to prerequisite relationships on the knowledge map |
| review_mode          | Whether the exercise is done by the student after he/she earn proficiency |
| time_done            | Unix timestamp in microseconds |
| time_taken           | Second the student spend on this exercise |
| time_taken_attempts  | Seconds the student spend on each answering attempt |
| correct              | Whether the student’s first attempt is correct, and the field would be false if any hint is requested |
| count_attempts       | How many times student attempt to answer the problem |
| hint_used            | Whether student request hints |
| count_hints          | How many times student request hints |
| hint_time_taken_list | Seconds the student spend on each requested hints |
| earned_proficiency   | Whether the student reaches proficiency.   Please refer to http://david-hu.com/2011/11/02/how-khan-academy-is-using-machine-learning-to-assess-student-mastery.html for the algorithm of determining proficiency |
| points_earned        | How many points students earn for this practice |

