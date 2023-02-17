# RQ2
## Data Collection
This folder contains a record of the number of times the mock framework has been used in each project. We use JDT to detect the import file in each file. If this file imports and calls the package of a mock, the mock is recorded as having been used in this file.
## Data Interpretation

| Column Name  | Description |
| ------------- | ------------- |
| Project Name  | Name of the apache project for statistics |
| Mocking Framework  | statistics of the mock framework |
|Used in # of Files|Number of files that reference the change framework api|

### Example data.
| Project Name  | Mocking Framework  | Used in # of Files|
| ------------- | ------------- |------------- |
|abdera|easymock|5|

5 files use easymock in project abdera.