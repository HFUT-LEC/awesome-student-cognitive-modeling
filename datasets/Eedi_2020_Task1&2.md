# Eedi_2020_Task1&2

## Dataset Description
They provided data from two school years (September 2018 to May 2020) of students’ answers to mathematics questions from Eedi, a leading educational platform which millions of students interact with daily around the globe.This dataset is from the Tasks 1 & 2 at the NeurIPS 2020 Education Challenge. The purpose of both task 1 and task 2 is to accurately predict which answers the students provide. In task 1, the goal is to predict correctness, while in task 2, the goal is to predict the chosen answer (A, B, C, or D).  
https://dqanonymousdata.blob.core.windows.net/neurips-public/data.zip


### Special Notes
- It contains 118,971 Students, 27,613 Questions, and 15,867,850 interactions.
- These pieces of information might be what you paid extra attention to in your model.
  - Concept Text
  - Concept Relation(Tree)


## Column Description

### The Structure

- metadata
  - [answer_metadata_task_1_2.csv](#1-answer_metadata_task_1_2csv)
  - [question_metadata_task_1_2.csv](#2-question_metadata_task_1_2csv)
  - [student_metadata_task_1_2.csv](#3-student_metadata_task_1_2csv)
  - [subject_metadata.csv](#4-subject_metadatacsv)
- train_data
  - [train_task_1_2.csv](#5-train_task_1_2csv)

## 1. answer_metadata_task_1_2.csv

| Attribute | Note |
| ------ | ------ |
| AnswerId |  An ID uniquely identifying the answer, which can be joined to the primarydataset. |
| DateAnswered |  Time and date that the question was answered, to the nearestminute. |
| Confidence |  Percentage confidence score given for the answer. 0 means a randomguess, 100 means total confidence. |
| GroupId |  The class (group of students) in which the student was assigned thequestion. |
| QuizId |  The assigned quiz which contains the question the student answered. |
| SchemeOfWorkId |  The scheme of work in which the student was assigned thequestion. |


## 2. question_metadata_task_1_2.csv
| Attribute | Note |
| ------ | ------ |
| QuestionId |  ID of the question answered. |
| SubjectId | Each subject covers an area of mathematics, at varying degrees of granularity. We provide IDs for each topic associated with a question in a list.  |

## 3. student_metadata_task_1_2.csv
| Attribute | Note |
| ------ | ------ |
| UserId |  An ID uniquely identifying the student, which can be joined to the primarydataset. |
| Gender |  The student’s gender, when available. 0 is unspecified, 1 is female, 2 ismale and 3 is other. |
| DateOfBirth |  The student’s date of birth, rounded to the first of the month. |
| PremiumPupil |  Whether the student is eligible for free school meals or pupil premium due to being financially disadvantaged. |


## 4. subject_metadata.csv
| Attribute | Note |
| ------ | ------ |
| SubjectId  |  An ID uniquely identifying an area of mathematics. |
| Name | Name of the  subject|
| ParentId |  The SubjectId of its parent subject|
| Level |  The level of the subject|

## 5. train_task_1_2.csv
| Attribute | Note |
| ------ | ------ |
| QuestionId |  ID of the question answered. |
| UserId |  ID of the student who answered the question. |
| AnswerId |  Unique identifier for the (QuestionId, UserId) pair, used to join with  associated answer metadata (see below). |
| IsCorrect |  Binary indicator for whether the student’s answer was correct (1 is  correct, 0 is incorrect). |
| CorrectAnswer |  The correct answer to the multiple-choice question (value in [1,2,3,4]). |
| AnswerValue | The student’s answer to the multiple-choice question(value in [1,2,3,4]). |

