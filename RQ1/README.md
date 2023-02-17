# RQ1
## Data Collection

The most raw data is from the GitHub links of all apache projects.
1. download the entire project and the log files by cloning the apache git repo.
2. use the understand sci tool to analyze the project.
3. use a script to initially analyze each project.

### [Per-project-commit-date-statistics](../RQ1/Per-project-commit-date-statistics)

Obtained via log file, which records information about each commit. This includes the ID, author, author's email, and date.

### [Project-log-files](RQ1\Project-log-files)

Cloned log files from github. The original .log file is included. and the 2.log file with date information.

### [understand-files](RQ1\understand-files)

The .und file is obtained by the understand tool. You can get the dependencies of the classes in the project by using the understand script.


### [RQ1_AllMockFrameworks.csv](RQ1\RQ1_AllMockFrameworks.csv)

The number of files that have been imported into the mock and the number of test files in each project are recorded.
We define the file that imports the package of UnitTest as the test file.