# lewagon-983-collab
The goal of this repo is to get used to a team workflow in preparation for the projects week. 

## Target skills
* [Github fundamentals](https://youtu.be/HVsySz-h9r4)
* Share maintanable code for others, write tests and docs
* [Agile workflow](https://www.atlassian.com/agile/project-management/workflow)
*  Scraping 
* Handling data with pandas
* Database design and manipulation


## Main idea
After these weeks at lewagon, i believe it's time to put our new skillset to use in a real world app. This will help us get ready for projects' weeks, we'll waste less time on coordination and workflow setups if we start working on this aspect now. At this point each one of us is capable of coding small functions able to perform targetted tasks individually. The plan is to combine our work so that it builds up into a more complex feature. 

### The app
The app i am suggesting is a web scraper that receives a shopping list as input in csv format. Then it scrapes a supermarket's website (or multiple websites like [this](https://www.marjane.ma/)) looking for the products listed and returning their availabitlity and prices. This is the main feature for now, we might think of new ones as we learn more.  I'll make a little rudimentary interface so it looks nice to interact with (this is outside the scope of the bootcamp). There's a way to make an interface using Tkinter but it looks awful and a bit harder to style.

## Project Structure 
The app will have  a Client folder which is a frontend in HTML/CSS/Javascript it will render a few pages for the user. 
* A Landing page with an input to import a csv file and a send button. 
* A results page that will show a table of all prices and availabilities of the products. 
* The usual error pages (404....)

The Server folder will hold the API code that will create endpoints for the user to interact with. We'll see this in the last weeks of the bootcamp :
* / : landing page
* /results : display results of a list
* /<scrape> : endpoint that will be hit by the input button, more details as we progress 

## Getting started 
### Requirements
Everyone has python, you'll need to have nodejs installed.

clone this repo by running this command in your chosen folder :
`git clone https://github.com/yjalil/lewagon-983-collab.git`
go to the client folder :
`cd client`
run yarn to install all front required packages :
`yarn `
go to the server folder :
`cd server`
run pip to install all backend required packages :
`pip install -r requirements.txt`

All set

### Running the app
We need to run two servers  (back and front) in two seperate terminal windows and we keep them open (as we did for Jupyter) :
back :
`uvicorn main:app`
front
`yarn start`

This will enable us to run our code on the browser by typing the urls /localhost:8000/ and /localhost:3000/
/localhost:8000/docs will open swagger which lists all the endpoints of the api and a way to test them, this can also be done on postman
