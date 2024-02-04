# EdNet_KT1

## Dataset Description
EdNet-KT1 is the dataset of student-system interactions collected over 2 years by Santa(an artificial intelligence guidance system). It contains 131317236 interactive information of 784309 students, which is the largest public interactive education system data set released so far. In our experiment, we sampled 5000 for this study. The sampled dataset includes 5000 students, 13169 questions, 189 KCs.  
KT1：http://bit.ly/ednet_kt1  
Content：http://bit.ly/ednet-content


### Special Notes
- These pieces of information might be what you paid extra attention to in your model.
  - Exercise Relation(tree)
  - Repeatable Answer Record


## Column Description

### KT1:

| Attribute    | Note                                                                                                                    |
|:--------------|:-------------------------------------------------------------------------------------------------------------------------|
| user_id      | student’s id |
| timestamp    | the moment the question was given, represented as Unix timestamp in milliseconds |
| solving_id   | represents each learning session of students corresponds to each bunle. It is a form of single integer, starting from 1 |
| question_id  | the ID of the question that given to student, which is a form of q{integer} |
| user_answer  | the answer that the student submitted, recorded as a character between a and d inclusively |
| elapsed_time | the time that the students spends on each question in milliseconds |

### Questions:

| Attribute      | Note |
|:----------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| question_id    | the ID of the question, which is a form of q{integer}. |
| bundle_id      | the ID of the bundle containing the question, which is a form of b{integer}. Each bundle can contains from 1 to 5 questions. |
| explanation_id | ID of corresponding explanations (expert's commentaries) for each bundle, which is a form of e{integer}. Note that bundle_ids and explanation_ids are the same for every question. |
| correct_answer | the correct answer of each question recorded as a character between a and d inclusively. The number of choices depends on the part of the question: every question that does not belong to part 2 has four choices, and part 2 questions have three. |
| part           | the part of each question. It is an integer from 1 to 7. |
| tags           | the expert-annotated tags for each question. It is a list of integers, which has a form of {integer};{integer};...;{integer}. |
| deployed_at    | represents the time that each question is started to served in Santa, represented as Unix timestamp in milliseconds. |


