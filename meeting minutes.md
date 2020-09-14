Meeting Minutes 11/6/2019 with TA office Hour
===

###### tags: `Deliverable Meeting`

- **Location:** BA
- **Date:** Nov 4, 2019 8:00 PM
- **Agenda**
0. Deliverable 1 discussion with Adam `20min`
	Ming Jin Lu
2. Deliverable 2 discussion `5min`
- **Participants:**

    - Ming Jin Lu
    - Caiquan shi
    - Linyue Wu 
    
- **Contact:** Adam - "email"
- **Host:** Adamn
- **Reference:** - [CSC301 Meeting Minutes 11/4/2019, github divliverbale 1 md]


## Meeting Notes
### Office hour comments: 
- Ambiguous description of server and deployment.
- The process should be a 3.
- Q1, 2 are good
- Q3: rewrite. why tasks are important to users and important to Q1?
- for overall quality: get rid of all templates and bullet points. -> 80(lose the bullet points and use headers) 
- email Adam when done
- Mention GitHub issues under Artifacts

### Deliverable 2 discussion
- instructions in the readme -> talk about workflow, set some expectations, explain what are semi-working and what not. Work on the most important feature first
- quality part: justify why certain decisions are made, ex: lots of backends and simple front end to test out. 
- Complete at least one workflow. the show we have some functionality: filter data, choose a team, etc.

 Conclusion: We need a clear description and explanation of why we choose to work on our current components.


 # General Info
Date: Nov 11th 2019
Location: BA2270
Time: 9:00pm - 9:30pm
# Meeting Process
- Partner's clarifications:
    -  in the database, delegation is team
    - connection of the data tables: game delegation -> game people -> game events
- Data for team(delegation) is not complete thus affecting our implementation with user story 2
- Showed the partner our current UI
    - partner's suggestions: 
    1. make it convenient for the people with intellectual disabilities : make bigger buttons
    2. put the two search options on the same page
    3. instead of texts, use sports icons in the drop down menu
- deploy both front-end and back-end on the FTP


CSC301 Meeting Minutes 11/4/2019
===

###### tags: `Deliverable Meeting`

:::info
- **Location:** BA
- **Date:** Nov 4, 2019 8:00 PM
- **Agenda**
0. Future Meeting & NoteTaking Discussion `10min`
	> [name=Ming Jin Lu]
1. Deliverable 1 Feedback Discussion `20min`
	> [name=Weitong Luo]
2. MeetUp with Partner `45min`
3. Deliverable 2 progress update`20min`
4. Setup milestone for next step
(https://)
- **Participants:**
    - Weitong Luo
    - Ming Jin Lu
    - Li Zhu
    - Caiquan shi
    - Linyue Wu 
    - Yangfan Li
    - Qi Zeng
    
- **Contact:** Weitong Luo (weitong.luo@mail.utoronto.ca)
- **Host:** Ming Jin Lu
- **Reference:** - [Last week meeting minute]

:::

## Meeting Notes

:books: Future Meeting & NoteTaking Discussion
---
We will use HackMD for our future group meetings and partner meetings. We will also use this as a way to keep track of each member's tasks.


are there similar applications like to for other sports/leagues/teams?


:mag: Deliverable 1 Feedback Discussion
---
### What we can start Doing

- What happened in deliverable 1?
The result is not acceptable, 
One of the problems quoted below: 
> instead of providing technical details, try to explain the benefits of your software from a usability standpoint
>
 However, we did explain the benefits of our software quoted in  
> "In summary, the product provides the user more flexities to search and view data as well as is capable of handling multiple search requests efficiently and delivering precise search results."

Q4: Not Describing our architecture

> You did not describe the architecture

![](https://i.imgur.com/bDL4yYB.png)

Overall Quality: 
> Didn't remove templates & instructions

We specifically put in the instructions so separate our sections clearly (since we have a very long document)





- Remark request

:dart: Sprint Goal
---
- On the frontend side, we have created different components across different branches. In this 2-3 days, we need to merge these branches. On the backend side, we need the data's from our partner ASAP, and create the API (using Python Flask) that can transfer the data and results to the frontend.

:closed_book: Tasks
--

### Backend Team:
>[name=Li Zhu]
>[name=Weitong Luo]
>[name=Caiquan Shi]
Current API: 
Database:
Connection:

Current Status:
***Li Zhu*** -> Modified backend structure to be modularized: data services and database services. Data services are to handle requests and send a response. Database services are to manage the database like creating the table(s)
**Weitong** -> Setup environment and structure for Linux/Mac
TMR task -> make sure data mapping data to APIs


### Frontend Team:
>[name=Ming Jin Lu]
>[name=Linyue Wu]
>[name=Yangfan Li]
>[name=Qi Zeng]

Current Status: 

**Jin** -> Completed basic DisplayEvent component, but it is for individual games, need to create a component to display team games. Currently on branch display event info
TMR task-> Create new Component for team games, read in from JSON file

**Linyue** -> Able to display all searched events. Need to display them in a table and call 

TMR task -> Figure out data transfer between components

**Yangfan Li** -> Implement util function for front-end to send out http request.

Invisible component bug fixed, due to bootstrap version not match.

TMR task: -> search -> event lists -> eventDisplay


## Notes for Partner Meeting
<!-- Other important details discussed during the meeting can be entered here. -->
Our table does not have any data right now,
now should be the latest version of lucid chart

We don't have data until tmr morning?

Next Meeting with partner-> Saturday afternoon around 3 pm

Next Meeting with the group -> 11/5/2019 afternoon
 
# General info
- Date: Oct 26th 2019
- Time: 7pm - 9pm
- Location: room 2101, Gerstein Library

# Topics covered
- Use an admin to filter table access rights
- Potential ways to connect front-end and back-end: AJAX, Angular, etc.
- A close lookup on the data structure on lucid chart shared by our partner
- Several searching APIs including search by name, ID, team, etc.
- Next week's agenda
1. Two users stories are picked where they require search by athlete and team respectively
	- Search an athlete: input an SOid(unique)
	- Search a team: input a name/ a team id(unique)
2. implement front-end controller