# Special Olympics 

## Iteration 02 - Review & Retrospect

 * When: Nov 11th 2019
 * Where: Bahen 2270

## Process - Reflection

#### Decisions that turned out well

1. Use Github issue and its label to assign work and have certain members to manage our documentation.
We were able to easily keep track of which specific feature and user story we are implementing and who we need to collaborate within our group to get work done.
2. Host meetings at least 3 time per week. 
We have made big progress every time we met. It is more efficient to communicate in person than have virtual meetings.
3. Designate certain members as UI designers.  
It made our UI easy to use and had the same style across all pages.

#### Decisions that did not turn out as well as we hoped

1. Use Github PR to resolve merge conflicts. 
Team members were having trouble using git smoothly since most of them are fairly new to the Github. It brought in many problems so sometime we just pushed to our dev branch directly.
2. Assigned four people as front-end developers whereas the back-end had a heavier workload and was a bit short-handed.
3. Trouble with deploying our app onto the partner's server due to the lack of knowledge and partner didn't want us to have too much access as it was also a production server.


#### Planned changes
1. Might assign one of the front-end developer to work on the back-end.
Our front-end is almost complete by now and yet more than half of the team is responsible for the front-end. We need more people to assist with the back-end developing. 

2. Communicate with our partner more regularly to make sure our deploy process is on the right track and also resolve some database issues.

## Product - Review

#### Goals and/or tasks that were met/completed:

1. Our first feature is that users can find all the games they have played and get a more detailed description of that game. Under tab Game, when opt in Search by ID, users can see all the games they have participated in by filling in their athlete ID.
2. Our second feature is adding an advanced filter that allows user to search the games that they have participated in. Under tab Game, when opt in Search by other parameters, users will select a sport type in the drop down menu and fill in their names and game date to get a list of games that satisfy all the parameters.
3. All the games are displayed in a table and users can click on a certain event to see the detailed game stats

<img width="1566" alt="Screen Shot 2019-11-16 at 16 53 12" src="https://user-images.githubusercontent.com/35976287/68999720-b00b4f00-0892-11ea-8fd5-0ec913da278b.png">
<img width="1566" alt="image" src="https://user-images.githubusercontent.com/35976287/68999725-cc0ef080-0892-11ea-8a4d-08c84f73ff74.png">
<img width="1566" alt="image" src="https://user-images.githubusercontent.com/35976287/68999730-f19bfa00-0892-11ea-8e26-a42de110da5f.png">
<img width="1680" alt="image" src="https://user-images.githubusercontent.com/35976287/69001018-e0a8b400-08a5-11ea-9e18-574a6d16ae9e.png">



#### Goals and/or tasks that were planned but not met/completed:
1. Under tab Team, implement search by team ID and search by other parameters.
We were unable to finish this because our partner did not give us the database associated with the team information until Nov 8th. 

#### How was your product demo?
After we have successfully connected the front-end with the back-end, we performed a few searches to make sure our implementation was correct by comparing the results with the database. We then had a small meeting to discuss the process of presenting our current work to the partner. Since our partner had an extremely busy schedule, we were only able to showcase our work via a voice call. We sent screenshots of our website while explaining to the partner how it works. 

Our partner accepted all the features and gave us a few suggestions. Since some users have intellectual disabilities, we need to display the desired result by requiring the simplest actions possible, for example, we might want to put 'search by ID' and 'search by other parameter' on the same page thus eliminating the opt button; and we also need to make bigger buttons so that it is easier to click.

The main takeaway is that, besides the functionality and the aesthetics, we also need to take the special needs of our target users into consideration. Making decisions based on our users' background and habit is a crucial element in developing.

## Meeting Highlights

Going into the next iteration, our main insights are:

#### Person's profile
When searching by a specific athlete ID, besides displaying all the games this person has played, this athlete profile should also be displayed on the same page. The profile should contain that athlete's name, the most recent event and link to that event, and that person's age when he/she attended each event.

#### Team's info
We will implement search results by team. Under tab team, users are able to either search by team name or other parameters including sports type etc, which will be decided by out partner's database. When searched by team's name, it will display that team's most recent events,  a link to each event and team members.

#### Competition info
When searching by a game name, we will be able to list all the events. 