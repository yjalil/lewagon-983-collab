# lewagon-983-collab
The goal of this repo is to get used to a team workflow in preparation for the projects week. If you are interested send me your git username so i can invite you as a collaorator.

## Target skills
* [Github fundamentals](https://youtu.be/HVsySz-h9r4)
* Share maintanable code for others, write tests and docs
* [Agile workflow](https://www.atlassian.com/agile/project-management/workflow)
*  Scraping 
* Handling data with pandas
* Database design and manipulation


## Main idea
After these weeks at lewagon, i believe it's time to put our new skillset to use in a real world app. This will help us get ready for project weeks, we'll waste less time on coordination and workflow setups if we start working on this aspect now. At this point each one of us is capable of coding small functions able to perform targetted tasks individually. The plan is to combine our work so that it builds up into a more complex feature. 

### The app
The app i am suggesting is a web scraper that receives a shopping list as input in csv format. Then it scrapes a supermarket's website (or multiple websites like [marjane](https://www.marjane.ma/)) looking for the products listed and returning their availabitlity and prices. This is the main feature for now, we might think of new ones as we learn more.  I'll make a little rudimentary interface so it looks nice to interact with (this is outside the scope of the bootcamp).

## Project Structure 
The app will have  a Client folder which is a frontend in HTML/CSS/Javascript it will render a few pages for the user. 
* A Landing page with an input to import a csv file and show results. 
* The usual error pages (404....)

The Server folder will hold the API code that will create endpoints for the user to interact with. We'll see this in the last weeks of the bootcamp :
* / : first endpoint example
* /<scrape> : endpoints that will be hit by the input button, more details as we progress 

## Getting started 
### Requirements
Everyone has python

clone this repo by running this command in your chosen folder :
`git clone https://github.com/yjalil/lewagon-983-collab.git`
go to the server folder :
`cd server`
run pip to install all backend required packages :
`pip install fastapi`

All set

### Running the app
back :
`cd server` then
`uvicorn main:app`
front
open index.html in your browser

If everything goes well you will be able to see these two pages on your browsers : 
![Server endpoint '/'](/screenshots/server.png)
![Interface main page](/screenshots/client.png)

### Git commands 

This is the basic workflow to contribute code, same we use in challenges :
* check modified files :
`git status`
* get the last changes if someone else changed the code 
`git pull https://github.com/yjalil/lewagon-983-collab.git`
* add your code to the staging area :
`git add <file>` or `git add -A`
* add a message to your code and commit
`git commit -m "<message>"`
* push the code to the remote repository
`git push https://github.com/yjalil/lewagon-983-collab.git`
 
 You can choose to create a pull request from github and merge the changes with the main branch if the conflicts check out. Feel free to push whatever you want, play around, this is a practice and it doesn't matter if you mess up the code. Git offers a way to revert commits if something goes wrong.

### Jira
I made a jira workspace for organizing TODO tasks. This is optinal just for fun to play around the Agile team concept. Any collaborator can assign a task to himself and work on it so that two people don't end up wasting time working on the same thing. You can create an [Atlassian account](https://www.atlassian.com/) and download Jira on your phone. Send me the Atlassian username so i can add you to the project (10 collabs allowed on the free version). You can create a task, report a bug, assign it, change its status to 'in progress' as you work on it, then 'finished' after you push it to git. The idea is to have a meeting, brainstorm, create small tasks like 'write function scrape_marjane_price()' and organise ourselves to get all the tasks done. The interface looks like this :
![Jira interface](/screenshots/jira.jpg)

 We'll edit this doc as we progress. Have fun everyone! 



