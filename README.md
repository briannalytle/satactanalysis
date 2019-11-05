# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 1: Standardized Testing, Statistical Summaries and Inference

### Problem Statement

With the new format of the SAT, the College Board needs to come up with some strategies on how to best allocate money to improve SAT participation rates. In this report, we must analyze data from the 2017 and 2018 SAT exams and ACT exams from across the country. With our findings, we will present strategies on how to improve overall SAT rates for upcoming years by focusing on a small group states. 

---

### Datasets

#### Provided Data

For this project, you'll have two provided datasets:

- [2017 SAT Scores](./data/sat_2017.csv)
- [2017 ACT Scores](./data/act_2017.csv)
- [2018 SAT Scores](./data/sat_2018.csv)
- [2018 ACT Scores](./data/act_2018.csv)

#### Manipulated Data
- [2017 State SAT/ACT results](./data/combined_2017.csv)
- [SAT/ACT Comparison (California, New York, Texas)](./data/sat_act.csv)
- [More SAT/ACT Comparison (California, New York, Texas)](./data/state_test.csv)

**This data has been compiled into CSV files which are also included in the *data* directory of this repo**


#### Outside Sources
https://www.worldatlas.com/articles/which-state-has-the-most-colleges.html
https://reports.collegeboard.org/sat-suite-program-results/class-2018-results
https://www.compassprep.com/great-to-good-the-diluted-value-of-high-test-scores/



| Column Name | Type | Dataset | Description |
| ------------|------|---------|-------------|
|state|object|combined_2017.csv|State where test was taken|
|sat_participation|integer|combined_2017.csv|percentage of SAT state student participation rate|
|sat_rw|integer|combined_2017.csvState average SAT evidence based reading and writing score|
|sat_math|integer|combined_2017.csv|State average SAT math score|
|sat_total|integer|Scombined_2017.csv|Total SAT average SAT score|
|act_participation|integer|combined_2017.csv|percentage of ACT state student participation rate|
|act_english|float|combined_2017.csv|State average ACT English score|
|act_math|float|combined_2017.csv|State average ACT math score|
|act_reading|float|combined_2017.csv|State average ACT reading score|
|act_science|float|combined_2017.csv|State average ACT Science score|
|act_composite|float|combined_2017.csv|State ACT total average score|
|state18|object|scores_2018|State where test was taken|
|sat18_participation|integer|scores_2018|percentage of SAT state student participation rate|
|sat18_rw|integer|scores_2018|State average SAT evidence based reading and writing score|
|sat18_math|integer|scores_2018|State average SAT math score|
|sat18_totalscore|integer|scores_2018|Total SAT average score|
|act18_participation|integer|scores_2018|percentage of ACT state student participation rate|
|act18_composite|float|scores_2018|State overall ACT Score|

---

### Trends

There was a a significant population of states that had a 100% participation rate for the SAT or ACT, but never both. If the state had a high a 100% participation rate for the SAT, they was a significantly low participation rate for the ACT and vice versa. IF a state had a a 90% + participation rate for either exam, the total average mean of the exam would be ranked low. Most states with a lower participation rates for exams were more likely to have a high overall mean. 

Between the two years, there were some states that made a large jump in SAT Participation. Illinois had a 9% participation rate for the 2017 SAT and a 99% participation rate for the 2018 SAT. The state's ACT participation rate dropped from 93% to 43%. Sources explained that this was because the state was no longer funding ACT exams for students and started to push funding for the SAT. 

Though some states improved their participation percentage in 2018, their participation percentage ranking dropped. We can assume this is because other states jumped higher in participation. As we can see in the boxplot below, the IQR of the ACT exam for both years is much higher than the SAT exam. We can notice that the overall SAT participation rates did improve in 2018, but it is still no where close to the ACT spread.


![participation spread](/../images/participation_spread.png?raw=true)

---

### Conclusion

The College Board should focus on funding the states with the most colleges and universities. California, New York, and Texas have over 200 colleges in their state and the participation rate for the SAT was below 70% each year with the exception of New York in 2018. All 3 states rank below 50% on ACT exam participation. This shows us there is the states have no ties with the ACT exam. The best way to influence students to take the SAT is to educate them on the exam itself. This could be exposing students early with mandatory PSAT examination. This could also mean providing more access to SAT student materials and SAT exam dates and locations.


