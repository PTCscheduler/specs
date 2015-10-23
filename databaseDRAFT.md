Example database with:
- 3 teachers
- 2 conference days
- first slot at 4pm both days
- last slot 530m day 1
- last slot 4:45 day 2
- 4 kids for each teacher (12 kids total)

Database Draft 1

schedule
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


day
______________________________
| ID          | date        |
| ------      |:-------   |
| 1           | 2015/23/3   |
| 2           | 2015/24/3   |

time
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

teacher
__________________________________
| ID          | name            |
| ------      |:-------   |
| 1           | Emmet Brown     |
| 2           | Clara Clayton   |
| 3           | Jules Verne     |

student
______________________________
| ID           | Child_Name          | Guardian_Name1   | Guardian_Name2   |
| ------      |:-------   | ------      |:-------   |
| 1            | Marty McFly         | Lorraine McFly | George McFly|
| 2            | Linda McFly         | Lorraine McFly | George McFly|
| 3            | Dave McFly          | Lorraine McFly | George McFly|
| 4            | Needles Something   | frank something | Sally franklin |
| 5            | Child Tannon        | Aunty Tannon | |
| 6            | Someone eles        | wallfower walter| | 
| 7            | other person        | Kado person |
| 8            | another person      | Kado person |
| 9            | little bear         | papa bear | moma bear|
| 10           | jack nursery        | goldy locks| |
| 11           | jill nursery        | goldy locks| |
| 12           | Humpty Dumpty       | Mother goose| |