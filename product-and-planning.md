UofT - Special Olympics
===


## Product Details


### Q1: What are we planning to build

Our team is building a web based sport/competition results search engine for Special Olympics Ontario. Special Olympics Ontario offers nineteen different sports options that lead to more than 500 competitions with more than 26,000 active athletes and more than 50,000 athletes over the last 12 years.

The problem as outlined by the partner is that at present there is considerable historical information, but this information is only presentable on a tournament by tournament basis with no ability to quickly and accurately search for information on an individual basis in order to measure performance improvement over time, as [current search tool](https://youthgames2019.com/results) is displaying data in plain HTML or PDF format.

The information is currently locked into several separate systems, one for team sports, excel spreadsheets for some sports, and a proprietary software which stores information in SQL tables in non-normalized data blobs. This structure means that existing information can only be queried through these systems and that search tools are limited to querying the information from tournaments one at a time.

The partner has developed a data structure to move the information into a normalized data warehouse, but is faced with the challenge of creating a new search tool to query this information and present it in an easy to consume and useful format. With our website, users will have a fancy, responsive and user-friendly UI that will be accessible to athletes, their coaches, their family/fans and the organization. Also, users are able to search by three types, and search results for each of the following search scenarios:
#### By competition
    Results of different types of competition
	Teams involved (team coach, team athletes, etc)
	Final results (scores, ranking, etc)
	Competition Statistics (individual / box scores)
#### By athletes or teams
	Athletes/teams basic information
	Competition results (by competition history / sport)
	Performance History (based on results, personal bests, trends)
#### By sports
	Performance results by athletes competing in sports
	Linked to first two search types (which athletes/teams or competitions featuring those sports)
	Performance bests (i.e, records by event, distance, sport)

Users are able to further filter the results. For example, `Sports: basketball` and `Teams: Raptors` yields basketball competitions that only involved team Raptors.

Users will also be able to view different results by clicking the links. For example, by searching `Sports: basketball`,  `Teams: Raptors` shows, and team details will be shown by clicking  `Raptors`.

---

### Q2: Understanding target users

 The main target users are Special Olympics athletes across all 19 sports, their coaches, family, supporters of special Olympics athletes and also donors and sponsors of Special Olympics.

Special Olympics Ontario has approximately 26,500 athletes and 11,500 coaches and volunteers who are the primary audience for this tool. Athletes and Coaches will be able to use this tool to search results and improve their training plans.

In addition, athletes have numerous fans, family and friends as well as sponsors, donors and media who would benefit from being able to easily access this information.

Most athletes compete in multiple sports (The partner reports on average athletes compete in 2.5 sports each) which means that the immediate audience for this tool is more than 55,000 users.

The partner has emphasized that the primary target audience are athletes with intellectual disabilities, so the user interface will have to be highly functional, easy to navigate and easy to use with little to no explanation. Navigation will have to be easy and very accessible for people with disabilities and responsive to multiple platforms.


#### Example use scenarios:
1. Special Olympic athlete: Kate Poto, is a special Olympic Athlete that loves to spend time with her teammates. She is currently on a basketball team. Her team will have a game in summer, she wants to see her team on our website. However, she is not very good at reading and remembering complicated instructions, she wishes that she can get her information easily on our website.

2. Special Olympic Coach: Thompson River, is a coach for the Kamloops floor hockey team. He is inspired by the skills and selflessness of Special Olympics ON athletes. He also serves as a speech coach, helping Local athletes to develop speeches so they can represent Special Olympics in their community. To prepare for the summer season, he needs to gather data for his team, and he will need to use our website to see the performances of other hockey teams in Special Olympics.
 
3. Family of Special Olympic athlete: Franklin Poto, is the father of  Kate Poto. He is very proud that his daughter Kate is both a hockey and golf Special Olympic athlete. He wants to see all tournaments, both hockey and golf, that his daughter participated in.

---

### Q3: Why would users choose our product? What are they using today to solve their problem/need?
Special Olympics is dedicated to diversifying the life of people with intellectual disabilities via sports. However, there is currently no platform to display the result of those athletes' performance. We are building the very first product for Special Olympics which supports search with multiple criteria and display of events/ individual athlete performance. This is a bridge that connects the Special Olympics athletes to the rest of the society since their efforts and performance now can be heard and seen more often. The main purpose is to allow an athlete's family and coach to look up their athlete’s status and performance. Furthermore, our product also provides a way for potential donors to have a fairly accurate and close insight of this special community. 

Our product allows the user to choose a single or combined search criteria like sport category and team name. The search results are displayed in a user-friendly manner. Data is shown in a form that may be pre-defined by the user. In addition to data display, the product allows the user to download the search results in pdf and/or excel.



---

### Q4: How do we build it?
We are building a web-based app. For front-end, we will use a react framework and JS. For back-end, we will use a Flask framework and python. We will follow RESTful to design our API-end points.

This application architecture will also increase the flexibility for the organization to add on to the application as needs evolve in the future. It will also allow the partner to use the application in a variety of ways (embedded into existing sites or making the application available on other devices.)

As a team of seven people, we will follow an agile workflow and use Github as our version control tool. We are planning to create pull requests for each merge, and we will review each other’s code to imitate pair programming. The app will be deployed on partners server. We will be calling partners API to retrieve the data we need. We will have JS files for data virtualization and Util/controllers for communication connection to SQL database (partner provided).

Testing: we will make sure that authors don’t test their own parts. We will manually
test our app and/or writing scripts (UI: selenium API-endpoints: shell/python)

High level structure:

![highLevelGraph](https://user-images.githubusercontent.com/33362849/66795577-002d7500-eed3-11e9-81e8-07d03ef65bb5.png)



---

### Q5: User stories that make up the MVP

> **As a basketball athlete** who plays in the Special Olympics, I want to check my stats in certain games in order to know where my strength and/or weakness is.

Acceptance criteria:


1. Ability to specify completed game(s) by player’s name and date.
2. 	Ability to list the detailed stats of individual players in the game.
3. 	Ability to track down the stats for specific player(s) in the game.

> **As a soccer team’s coach** (Team Based Sports) in the Special Olympics, I want to check my teams’ stats in a certain period of time in order to make appropriate training plans.

Acceptance criteria:

1. Ability to specify completed game(s) by team’s name and given date(s).
2. Ability to list the detailed result stats of specific team.
3. Ability to list the detailed result stats of each individual player in the team.

> **As a Track and Field / Swim Coach (Individual Sport)** in the Special Olympics, I want to check my athletes' performance over time in order to keep track of personal bests and provide accurate and personal training plans.

Acceptance criteria:

1. Ability to search athlete performance by competition, sport and event (i.e. Track and Field, 100m Run) over time.
2. Ability to see detailed results for an athlete in a particular sport by event (i.e. multiple distances in swimming).
3. Ability to see personal bests.


>  **As a friend, fan or media,** I want to know the general information about certain competitions and search up the history of athletes competing in order to decide which competition(s) I should follow.

Acceptance criteria:

1. Ability to specify certain types of competition by age, sponsorships or locations etc...
2. Ability to list all the general information in the competition for example teams’ coaches, teams’ players, schedules etc...

> **As a parent whose daughter is a swimmer**, I want to be able to see the results of my daughters competitions and have a space to celebrate and showcase her talent.

Acceptance criteria:

1. Ability to specify certain types of competition by age, sponsorships or locations etc…
2. Ability to specify teams’ general information in certain competition.
3. Ability to view a biography / competition history by athlete to see performance and improvements over time.
---

## Process Details

### Roles & responsibilities

##### Front-end Developer (technical)
* Design and implement User Interface (UI) through which the user interacts with the web-based app using frameworks, Javascript, HTML and CSS.
* Ensure user-responsive experience and user-friendly display of content.

##### Back-end Developer (technical)
* Design and implement RESTful APIs to handle search requests.
* Implement methods to search SQL databases and wrap up the search results as JSON object using server-side language (Python).
* Design SQL query to search single or multiple SQL Tables efficiently.
* Ensure robust backend processing by handling and logging various errors.

##### Full-stack Developer (technical)
* Work across front-end and back-end.
* Ensure smooth link between search request and response.

##### Q&A Developer (technical)
* Test page, methods and APIs for front and back end.
* Give feedbacks to developers and help debug.
* Ensure desired functionality and bug-free code.

##### Project Manager (non-technical)
* Communicate with the user regularly to intake user feedback and requests as well as inform the user of project progress and technical implementation.
* Notify the developers about the user requests and help to solve user concerns.
* Ensure the project stays within the scope and satisfies the user’s needs.

##### Scrum Master (non-technical)
* Organize regular team meetings.
* Document the development process.
* Build and maintain User Manual.
* Ensure the team members stay focused and follow the agreed-upon rules.

##### Product Designer (across technical and non-technical)
* Search the open-source resources and determine appropriate open source tools used by the project.
* Supervise the front and back end development and give timely technical advice to the developers.
* Help the project manager to use proper technical resources to implement the user’s requests.
* Ensure to resolve issues between user’s demands and technical implementation.


---

### Team members & associated roles

<i class="fa fa-user"></i> **Linyue Wu**:
* Tech role: front-end
* Non-tech role: Documentation
* Strengths: Python, JS, HTML
* weaknesses: Java, SQL, design

<i class="fa fa-user"></i> **Caiquan Shi**:
* Tech role: back-end
* Non-tech role:  Facilitator
* Strengths: sql, python, C
* Weaknesses: java,  javascript, communication

<i class="fa fa-user"></i> **Qi Zeng**:
* Tech role: front-end, Q&A
* Non-tech role: product designer
* Strengths: sql, python, Javascript, selenium
* Weaknesses: react, communication, java

<i class="fa fa-user"></i> **Ming Jin Lu**:
* Tech role: front-end
* Non-tech role: Graphic designer
* Strengths: UI/UX design, Front End website development, Adobe Illustrator, Photoshop
* weaknesses:	 Complex Algorithm designs, Back end, Data structure designs

<i class="fa fa-user"></i> **Weitong Luo**:
* Tech role: back-end 
* Non-tech role: project manager
* Strengths: Python, SQL operations, several MVC frameworks
* weaknesses:	 Front end, Javascript, designing 

<i class="fa fa-user"></i> **Yangfan LI**:
* Tech role: full stack, Q&A
* Non-tech role: scrum master
* Strengths: React/JS, css, selenium
* Weaknesses:  Database, Java, design

<i class="fa fa-user"></i> **Li Zhu**:
* Tech role: full stack
* Non-tech role: product designer
* Strengths: Javascript, Python, SQL
* Weaknesses: React, scrum, project management

---

### Team Rules

#### **Communications**

Our expected communication frequency is at least three times a week. WeChat group is our main communication channel. Video calls will be made when we are in major project transition phases. When a member has made a significant cahnge, or has found a significant problem on our project, it is his/her responsible to update his process in our WeChat group.

We will email our partner when it is needed to. If the problem cannot be addressed via email, we will arrange a video call that will fit into the partner's schedule. If it is an emergent situation, we will have to call our partner.

The partner has provided access to internal tools used by the partner for project management including Google Suites (A shared google drive), Office 365 and the partners project tracking should we require it. The partner has indicated that they are available to engage in standup meetings, and check-ins as required.

#### **Meetings**

Member that can not attend our weekly meeting will need to notify the team before Sunday. Every member will have to provide their email and phone numbers in wechat Group. If a particular member did not show up during meetings for no reason, other members will have to take responsibility for calling (or other methods to contact this person) to check in with the status of this person. For each meeting, one or more members are responsible to use [HackMD](https://hackmd.io), (a markdown editor) for note taking. This meeting notes will be uploaded to GitHub issues.


---

#### **Conflict Resolution**:



**Conflict:** The team is split into two parts where they each insist on their own ideas==

**Solution:** 
We will take a step back and list all the pros and cons of each method. The decision will be made in the interest of the project and our partner's requirement.

**Conflict:** One of the team members is non-responsive which severely affects the process of our project.==
**Solution:**
We will talk to that team member in person. If that person continues to avoid responsibilities, we will split that person's task to ensure the project goes smoothly. Then we will have to talk to the TA about the situation.

**Conflict:** One of the team members is unable to complete his tasks prior to the due date==

**Solution:**
We will reassign some of that person's tasks to other team members to ensure our progress is not behind. We will then talk to that team member and assign different types of tasks to that person according to his preference and abilities.

---

### Events

There will be weekly fixed personal meetings on Monday at 8:00 pm. Meetings will be held at an available study room at Gerstein library or Bahen. Meeting's agenda will typically include: Share our progress in terms of our own tasks and check if everyone is on their right track. Set the course of the project and make sure everyone understands the plan. 
We will have code reviews in every meeting if it's necessary.


---

### Partner Meetings

Online meeting, the first one on 10/10/2019, at 8:00 pm to 10:00 pm.
[Meeting notes link](https://docs.google.com/document/d/1uXJNWerh-7vM3B8sewZeb5sKa3IkQkl17zfe1OOznM8/edit?usp=sharing)

After the meeting, our group has decided to do a web-based project that allows people to access information and data revolving on Special Olympic easily and more conveniently. We have a general idea of what type of searches and general results will be presented on our website, and the expectation of this project in our partner end. The smaller details and data structure will need further discussion.

---

### Artifacts

We use github issues to keep track our progress, manage our task distribution, and list TODOs. [github issue link](https://github.com/csc301-fall-2019/team-project-uoft-special-olympics/issues)
Every Weekly meetings, we will spend our first 15 - 30 minutes to track our work status and set up a new milestone for our next week to complete. Members of our team will pick a focus, front-end, back-end, or both, based on their past experience and personal preference. When the weekly milestone is set, tasks will be divided up and assigned to each member. After the tasks are assigned, members will work individually. However, during next week’s Wednesday, each member will have the responsibility of updating the progress of their work in the wechat group. If a member is having difficulty completing on his/her task, his task will be simplified furthermore and be redistributed to all members of the team. During our weekly meetings, we will use [HackMD](https://hackmd.io) as a markdown editor for meeting notes. Every member can edit this markdown at the same time. After the meeting, one member will post our meeting note on github issues for record.


## Appendix and FAQ


**This is a resubmitted Deliverable 1:** We drastically changed the presentation of this deliverable to make this document more readable. We rewrote Q3, artifacts and did some minor editing in different parts of this document. 


