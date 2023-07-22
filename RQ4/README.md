# RQ4
## Data Collection
In RQ3, we counted the usage status of the TOP3 frameworks in different projects

## structure of the file


Folder name, such as [easymock](../RQ3/easymock),[mockito](../RQ3/easymock),[powerMock](../RQ3/easymock) records the corresponding mock framework.

The file name records information about each project. For example, powerMock/accumulo.csv records the number of times powermock is used in the accumulo project.

| Column Name  | Description |
| ------------- | ------------- |
|file_path|The location of the project's Java files |
|method|The mock method used in the file|
|api(Optional)|The Api package corresponding to the current mock method |


