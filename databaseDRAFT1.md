information gathered -> Child Name, Child grade(?), Child's teacher, Parent/guardian name, Parent/Guardin name2, date of conference, time slot of conference, parent email, parent email2

Example database with:
- 3 teachers
- 2 conference days
- first slot at 4pm both days
- last slot 530m day 1
- last slot 4:45 day 2
- 4 kids for each teacher (12 kids total)

Database Draft 1

**schedules**
__________________________________________________________________________
| ID          | day_id    | time_id     | student_teacher_id  |
| ------      |:-------   |  -----:     |-----:      |
|    1         |     1    |     1        |    1       | 
|    2         |     2    |     1        |    2       | 
|    3         |      2     |     1        |    3       |
|    4         |      1     |       3      |    4       | 
|    5         |       2    |       3      |    5       | 
|    6         |       2    |       4      |    6       | 
|    7         |       2    |      3       |    7       | 
|    8         |       1    |     3        |    8       | 
|    9         |       1    |     4        |    9       | 
|    10         |       2    |      5       |    10       | 
|    11        |        1   |       1      |    11       | 
|    12       |      2     |      7       |    12       


**days**
______________________________
| ID          | date        |
| ------      |:-------   |
| 1           | 2015/23/3   |
| 2           | 2015/24/3   |

**times**
______________________________
| ID          | slot   |
| ------      |:-------   |
| 1           | 4:00   |
| 2           | 4:15   |
| 3           | 4:30   |
| 4           | 4:45   |
| 5           | 5:00   |
| 6           | 5:15   |
| 7           | 5:30   |

**teachers**
__________________________________
| ID          | name            | email | password
| ------      |:-------   | ------      |:-------   |
| 1           | Emmet Brown     | Emmet.Brown@ops.edu | bcryptorsimilarM213 |
| 2           | Clara Clayton   | Clara.Clayton@ops.edu | b34232ptorsimilarM213 |
| 3           | Jules Verne     | Jules.Verne@ops.edu | bcryp342342imilarM213 |

**administrators**
__________________________________
| ID          | first_name | last_name            | email | password
| ------      |:-------   | ------      |:-------   |
| 1           | Gerald | Strickland     | Gerald.Strickland@ops.edu | bcryptorsimilarM213 |


**students**
______________________________
| ID           | first_name          | last_name
| ------      |:-------   | ------      |
| 1            | Marty | McFly         |
| 2            | Linda | McFly         | 
| 3            | Dave | McFly          | 


**guardians**
__________________________________
| ID          | first_name            | last_name | email | 
| ------      |:-------   | ------      |:-------   | --- |
| 1           | Lorraine  | McFly     | L.mcfly@gmail.com | 
| 2           | George  | McFly     | G.mcfly@yahoo.com | 

**students_guardians(Bridge)**
__________________________________
| guardian_id          | student_id |         
| ------      |:-------   |
| 1           | 1 | McFly     | 
| 2           | 2  | McFly     | 

**students_teachers(Bridge)**
__________________________________
|ID| student_id          | teacher_id |         
|---| ------      |:-------   |
|1| 1           | 1 | 
|2| 2           | 2 |
