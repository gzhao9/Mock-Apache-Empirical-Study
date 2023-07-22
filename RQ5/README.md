# RQ5
## Data Collection
We use a Java parser script to scan each file for calss, and we record a class as a custom mock class if it meets the following three conditions
1. This file is a test file
2. This file not import the mock framework
3. The class in this file include the "mock" or "spy" Keywords.
## Data Interpretation
| Column Name  | Description |
| ------------- | ------------- |
| Project Name  | Name of the apache project for statistics |
| test file  | The test file to which the information recorded in the current line belongs |
|classes|The class name which include the "mock" or "spy" Keywords|
|path|The path of the analyzed class in the current project|
