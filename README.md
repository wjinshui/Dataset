# Dataset
Db.sqlite is an SQLite database file, which contains all the data we collected in the experiment.

## Tables related to SQL statements submitted by students

Tables with names beginning with 'exercise_' are all related to SQL statements, and two of them are most important. 
One is the exercise_result table, which records most of the information related to the SQL statements submitted by students, 
and the other is the exercises_exercise table, which records most of the information related to exercises. 
**The student submissions are stored in the 'submitted_answer' field of the exercise_result data table.**


Table 1 Description of exercise_result table.

| Field | comment | datatype |
| :------:| :------: | :------: |
| submission_id  | Submission ID | INT |
| submitted_answer | SQL statement submitted by student | TEXT |
| submitted_time | Time of submission | NUM |
| answer | Reference statement provided by tutors | TEXT |
| exercise_id | Exercise ID | INT |
| is_correct | Mark whether the statement is correct | INT |
| score | Scores calculated by our model | REAL |
| student_id | Student ID | INT |
| type | Classification of statement | TEXT |
| difficulty | The difficulty coefficient of the exercise | INT |


Table 2 Description of exercises_exercise table.

| Field | comment |datatype |
| :------:| :------: | :------: |
| id  | Exercise ID| INT|
| short_title | short title of exercise |TEXT|
| preamble | description of exercise | TEXT |
| difficulty | coefficient of difficulty | integer |
| visible | whether the exercise is visible  | boolean |
| priority | the priority of exercise | integer |

## Tables related to SQL statements submitted by students
Please refer to db_schema.pdf for the database schema used in the experiment.

#
