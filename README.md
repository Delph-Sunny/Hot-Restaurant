# Class Activity: Hot-Restaurant

:construction:   IN PROGRESS  :construction:  

---

## Description: 
Basic app demonstrating Node and Express with jQuery. Overall purpose is to help schedule reservation requests. Restaurant has just 5 tables available. First five requests get a reservation, every request after that is sent to the waiting list.
* Live Demo: <http://hot-restaurant.herokuapp.com/>
![Hot Restaurant Image](Images/HotRestaurant.png)
 * Phase I (15 min): For this first phase, aim to write out the pieces that will need to be programmed to create the functionality of your application. Try to break it into 6-7 pieces.
    * Create the front-end (visuals) for home page, reservation form, and reservation views.
    * Create a basic server using Express.JS
    * Create a few array variables that will hold the data
    * Create a set of routes for getting and posting table data
    * Create a set of routes for displaying the HTML pages
    * Use jQuery to run AJAX calls to GET and POST data from users to the Express server
* Phase II (*20 min): For this second phase, aim to complete the following:
    * Backend Team: 
      * Create a basic Express server. 
      * Your server at this point should do the BARE MINIMUM. (Effectively, it should just say: "Listening at PORT 3000" when the command `node server.js` is run.)
    * Frontend Team:
      * Create three HTML files one called `home.html`, another called `tables.html`, and another called `reserve.html`. Use dummy data and create pages similar to the one shown to you on the sample Hot Reservation webpage.
    * All: If you finish early, begin thinking about how the Data, API, and Routes should look.
 * Phase III (*40 min): For this third phase, aim to complete the following:
    * Backend Team: 
      * Create a set of variables (hint: arrays of objects) for holding the reservation and waitlist data 
      * Create a set of routes that then display this data as JSONs. Users should be given these JSONs if they visit the appropriate page (i.e. if a user visits `localhost:3000/api/tables` they should see a JSON of table data).
    * Frontend Team:
      * Temporarily join the backend team. Your task will be to create Express routes that display your HTML pages when a user visits the appropriate page. (i.e. if a user visits `localhost:3000/tables`... they should be shown the `table.html` page.) 
      * If you finish early begin creating the code necessary to convert your form data into JSON objects.
  * Phase IV (60 min): For this fourth phase, aim to complete the following:
    * Backend Team: 
      * Create the logic that handles reservation requests. Your code should work such that POST requests take in JSON objects, checks if there is any space left, then adds the JSON object to either the reservation array or the waitlist array. Your POST route should also respond to requests with a confirmation (true or false) of whether or not the requestor has a reservation (or is on the waiting list).
      * You should be using Postman to do all your testing at this point.
    * Frontend Team:
      * Begin to do serious research on AJAX. Specifically, focus your attention on how AJAX can be used to do both GET and POST requests. 
      * Then create the necessary code on your `tables.html` page such that it can retrieve data from the Backend Team's API. In essence you will be creating an AJAX GET request to retrieve the data.
      * Then create the necessary code on your `reserve.html` page such that it can send data to the Backend Team's API. In essence you will be creating an AJAX POST request to send the data. 
    * All: This is the most challenging part of today's activity. Be persistent! You can do this!
 * Phase V (20 min): For the fifth and final phase, aim to complete the following:
    * All: 
      * Complete any remaining functionality from the previous phase if you need more time. 
      * Then, thoroughly test your application for bugs. Check if there are any obvious ways to crash the application. 
      * Then, if you have more time -- begin to tackle any bonus of your choice.
![Diagram](Images/Diagram.png)
## Notes
* You will NOT need a MySQL Database for this exercise.
* Current app doesn't have admin handling. We'll deal with that at a later time.
* Don't separate the JavaScript from the HTML in the client-side code. (i.e. Don't use external JavaScript. If you do, you will need an additional line of code to configure the express server to know where the JavaScript is).
## Resources:
  * <https://scotch.io/tutorials/use-expressjs-to-get-url-and-post-parameters>
  * <https://scotch.io/tutorials/build-a-restful-api-using-node-and-express-4>