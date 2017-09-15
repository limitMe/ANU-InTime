

#### Procedure if students want to generate their timetable manually:

1. Log in Wattle with username and password. Then selected courses can be seen at:

https://wattlecourses.anu.edu.au/my/

2. Click specific course, like 

https://wattlecourses.anu.edu.au/course/view.php?id=20810

pay attention to "LECTURE ENROLMENTS HERE", and "TUTORIAL", click and you can find the group selecting page.

3. From the group selecting page, the specific lecture and tutorial can be seen, as well as their time and location. For more information, query with id at:

http://timetabling.anu.edu.au/sws2017/


#### Function of the app

- Update timetable
- Present timetable

#### Overall of Update Workflow

Since Wattle didnot provide any APIs, after analysed its webpages, I realized that datas and styles are binded together at server side, and it will be hard if I want to form up special requests because too many paras was added. So the solution has to become rather inelegant, I will use a hidden UIWebView load the page, extract data from DOMs using JavaScript.

The overall workflow looks like below:

![Overall of Update Workflow](/images/Update%20Workflow.png?raw=true)