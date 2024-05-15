# Student-Performance-Analysis

*Student performance analysis:*

### Dataset Description:

Gender: Gender of the student (male/female)

EthnicGroup: Ethnic group of the student (group A to E)

ParentEduc: Parent(s) education background (from some_highschool to master's degree)

LunchType: School lunch type (standard or free/reduced)

TestPrep: Test preparation course followed (completed or none)

ParentMaritalStatus: Parent(s) marital status (married/single/widowed/divorced)

PracticeSport: How often the student parctice sport (never/sometimes/regularly))

IsFirstChild: If the child is first child in the family or not (yes/no)

NrSiblings: Number of siblings the student has (0 to 7)

TransportMeans: Means of transport to school (schoolbus/private)

WklyStudyHours: Weekly self-study hours(less that 5hrs; between 5 and 10hrs; more than 10hrs)

MathScore: math test score(0-100)

ReadingScore: reading test score(0-100)

WritingScore: writing test score(0-100)


### Analytical Questions:

What factors (features) affect test scores most?

Are there interacting features which affect test scores?

### How to perform data preprocessing on the given dataset:

Data processing typically involves several steps, including data cleaning, transformation, and analysis. Here's a basic outline of how you could approach processing the data from your data dictionary:

#### Data Cleaning:
Identify and handle missing values: Check for any missing values in each column and decide how to handle them (e.g., imputation or removal).
Remove duplicates: Identify and remove any duplicate rows if present in the dataset.
Check for outliers: Examine numerical columns for outliers and decide whether to keep or remove them based on domain knowledge.

#### Data Transformation:
Encode categorical variables: Convert categorical variables (e.g., Gender, EthnicGroup) into numerical format using techniques like one-hot encoding or label encoding.
Normalize or standardize numerical variables: Scale numerical variables (e.g., MathScore, ReadingScore) to a similar range to prevent any single variable from dominating the analysis.

#### Feature engineering:
 Create new features if necessary, based on domain knowledge or data exploration.

#### Explore relationships: 
Analyze relationships between variables using techniques such as correlation analysis or visualization (e.g., scatter plots, histograms).
Perform statistical analysis: Conduct statistical tests or calculations to derive insights or validate hypotheses about the data.
Apply machine learning algorithms: Utilize machine learning models to predict or classify outcomes based on the available data.

#### Validation and Iteration:
Validate results: Validate the processed data and analysis results to ensure accuracy and reliability.
Iterate if necessary: If insights are inconclusive or further exploration is needed, iterate on the data processing steps or consider additional data sources.

#### Documentation:

•	Document data processing steps: Document each step taken during data processing, including any decisions made and the rationale behind them.
•	Document analysis results: Summarize key findings and insights obtained from the data analysis process.

## Data Processing:

One by one studying each features and its importance:

1. Ethnic Group :

What is it and why it is important?

The term "ethnic group" refers to a community or population that shares a common cultural heritage, ancestry, language, or other cultural traits. In the context of your data dictionary, "ethnic group" likely represents different demographic groups based on ethnicity or cultural background.

The specific ethnic groups included in your dataset are labeled as Group A to Group E. Without additional context or information, it's not possible to determine the exact composition or characteristics of each ethnic group. However, in practical data analysis, ethnic groups could represent various cultural or ethnic backgrounds such as African American, Hispanic/Latino, Asian, Caucasian, etc.

Why is it important and how it is effecrting my dataset?

Yes, the ethnic group can be an important factor to consider when analyzing its potential effects on test scores. Understanding how different ethnic groups perform on tests can provide valuable insights into educational disparities and help identify areas for improvement in educational policies and practices.

Here are some ways ethnic group might impact test scores:

Cultural Differences: Different ethnic groups may have varying cultural backgrounds, including attitudes towards education, study habits, and expectations for academic achievement. These cultural differences can influence how students approach learning and perform on tests.

#### Note: Similarly checking all the features and its importance.

#### Handling null values for each features:

As the no. of null values is very less in comparison to our original dataset.

So, we will simply drop the rows with null values.


#### Removing all the unnecessary columns:

Such as unnamed: 0

#### Creating plots for each features and checking its values and making conclusions:

After plotting graphs of each features I have made below conclusions:

1. The number of males exceeds the number of females.

2. The majority of students belong to Group C ethnic group.

3. A small proportion of students have parents with higher education.

4. A larger portion of students are receiving standard food.

5. Few students are participating in test preparations.

6. The majority of students' parents are married.

7. Students are actively engaged in sports.

8. Being the first child does not significantly affect student performance.

9. Most students utilize the school bus for transportation.

10. Out of 19,000 students, 10,000 are studying for 5 to 10 hours weekly.


## Creating some analytical questions to check how each features may affect students test score:

Here are some questions you can consider for each feature to explore how they may affect students' test scores:

1.	Do males tend to score higher than females on tests, or vice versa?

2.	Is there a significant difference in test scores between male and female students?

3.	Are there variations in test scores among different ethnic groups?

4.	Do students from certain ethnic groups consistently outperform others?

5.	Does the level of parental education correlate with students' test scores?

6.	Do students with parents holding higher degrees tend to perform better academically?

7.	Are there differences in test scores between students receiving standard lunch and those receiving free/reduced lunch?

8.	Does access to standard food affect academic performance?

9.	Do students who complete test preparation courses perform better on tests compared to those who don't?

10.	Is there a correlation between test preparation and improved test scores?

11.	Does the marital status of parents influence students' academic performance?

12.	Are students with married parents more likely to achieve higher test scores?

13.	Does participation in sports impact students' test scores positively or negatively?

14.	Are students who regularly participate in sports more likely to excel academically?

15.	Does being the first child in the family affect academic performance?

16.	Are first-born children more or less likely to achieve higher test scores compared to non-first-born children?

17.	Does the mode of transportation to school have any effect on students' test scores?

18.	Are students using the school bus more or less likely to perform well on tests compared to those using private transport?

19.	Is there a correlation between the number of weekly study hours and test scores?

20.	Do students who study more hours per week tend to achieve higher test scores?


## Conclusions:

1. Male students demonstrate stronger performance in mathematics, while female students exhibit higher scores in reading and writing.

2. Group E consistently outperforms other ethnic groups across all subjects.

3. Students with parents holding higher education degrees, particularly master's degrees, show superior academic performance compared to their peers.

4. Students receiving standard lunch perform better academically than those receiving free lunch.

5. Completion of the Test Preparation course correlates with higher test scores compared to students who have not completed it.

6. Marital status appears to have no discernible impact on student performance, as indicated by the graphs.

7. Students who engage in regular sports participation tend to achieve higher scores compared to those who participate occasionally or not at all.

8. Whether a student is the first or last child in the family does not significantly influence their test scores.

9. Students who dedicate more hours to weekly study sessions tend to achieve higher test scores.

### In wrapping up, let's answer few more questions:

1. How effective is the test preparation course?
   - The efficacy of the test preparation course is evident. Male students notably improved their writing scores after participating in the course.

2. Which major factors contribute to test outcomes?
   - Key contributors to test outcomes include lunch type, participation in test preparation, and gender. Male students tend to outperform their female counterparts in math tests, while females excel in writing and reading tests. Notably, lunch type had the most significant impact on math test scores.

3. What would be the best way to improve student scores on each test?
   - As discussed earlier, the test preparation course proves beneficial. However, it's important to note that while factors like lunch type, participation in test preparation, and gender play a role, the provided features alone may not fully elucidate the factors influencing student test performance. Further exploration may be necessary to identify additional contributing factors.
