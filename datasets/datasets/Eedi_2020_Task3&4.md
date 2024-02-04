# Eedi_2020_Task3&4

## Dataset Description
This dataset is from the Tasks 3 & 4 at the NeurIPS 2020 Education Challenge. Task 3 focuses on predicting the quality of questions accurately. In Task 4, the aim is to recommend a personalized sequence of questions for each student that best predicts the student’s answers.  
https://dqanonymousdata.blob.core.windows.net/neurips-public/data.zip


### Special Notes
- It contains 4,918 Students, 948 Questions, and 1,382,727 interactions.
- These pieces of information might be what you paid extra attention to in your model.
  - Exercise Images
  - Concept Text
  - Concept Relation(tree)


## Column Description

### The Structure
- images
  - 0.jpg...
- metadata
  - [answer_metadata_task_3_4.csv](#1-answer_metadata_task_3_4csv)
  - [question_metadata_task_3_4.csv](#2-question_metadata_task_3_4csv)
  - [student_metadata_task_3_4.csv](#3-student_metadata_task_3_4csv)
  - [subject_metadata.csv](#4-subject_metadatacsv)
- train_data
  - [train_task_3_4.csv](#5-train_task_3_4csv)

## 1. answer_metadata_task_3_4.csv

| Attribute | Note |
| ------ | ------ |
| AnswerId |  An ID uniquely identifying the answer, which can be joined to the primarydataset. |
| DateAnswered |  Time and date that the question was answered, to the nearestminute. |
| Confidence |  Percentage confidence score given for the answer. 0 means a randomguess, 100 means total confidence. |
| GroupId |  The class (group of students) in which the student was assigned thequestion. |
| QuizId |  The assigned quiz which contains the question the student answered. |
| SchemeOfWorkId |  The scheme of work in which the student was assigned thequestion. |


## 2. question_metadata_task_3_4.csv
| Attribute | Note |
| ------ | ------ |
| QuestionId |  ID of the question answered. |
| SubjectId | Each subject covers an area of mathematics, at varying degrees of granularity. We provide IDs for each topic associated with a question in a list. In addition to the topics, we will also provide the image presented to the student for each question.|

## 3. student_metadata_task_3_4.csv
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

## 5. train_task_3_4.csv
| Attribute | Note |
| ------ | ------ |
| QuestionId |  ID of the question answered. |
| UserId |  ID of the student who answered the question. |
| AnswerId |  Unique identifier for the (QuestionId, UserId) pair, used to join with  associated answer metadata (see below). |
| IsCorrect |  Binary indicator for whether the student’s answer was correct (1 is  correct, 0 is incorrect). |
| CorrectAnswer |  The correct answer to the multiple-choice question (value in [1,2,3,4]). |
| AnswerValue | The student’s answer to the multiple-choice question(value in [1,2,3,4]). |