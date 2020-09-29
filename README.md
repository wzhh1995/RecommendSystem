Restaurant Recommend System
=======

## Introduction <br>
This is a full-stack web service to improve restaurant searching and recommendation experience based on personalized information <br>

## Purposals <br>
1. Created Java servlets with `RESTful` APIs and handle HTTP requests and responses <br>  
2. Designed the whole backend data model, built databases(`MySQL`, `MongoDB`) to capture real-time data from Yelp API <br>
3. Architected and implemented the interactive web frontend workflow utilizing `HTML`, `CSS` and `JavaScript`. <br>

## Architecture
* ### WebContent 
The frontend system which concludes: <br>
1. <b> index.html </b>: Main html page <br>
2. <b> scripts </b>: `JavaScript` for index.html (use `Jquery` and `AJAX` to simplify the web connection) <br>
3. <b> style </b>: `CSS` style for index.html <br>

* ### src 
The backend system which contains: <br>
1. <b> algorithm </b>: Recommendation algorithm. Firstly search items according to the categories of user's favorite items then sort by the distance <br>
2. <b> db </b>: The database program which has two versions (`MongoDb`/`mysql`). Use DBConnectionFactory to switch the database <br>
3. <b> entity </b>: Creat an Item class to filter the information that get from the external api <br>
4. <b> external </b>: Call api. TickedMaster API is used in this project. Use ExternalApiFactory can change API simply <br>
5. <b> rpc </b>: WebServlet program which use Restful API <br>
 SearchItem : Search nearby items by calling API <br>
 RecommendItem : Return recommendation items. <br>
 ItemHistory : Return the history of user's favorite items.<br>
 
 ## TODO
