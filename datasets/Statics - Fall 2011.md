# Statics - Fall 2011

## Dataset Description
This dataset was collected from the online course "OLI Engineering Statics - 1.14." The data collection period spans from August 22, 2011, to December 8, 2011.   
https://pslcdatashop.web.cmu.edu/Export?datasetId=507


### Special Notes
- It contains The dataset encompasses 333 students, 1,224 steps of questions, 94 KCs.
- These pieces of information might be what you paid extra attention to in your model.
  - Exercise Text(webpages)
  - Exercise Relation(tree)
  - Concept Text
  - Repeatable Answer Record


## Column Description
| Attribute            | Note |
| :---- | :---- |
| Row | A row counter. |
| Sample | The sample that includes this step. If you select more than one sample to export, steps that occur in more than one sample will be duplicated in the export. |
| Anon Student ID | The student that performed the step. |
| Problem Hierarchy | The location in the curriculum hierarchy where this step occurs. |
| Problem Name | The name of the problem in which the step occurs. |
| Problem View | The number of times the student encountered the problem so far.|
| Step Name | Formed by concatenating the "selection" and "action". Also see the glossary entry for "step". |
| Step Start Time | If it's the first step of the problem, the step start time is the same as the problem start time If it's a subsequent step, then the step start time is the time of the preceding transaction, if that transaction is within 10 minutes. If it's a subsequent step and the elapsed time between the previous transaction and the first transaction of this step is more than 10 minutes, then the step start time is set to null as it's considered an unreliable value. |
| First Transaction Time | The time of the first transaction toward the step. |
| Correct Transaction Time | The time of the correct attempt toward the step, if there was one. |
| Step End Time | The time of the last transaction toward the step. |
| Step Duration (sec) | The elapsed time of the step in seconds, calculated by adding all of the durations for transactions that were attributed to the step. |
| Step Duration (sec) | The elapsed time of the step in seconds, calculated by adding all of the durations for transactions that were attributed to the step. |
| Correct Step Duration (sec) | The step duration if the first attempt for the step was correct. |
| Error Step Duration (sec) | The step duration if the first attempt for the step was an error (incorrect attempt or hint request). |
| First Attempt | The tutor's response to the student's first attempt on the step. Example values are "hint", "correct", and "incorrect". |
| Incorrects | Total number of incorrect attempts by the student on the step. |
| Hints | Total number of hints requested by the student for the step. |
| Corrects | Total correct attempts by the student for the step. (Only increases if the step is encountered more than once.) |
| Condition | The name and type of the condition the student is assigned to.  |
| KC (model_name) | Knowledge component(s) associated with the correct performance of this step. |
| Opportunity (model_name) | An opportunity is the first chance on a step for a student to demonstrate whether he or she has learned the associated knowledge component.  |
| Predicted Error Rate (model_name) | A hypothetical error rate based on the Additive Factor Model (AFM) algorithm. 1:error,0:correct. |

