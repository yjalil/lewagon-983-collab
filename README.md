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
![alt text](https://github.com/[username]/[reponame]/blob/[branch]/image.jpg?raw=true)
![Server endpoint '/'](https://github.com/yjalil/lewagon-983-collab/blob/main/screenshots/server.png)
![Interface main page](https://github.com/yjalil/lewagon-983-collab/blob/main/screenshots/client.png)
