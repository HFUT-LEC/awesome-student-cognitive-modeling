# Bridge2Algebra_2006-2007

## Dataset Description
This dataset is also from the KDD Cup 2010 EDM Challenge.   
https://pslcdatashop.web.cmu.edu/KDDCup/downloads.jsp  


### Special Notes
- It contains 256589 interactions, 1146 students, 19429 questions and 611 KCs.
- These pieces of information might be what you paid extra attention to in your model.
  - Concept Text
  - Repeatable Answer Record


## Column Description
| Attribute                   | Note |
|:-----------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| Row                         | The row number |
| Anon Student Id             | Unique, anonymous identifier for a student |
| Problem Hierarchy           | Course-level hierarchy containing the problem |
| Problem Name                | Unique identifier for a problem |
| Problem View                | Total times the student has seen the problem up to this point|
| Step Name                   | Unique identifier for a steps within a problem |
| Step Start Time             | The starting time of the step | 
| First Transaction Time      | First transaction time for the step |
| Correct Transaction Time    | Time of the first correct attempt for the step, if any |
| Step End Time               | Last transaction time for the step|
| Step Duration (sec)         | Duration of the step in seconds, calculated by summing all durations attributed to the step (can be null if the First Transaction Time is null) |
| Correct Step Duration (sec) | Duration of the step if the first attempt was correct |
| Error Step Duration (sec)   | Duration of the step if the first attempt was incorrect (either an incorrect attempt or a hint request) |
| Correct First Attempt       | Tutor's assessment of the student's first attempt on the step--1 if correct, 0 if incorrect |
| Incorrects                  | Number of incorrect attempts by the student on the step|
| Hints                       | Number of hints requested by the student for the step|
| Corrects                    | Total number of correct attempts by the student on the step (only increments if the step is encountered multiple times)                         |
| KC(KC Model Name)           | Identified skills used in the problem |
| Opportunity(KC Model Name)  | Counts up by one each time a student encounters a step with the listed knowledge components |