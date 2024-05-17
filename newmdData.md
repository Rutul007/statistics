Here is an example of an attendance table for a database:


Table Name: attendance


| Column | Data Type | Description |
|------------------|-----------|------------------------------------------|
| id | INT | Primary key, unique identifier |
| student\_id | INT | Foreign key from the students table |
| course\_id | INT | Foreign key from the courses table |
| date | DATE | Date of attendance |
| is\_present | BOOLEAN | Indicates if the student was present or not|


Example Data:


| id | student\_id | course\_id | date | is\_present |
|----|------------|-----------|------------|------------|
| 1 | 123 | 101 | 2022-01-01 | true |
| 2 | 456 | 101 | 2022-01-01 | false |
| 3 | 789 | 102 | 2022-01-02 | true |
| 4 | 123 | 102 | 2022-01-02 | true |
| 5 | 456 | 102 | 2022-01-02 | false |


This table allows you to track the attendance of each student for each course they are enrolled in. In this example, student with id 123 was present for course 101 on January 1st, while student with id 456 was absent. On January 2nd, both students were present for course 102, while student 789 was also present.

