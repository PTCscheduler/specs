information gathered -> Child Name, Child grade(?), Child's teacher, Parent/guardian name, Parent/Guardin name2, date of conference, time slot of conference, parent email{put where?}, parent email2{put where?} **it's not all in db :(**

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
| ID          | day_id    | time_id     | teacher_id | student_id  |
| ------      |:-------   |  -----:     |-----:      |-----:       |
|    1         |     1    |     1        |    1       | 10           |
|    2         |     2    |     1        |    1       | 6           |
|    3         |      2     |     1        |    2       | 3           |
|    4         |      1     |       3      |    3       | 4           |
|    5         |       2    |       3      |    3       | 5           |
|    6         |       2    |       4      |    3       | 2           |
|    7         |       2    |      3       |    2       | 7           |
|    8         |       1    |     3        |    1       | 8           |
|    9         |       1    |     4        |    1       | 9           |
|    10         |       2    |      5       |    2       | 1          |
|    11        |        1   |       1      |    3       | 11          |
|    12       |      2     |      7       |    2       | 12          |


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
| ID          | name            | email | password
| ------      |:-------   | ------      |:-------   |
| 1           | Gerald Strickland     | Gerald.Strickland@ops.edu | bcryptorsimilarM213 |


**students**
______________________________
| ID           | child_name          | guardian_id   | guardian_Name2   | teacher_id  (not needed technically) |
| ------      |:-------   | ------      |:-------   | :-------   | 
| 1            | Marty McFly         | 1 | 2| 2 |
| 2            | Linda McFly         | 1 | 2| 3 |
| 3            | Dave McFly          | 1 | 2| 2 |
| 4            | Needles Something   | frank something | Sally franklin | 3 |
| 5            | Child Tannon        | Aunty Tannon | | 3 |
| 6            | Someone eles        | wallfower walter| | 1|
| 7            | other person        | Kado person | | 2 |
| 8            | another person      | Kado person | | 1 |
| 9            | little bear         | papa bear | moma bear| 1|
| 10           | jack nursery        | goldy locks| | 1 |
| 11           | jill nursery        | goldy locks| | 3 |
| 12           | Humpty Dumpty       | Mother goose| | 2 |

**guardians**
__________________________________
| ID          | first_name            | last_name | email | student_id
| ------      |:-------   | ------      |:-------   | --- |
| 1           | Lorraine  | McFly     | L.mcfly@gmail.com | 1 |
| 2           | George  | McFly     | G.mcfly@yahoo.com | 1 |
