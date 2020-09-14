# Special Olympics

## Description 
The application is a web based sport/competition results game search engine for Special Olympics Ontario. Users are able to search by three types including game, team and sports. With our website, users will have an easy-to-use and user-friendly UI that will be accessible to athletes that have Intellectual disabilities, their coaches, their family/fans and the organization. The main purpose is to allow the athletes, their families and coaches to look up their athlete’s status and performance. In addition, our product also provides a way for potential donors to have a fairly accurate and close insight of this special community.

The problem is that, at present, there is considerable historical information, but this information is only presentable on a tournament by tournament basis with no ability to quickly and accurately search for information on an individual basis in order to measure performance improvement over time, as current search tool is displaying data in plain HTML or PDF format.

This application is the solution not only because it is an accurate search engine, but also it is built in a way to accommodate people with intellectual disabilities, which is the main users of our application.

## Key Features
 There are three main features for our website.

1. Search games hosted by Ontario Special Olympics.
2. Search teams that have participated in Ontario Special Olympic games.
3. Search an athlete based on their SOOID or their name and provide their public information.
4. Display an athelet's personal profile when his/her name is clicked.

## Instructions

For our website users, they do not need any registration. All our data is provided by Special Olympic Ontario. Once our users have landed to our website (http://results.sooinc.ca), they can start the searching process. They can choose any field via search tabs to perform a search.
Game example: 2019 SOO Invitational Youth Games
Team example: Team Timmins, Napanee District SS (a dropdown will show up when users type in at least three characters)
Athlete example: 
    SOOID: 210177, 210055, 214336, 212544 etc. 
Other paramaters: Athletics/Track and Field; Lucas Rea; 2019-05-15
 
 ## Development requirements

All libraries used for the front-end are included in a package-json file under the folder special-olympics-ui. Developers need to `npm install` and set up all the dependencies. The front-end of this project is developed by React.js.

We are using Python flask to develop our back-end. We need to set up a virtual environment for our back-end development. The full documentation is located in our github issue “Backend environment set up #49”.



 ## Licenses 
After the publication of our project, we will still make our repository private and not adding any License to our project. The reason is that our project will contain both private and public information for more than 26,000 active athletes. We do not want any other individuals or organizations to have a hold of these information.