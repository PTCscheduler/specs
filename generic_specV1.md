#Generic Spec 
Not specifically functional or technical spec, a mostly comprehensive collection of what the software should do, content it keeps and how it should react.
##The goal of the software
Parent teacher conferences (PTC) happen twice a year in Omaha Public Schools(OPS), currently a parent signs up for a PTC via a peice of paper while talking to the teacher at open house. The time the parent signs up for in August is the time they are given for PTC's in October and Feburary. Changes are made via phone call to secretaries and post it notes delivered to teachers. This process can be streamlined and duplicated via technology.

The timeline and desires allows for two pushes of the prodcut, the first version to be usable by december 20th. And the second to be done thereafter.

To hopefully help there will be user stories/senarios through out this document. For reference the characters are the following:

George Mcfly - Father
Lorraine Mcfly - Mother
Dave Mcfly - son/brother
Linda Mcfly - daughter/sister
Marty Mcfly - son/brother
Biff Tannen - Marty's classmate
Gerald Strickland - School Office administrator
Emmet Brown - Teacher
Clara Clayton - Teacher

###First push of the software
Will focus on the usability/functions for the teachers and administrators and not for the parents. The content will be entered in ahead of time for administrators and teachers to use.

####User levels (version 1)
*Administrator* 
- Can do CRUD operations on all schedules
- creates a login with a @ops.edu email
- should be able to print a master list of all conferences (template to be given to us)

*Teacher* 
- can do CRUD operations on their own schedule, can not see other teachers schedule
- creates a login with a @ops.edu email
- should be able to print their own schedule
- should be able to print reminder slips
- send email reminder to parents

**Senario 1 **(Why the administrator needs complete access)
Lorraine Mcfly calls the office of the school and Strickland answers, the current time slot of 3pm for PTC won't work she'd like to change it to 4pm. Strickland asks what teacher and must log into the platform look up Dr. Brown sees that an 4pm doesnt work but 4:45 later does. Lorraine agrees and hangs up while Strickland changes Brown's PTC schedule. When Dr. Brown loggs into the platform again a notification appears at the top to the change. 

**Senario 2** (why the reminder functionality)
25% of Ms. Clayton's class does not have internet at home or the parent's do not have an email address. Since the parents signed up for these slots months ago she'd like to send notes home with the kids as reminders. But doesn't need to remind all of the parents with a peice of paper, she doesn't hate trees. Ms. Clayton logs into the system selects reminder slips from the menu, clicks students she needs the reminders for and hits print. She then goes to the reminders menu and clicks email reminders, checks the boxes by the students with emaill addresses and clicks 'send notification'.  

####The schedule (what this thing revolves around) (version 1)
On wednesday Feb 21 2016 from 4:30pm until 8pm

On thursday Feb 22 2016 from 1pm until 8pm

15 minute intervals

a parent is allowed one 15 min interval per child

information gathered -> Child Name, Child grade, Child's teacher, Parent/guardian name, Parent/Guardin name2, date of conference, time slot of conference, parent email, parent email2
####Reminders
*online*

*print*
printable pdf quater size notes of students 
-------------------------------------------
|                                           |
| to the parents of ___ childs name___      |                           
| 
| Your parent teacher conference is at      |                            
| 
| time____                                  |
|                                           |
| date____                                  |
| 
| with___teacher name___                    |             
____________________________________________