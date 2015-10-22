#Generic Spec 
Not specifically functional or technical spec, a mostly comprehensive collection of what the software should do, content it keeps and how it should react.
##The goal of the software
Parent teacher conferences (PTC) happen twice a year in Omaha Public Schools, currently a parent signs up for a PTC via a peice of paper while talking to the teacher at open house. The time the parent signs up for in August is the time they are given for PTC's in October and Feburary. Changes are made via phone call to secretaries and post it notes delivered to teachers. This process can be streamlined and duplicated via technology.

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

###Second push of the software
Adding parent functionality to the equation.

####There will be three user levels ( version 2)
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

*Parents*
- 
-

####The schedule (what this thing revolves around) (version 2)
Must be able to:
- select month date year (typically a 2 day span)
- identify start time for each day (this varies per day)
- indentify end time for each day (this can vary per day)
- indentify time slot intervals (same span per slot likely 15 min)
- block out times for lunch _2 15 minute spans_
- reserve times for esl/translator bookings


