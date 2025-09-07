# what is DevOps??
* DevOps - development + operations 

# what is computer??
* Laptop/Desktop/Mobile/server is nothing but computing device

## let's say when we are  purchasing computer/mobile what are the things that we check
	* Processor
	* RAM
	* Storage
*	OS
We can call this as computer/mobile.

** Where it comes to server which includes the same but it's seems like black screen, 
only text but there is no graphics. where it comes to windows user interface everyting 
is graphics.

so OS is a Graphics + kernel which is Linux server not windows.

do we have Graphics in servers??
No right,why??

Bacically uses of Laptop/Desktop purpose is internet searching + development 
+ songs + videos etc.. as daily routine.
where it comes to mobile = Apps + internet + calling + songs + videos etc..
where it comes to server is used to serve the applcations 

why we are preferring servers??

if we use graphics = more memory + more power + more time
where it comes to  server = less memory + less power + less time + less cost

Client and Server architecture:
-------------------------------
In our internet world, everythig is computer right

let's say we have lawyer, we are clients for him
here lawyer providing legal services, so we are clients.
which means who gives info called service provider
			who requests info called client
if we take laptop and server
laptop is Client
server is facebook

In the same senario if we have laptop and mobile
mobile consists of some folders, so we are sending that folders to laptop.
In this case mobile is client
			 computer is server

if we are sending that folders from laptop to mobile.
In this case mobile is server
			 computer is client
			 

let's we discuss a small concept:
---------------------------------
stackholders --> who are the part of system
if we consider school which inclues students, parents and teachers.
and the target is ideally 100% studnts should get pass

50 years back:
---------------
only one final exam in a year

student = will not study from day-1
teachers = teachers may not focus to complete syllubus from day-1
parents = they always worried about their children from day-1

pass percent was very less

30 years back:
--------------
started conducting unit test-1, unit test-2, unit test-3, 
half yearly, unit test-4, grand test, final test.

student = will may study from day-1
teachers = teachers may focus to complete syllubus from day-1
parents = they not worried about their children

everybody will analyse the results.

out of 100 --> 30 members got 31% in unit test-1
so that they analyze where they are lagging and in the next exam they will rectify 
that to get good percentage.
unt test-2 -> 50%
unit test-3 -> 75%
Final exam -> 90% 

20 years back:
--------------
daily slip tests

day-1 -> teachers teach something from day-1
day-2 -> will conduct exams from intial

students = they start studying from day-1
teachers =  they start teaching from day-1
parents = they can see results from day-1

now the pass percentage will increase 99%

this is process improvement.

Take example as whatsapp, facebook.
from 2012 to till now, see the process improvement.

SDLC -> software development life cycle
1. Requirements gathering -> what customers wants
2. planning
3. Analysis -> Analyse the requirements
4. design -> start designing the project, customers will accept the designing
5. develop/implement -> implement the designing
6. deployment
7. test -> test the design
8. maintenence


waterfall model -> water is falling down

Once requirements are fixed we can't change

if we take house as example, construction is over but tesing is failed and the 
output is not as per design. we have to demolish the house and start again

disadavantages:
===============
it can't accomidate new requirements
final product output is only at the end

In IT stakeholders are developers, testing team, clients.

waterfall model(IT):
=====================
students = developers
teachers = testing team
parents = clients

developers, testing team, clients

so the time period of the project is 2 to 3 yeras.

developers = no development from day-1
testers = no testing from day-1
clients = worried

after 1 year they start serious development.
after that few employees is resign, new employees will come, we have to provide KT.
which is not possible to give KT about last one year work that we processed.

finally development started
testing team what to do --> they are reading 100's of pages from client requirements 
and planning test cases...
so the development is completed in DEV env, developers tested it is good

where it comes to testing team, they have to raise more and more defects

lets consider 2 years over only left for the project.

started fights between developers and testers

let's say 100 defects are there out of 80 valid, 20 defects invaid

lot of email's b/w developers and testers.. involving team leaders.. involving managers..
and project head.

even though no one happy.

but clients expets ferrari but they will get maruthi-800.

to over come this we got agile

Agile:
======
Final product -> multiple modules -> each sprint we ahve one module
start with small things --> keep short goals

devide the system into small modules:
sign up and login
product catalouge
cart
payment
delivery
shipping

sprints and modules

sprint-1 may be for 1 month:
-----------------------------
sign up and login

developers = they start from day-1 = 10 days for development
testers = 10 days for testing
10 days for deployment

let's say 10 defects are there out of 8 valid, 2 defects invaid

again discussion will happen b/w developers and testers

90% completed and 10% pending 

where we have daily standup calls
1. what you did yesterday, 
2. what are you going to do today,
3. Are you facing any problems

sprint-2:
---------
product catalouge

along with product catalouge we have to work on sign up and login

sprint-final:
-------------
if client expect ferrari at least they will get Honda city


internet revelotion started around 2016 right

so that all people are spending time on youtube, facebook, instagram etc..,

too much load on servers

but we need 100% solution right!!

In the same agile methodology process improvement has changed.

sprint-1 = process improvement:
-------------------------------
day-1 he developed a code for Enter your fist name 
day-1 ask this testing team to test this small code

lets say we have 10 test cases, like 

test case-1:
* enter the name in 20 charcterstics
* enter the numbers in the name field

like wise we have 10 test cases.

in this case no chance of raising invalid defects.
developers and testers will communicate daily.

if suppose they are 3 valid defects they will communicate in daily life

previosly what code they wrote they might be chances to forgot and when we are seeing 
invaid defects will some type of negative feeling.

DevOps: 
=> DevOps is a kind of agile methodology like it is the combination of 
   many tools and technologies and if the developed code is built, deploy and tested 
   on the same day is called devops.
=> We can achieve this using continous integration, continous delivery, continous deployment
=> We have to make sure that faster release to the market with less defects.

	1. Faster releases to the market(Speed)
	2. Less defects (Accuracy)
	
	Advantage of devops:
	---------------------
	we improve the communication between developers and testers and thier effeciency 
	become more. there are no fights between teams. the product delevery is 100% accurate.
	
long ago if we go to banks frequently they are telling 
like servers got down and under maintenance but now a days which is not much. 
the reason behind this is devops and cloud technologies.

And it is difficult to do manual testing so the we are going with automated testing
here we have build and deploment that is nothing but we have to bulid, then deploy 
it on servers then we have to stop the servers and start the servers. 

if suppose 1.0 version is running
download the new version
stop the system
remove the old version
install new version
start the system

if we keep servers in on-primise 
it is difficult to maintain so that we are using cloud platform. if we need one server
from on-primise it will take 10days like that so if you keep infrastruture in cloud
and if you apply devops on top of it  then will become fully automated.

this deploment is time taking process, 
generally assume it will take 30 min for automation.
if we go with manually might be take 1 day also.

how much important two wheels for a bike, like DevOps and cloud are important 
for automation. if you use devops on onprimise you will not get 100% automation. 
if you are in cloud you think that no need of devops again you will 
not get 100% automation.