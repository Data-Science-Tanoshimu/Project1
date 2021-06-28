# The SAT and The ACT Analysis

### Problem Statement

Using the test score data from 2017 and 2018 to determine how to increase participation rates for the SAT and the ACT.

---

### Datasets

#### Provided Data

For this project, there are four provided datasets:

- [2017 SAT Scores](./data/sat_2017.csv)
- [2017 ACT Scores](./data/act_2017.csv)
- [2018 SAT Scores](./data/sat_2018.csv)
- [2018 ACT Scores](./data/act_2018.csv)

These datasets give the average SAT and ACT scores as well as participation rates for the graduating classes of 2017 and 2018 for each state.

The datasets were collected from [here](https://blog.collegevine.com/here-are-the-average-sat-scores-by-state/) for the SAT and [here](https://blog.prepscholar.com/act-scores-by-state-averages-highs-and-lows) for the ACT.

The 2018 state-by-state result averages and participation rates for the SAT are available in PDF format [here](https://reports.collegeboard.org/sat-suite-program-results/state-results). The 2018 ACT state-by-state mean composite scores and participation rates can be found [here](http://www.act.org/content/dam/act/unsecured/documents/cccr2018/Average-Scores-by-State.pdf).

---

### Executive Summary

#### 1. 2017 Data Import & Cleaning
- Import and Cleaning of the SAT & ACT 2017 data
- Merge the SAT data with the ACT data
- Save the merged data as [2017 combined](./data/combined_2017.csv)

#### 2. 2018 Data Import & Cleaning
- Import and Cleaning of the SAT & ACT 2018 data
- Merge the SAT data with the ACT data
- Save the merged data as [2018 combined](./data/combined_2018.csv)
- Merge the 2017 data with the 2018 data
- Save the combined 2017 and 2018 data as [final](./data/final.csv)

#### Data Dictionary

This data dictionary is represents the combined data above. This dataset is used to exploration purposes.

|Feature|Type|Dataset|Description|
|---|---|---|---|
|**state**|*object*|act_sat_final|The Us state names|
|**participation_sat_17**|*integer*|act_sat_final|The percentage of the particition rate for the SAT in a state | 
|**reading_and_writing_sat_17**|*integer*|act_sat_final|The test score average for each state for the Reading and Writing portion of the SAT for all students who took the SAT in 2017 (units represent test score which range from a minimum of 200 to a maximum of 800)|
|**math_sat_17**|*integer*|act_sat_final|The test score average for each state for the Math portion of the SAT for all students who took the SAT in 2017 (units represent test score which range from a minimum of 200 to a maximum of 800)|
|**total_sat_17**|*integer*|act_sat_final|The test score average for each state for the Total portion of the SAT for all students who took the SAT in 2017 (units represent test score which range from a minimum of 400 to a maximum of 1600)|
|**participation_act_17**|*integer*|act_sat_final|The percentage of the particition rate for the ACT in a state| 
|**english_act_17**|*float*|act_sat_final|The test score average for each state for the English portion of the ACT for all students who took the ACT in 2017 (units represent test score which range from a minimum of 1 to a maximum of 36)|
|**math_act_17**|*float*|act_sat_final|The test score average for each state for the Math portion of the ACT for all students who took the ACT in 2017 (units represent test score which range from a minimum of 1 to a maximum of 36)|
|**reading_act_17**|*float*|act_sat_final|The test score average for each state for the Reading portion of the ACT for all students who took the ACT in 2017 (units represent test score which range from a minimum of 1 to a maximum of 36)|
|**science_act_17**|*float*|act_sat_final|The test score average for each state for the Science portion of the ACT for all students who took the ACT in 2017 (units represent test score which range from a minimum of 1 to a maximum of 36)|
|**composite_act_17**|*float*|act_sat_final|The test score average for each state for the Composite portion of the ACT for all students who took the ACT in 2017 (units represent test score which range from a minimum of 1 to a maximum of 36)|
|**participation_sat_18**|*integer*|act_sat_final|The percentage of the particition rate for the SAT in a state | 
|**reading_and_writing_sat_18**|*integer*|act_sat_final|The test score average for each state for the Reading and Writing portion of the SAT for all students who took the SAT in 2018 (units represent test score which range from a minimum of 200 to a maximum of 800)|
|**math_sat_18**|*integer*|act_sat_final|The test score average for each state for the Math portion of the SAT for all students who took the SAT in 2018 (units represent test score which range from a minimum of 200 to a maximum of 800)|
|**total_sat_18**|*integer*|act_sat_final|The test score average for each state for the Total portion of the SAT for all students who took the SAT in 2018 (units represent test score which range from a minimum of 400 to a maximum of 1600)|
|**participation_act_18**|*integer*|act_sat_final|The percentage of the particition rate for the ACT in a state| 
|**composite_act_18**|*float*|act_sat_final|The test score average for each state for the Composite portion of the ACT for all students who took the ACT in 2018 (units represent test score which range from a minimum of 1 to a maximum of 36)|

#### 3. Exploratory Data Analysis
- Summary statistics
- Calculation of the standard deviation
- Investigate trends in the data


#### 4. Data Visualization
- Visualize correlations between all numeric features
- Define a custom function for the subplot histograms
- Plot and interpret histograms such as participation rates
- Plot and interpret scatter plots
- Plot and interpret boxplots
- Additional scatter plot (participation rates vs. scores)

#### 5. Descriptive and Inferential Statistics
- Summarizing distributions with statistical measures and Q-Q plots
- Estimate data limits

#### 6. Outside Research
- Pick 3 states (Delaware, Alabama, Florida) that demonstrate interesting trends.
- Delaware has a 100% participation rate for the SAT in 2017. The SAT is mandatory.
- Alabama has a 100% participation rate for the ACT in 2017. The ACT is mandatory
- Florida has an 83% participation rate for the SAT in 2017 and has a 73% participation for the ACT in 2017. The both tests are not mandatory.
- There is a tendency that the more the participation rates go up, the less the scores go down.

#### 7. Conclusions/Recommendation
There are some states that have made the tests mandatory. If other states were to make the tests mandatory, they could see an increase in the participation rate of the tests.

For example, Oregon has participation rates of the both tests less than 50% year and year.
Oregon can increase its participation rate for a test if they make it mandatory.

However, there could be a potential trade-off as states with high participation rates have low composite/total scores.
A potential reason could be that students that normally have no interest in taking the tests are forced to take them.
Instead of making the tests mandatory, it might be better to set up initiatives to foster interests to take the tests.

For further research in the future, gathering data regarding the household income of the students' parents would help to determine whether income has an affect on participation rates. If so, states can set policies to help students from low income families.

---
