# ASSISTment_2017

## Dataset Description
This dataset utilized in the 2017 ASSISTments data mining competition. Researchers collected it from a longitudinal study, which tracks students from their use of ASSISTments blended learning platform in middle school in 2004-2007.   
https://sites.google.com/view/assistmentsdatamining/dataset  


### Special Notes
- It contains 942781 interactions, 1709 students, and 3162 questions.
- These pieces of information might be what you paid extra attention to in your model.
  - Concept Text
  - Repeatable Answer Record
  - The time when students start answering a question and the duration of time spent on answering the question.

## Column Description
| Attribute | Note |
| ------ | ------ |
| student id | a deidentified ID/tag used for identifying an individual student |
| SY ASSISTments Usage | the academic years the student used ASSISTments |
| AveKnow | average student knowledge level (according to Bayesian Knowledge Tracing algorithm – cf. Corbett & Anderson, 1995) |
| AveCarelessness | average student carelessness (according to San Pedro, Baker, & Rodrigo, 2011 model) |
| AveCorrect | average student correctness |
| NumActions | total number of student actions in system |
| AveResBored | average student affect: boredom (see Pardos, Baker, San Pedro, Gowda, & Gowda, 2014) |
| AveResEngcon | average student affect:engaged concentration (see Pardos, Baker, San Pedro, Gowda, & Gowda, 2014) |
| AveResConf | average student affect:confusion (see Pardos, Baker, San Pedro, Gowda, & Gowda, 2014) |
| AveResFrust | average student affect:frustration (see Pardos, Baker, San Pedro, Gowda, & Gowda, 2014) |
| AveResOfftask | average student affect: off task (see Pardos, Baker, San Pedro, Gowda, & Gowda, 2014 and also Baker, 2007) |
| AveResGaming | average student affect:gaming the system (see Pardos, Baker, San Pedro, Gowda, & Gowda, 2014 and also Baker Corbett Koedinger & Wagner, 2004) |
| actionId | the unique id of this specific action |
| skill | a tag used for identifying the cognitive skill related to the problem (see Razzaq, Heffernan, Feng, & Pardos, 2007) |
| problemId | a unique ID used for identifying a single problem |
| assignmentId | a unique ID used for identifying an assignment |
| assistmentId | a unique ID used for identifying an assistment (a instance of a multi-part problem) |
| startTime | when did the student start the problem (UNIX time, seconds) |
| endTime | when did the student end the problem (UNIX time, seconds) |
| timeTaken | Time spent on the current step |
| correct | Answer is correct |
| original | Problem is original not a scaffolding problem |
| hint | Action is a hint response |
| hintCount | Total number of hints requested so far |
| hintTotal | total number of hints requested for the problem |
| scaffold | Problem is a scaffolding problem |
| bottomHint | Bottom-out hint is used |
| attemptCount | Total problems attempted in the tutor so far. |
| problemType | the type of the problem |
| frIsHelpRequest | First response is a help request |
| frPast5HelpRequest | Number of last 5 First responses that included a help request |
| frPast8HelpRequest | Number of last 8 First responses that included a help request |
| stlHintUsed | Second to last hint is used an indicates a hint that gives considerable detail but is not quite bottom-out |
| past8BottomOut | Number of last 8 problems that used the bottom-out hint. |
| totalFrPercentPastWrong | Percent of all past problems that were wrong on this KC. |
| totalFrPastWrongCount | Total first responses wrong attempts in the tutor so far. |
| frPast5WrongCount | Number of last 5 First responses that were wrong |
| frPast8WrongCount | Number of last 8 First responses that were wrong |
| totalFrTimeOnSkill | Total first response time spent on this KC across all problems |
| timeSinceSkill | Time since the current KC was last seen. |
| frWorkingInSchool | First response Working during school hours (between 7:00 am and 3:00 pm) |
| totalFrAttempted | Total first responses attempted in the tutor so far. |
| totalFrSkillOpportunities | Total first response practice opportunities on this KC so far. |
| responseIsFillIn | Response is filled in (No list of answers available) |
| responseIsChosen | Response is chosen from a list of answers (Multiple choice, etc). |
| endsWithScaffolding | Problem ends with scaffolding |
| endsWithAutoScaffolding | Problem ends with automatic scaffolding |
| frTimeTakenOnScaffolding | First response time taken on scaffolding problems |
| frTotalSkillOpportunitiesScaffolding | Total first response practice opportunities on this skill so far |
| totalFrSkillOpportunitiesByScaffolding | Total first response scaffolding opportunities for this KC so far |
| frIsHelpRequestScaffolding | First response is a help request Scaffolding |
| timeGreater5Secprev2wrong | Long pauses after 2 Consecutive wrong answers |
| sumRight | NaN |
| helpAccessUnder2Sec | Time spent on help was under 2 seconds |
| timeGreater10SecAndNextActionRight | Long pause after correct answer |
| consecutiveErrorsInRow | Total number of 2 wrong answers in a row across all the problems |
| sumTime3SDWhen3RowRight | NaN |
| sumTimePerSkill | NaN |
| totalTimeByPercentCorrectForskill | Total time spent on this KC across all problems divided by percent correct for the same KC |
| prev5count | NaN |
| timeOver80 | NaN |
| manywrong | NaN |
| confidence(BORED) | the confidence of the student affect prediction: bored |
| confidence(CONCENTRATING) | the confidence of the student affect prediction: concecntrating |
| confidence(CONFUSED) | the confidence of the student affect prediction: confused |
| confidence(FRUSTRATED) | the confidence of the student affect prediction: frustrated |
| confidence(OFF TASK) | the confidence of the student affect prediction: off task |
| confidence(GAMING) | the confidence of the student affect prediction: gaming |
| RES_BORED | rescaled of the confidence of the student affect prediction: boredom |
| RES_CONCENTRATING | rescaled of the confidence of the student affect prediction: concentration |
| RES_CONFUSED | rescaled of the confidence of the student affect prediction: confusion |
| RES_FRUSTRATED | rescaled of the confidence of the student affect prediction: frustration |
| RES_OFFTASK | rescaled of the confidence of the student affect prediction: off task |
| RES_GAMING | rescaled of the confidence of the student affect prediction: gaming |
| Ln-1 | baysian knowledge tracing’s knowledge estimate at the previous time step |
| Ln | baysian knowledge tracing’s knowledge estimate at the time step |
| schoolID | the id (anonymized) of the school the student was in during the year the data was collected |
| MCAS | Massachusetts Comprehensive Assessment System test score. In short, this number is the student’s state test score (outside ASSISTments) during that year. -999 represents the data is missing |
  
