# Math2

## Dataset Description
Similar to the Math 1 dataset, this dataset is also collected from two final mathematical exams from high school students, including both objective and subjective problems, which represented by a score matrix and a given Q-matrix by education experts.   
http://staff.ustc.edu.cn/~qiliuql/data/math2015.rar


### Special Notes
- It contains 3911 examinees, 17 skills, 16 objective problems and 4 subjective problems.
- The concept text is included in it.
- It can be downloaded automatically in our models.

## Files Description
| File | Note |
| :------ | :------ |
| data.txt | The responses or normalized scores (which are scaled in range [0,1] by dividing full scores of each problem) of each examinee on each problems, and a row denotes an examinee while a column stands for a problem. |
| q.txt | The indicator matrix of relationship between problems and skills, which derives from experienced education experts. And a row represents a problem while a column for a skill. E.g., problem i requires skill k if entry(i, k) equals to 1 and vice versa.|
| qnames.txt | The detailed names or meanings of related specific skill.|
| problemdesc.txt | The description of each problem, including the problem type (objective or subjective) and full scores of each problem (set to 1 for all the problems in FrcSub dataset).|
| rawdata.txt | The raw unnormalized scores of the Math1 and Math2 datasets. |

