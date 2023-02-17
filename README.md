# The Data and Result of Mock-Apache-Empirical-Study

This GitHub repro contains the raw data we collected as well as the results. We will explain how the data was collected and what tools were used.

## Basic Data Collection and Tool Uesd in RQS

You can see the corresponding README in the specific file

### [Raw Data in RQ1](RQ1)

### [Raw Data in RQ2](RQ2)

### [Raw Data in RQ3](RQ3)

### [Raw Data in RQ4](RQ4)

## In Result Files

### [RQ1_all_metrics.csv](RQ1_all_metrics.csv)

The file records some basic information about each project, such as the number of commits, etc. The left side is for projects that have not imported mock, and the right side is for projects that have imported mock. Each column has the same meaning, but the only difference is whether the mock is imported or not

| Column Name  | Description |
| ------------- | ------------- |
| Project Name |  Name of the apache project for statistics |
| commits |Number of commits for this project |
| contributors |Number of contributors for this project |
| releases | Number of releases for this project |
| .java Files, | Number of .java Files for this project  |
| LOC |Number of LOCs for all files this project |
| test Files, | Number of test Files for this project |
| test LOC, | Number of LOCs for test files this project  |
| 'Mock' imports, | The total number of files imported mock in the project |
| Mocking frameworks, | The total number of Mocking frameworks imported in the project|

### [RQ2_FrameworkRank.xlsx](RQ2_FrameworkRank.xlsx)

The left side is based on the raw data counted in RQ2. It records what mock frameworks have been used for each project.
On the right side, the top 4 frameworks are recorded in how many projects they have been used in and the percentage of projects that have used the mock.


### [RQ2_LibraryClassSummary.xlsx](RQ2_LibraryClassSummary.xlsx)

Count the number and percentage of internal classes vs external classes in a project that are mocked.


### [RQ3_EasyMockUsage.xlsx](RQ3_EasyMockUsage.xlsx), [RQ3_MockitoUsage.xlsx](RQ3_MockitoUsage.xlsx), [RQ3_PowerMockUsage.xlsx](RQ3_PowerMockUsage.xlsx)

These three files take a similar file structure


| Column Name  | Description |
| ------------- | ------------- | 
| method| The method of the current statistic, such as mockito's when()| 
| label|Manual labeling of method | 
| count | Number of times the method has been called | 



### [RQ4_CustromMockDestribution.xlsx](RQ4_CustromMockDestribution.xlsx)

The number of custom mock classes in each project was counted and it was concluded that there were 144 projects using custom mock classes and a total of 2,237 custom mock classes.

### [RQ4_44classes_select.xlsx](RQ4_44classes_select.xlsx)

We selected 2% of the 2,237 custom mock classes is 44 for manual analysis.

| Column Name  | Description |
| ------------- | ------------- | 
| Project| The project where the analyzed class is located | 
| java file| The java file where the analyzed class is located | 
| class|Name of the custom mock class being analyzed | 
| Inheritance| Whether this class has inherited behavior | 
| Isolation| Whether this class is doing isolation. (Is the concept of mock being used) | 
| Can use mock| Whether it can be refactored to mock | 
| Favor Mock| Whether or not favor using mock framework | 
| Reason| Explanation about labels | 
