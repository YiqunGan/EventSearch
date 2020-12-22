# EventSearch

-	Developed a web service with RESTful API using java servlets to handle HTTP requests and response.
-	Created relational database MySQL to store user information and the searched results returned from Ticketmaster API.
-	Designed recommendation algorithms by fetching user’s history database records.
-	Built an interactive website using HTML, CSS and JavaScript that can search for nearby events, save favorite events.
-	Used content-based recommendations algorithms based on categories of user history to match similar events.
-	Implemented business logic of the application with java, deployed the server and database in AWS EC2.

## Infrastructure 

- 3-tier architecture
   * Presentation tier: HTML, CSS, JavaScript
   * Data tier: MySQL
   * Logic tier: Java

## API Design
- Logic tier(Java Servlet to RPC)
   * Search
      * searchItems
      * Ticketmaster API
      * parse and clean data, saveItems
      * return response
   * History
      * get, set, delete favorite items
      * query database
      * return response
   * Recommendation
      * recommendItems
      * get favorite history
      * search similar events, sorting
      * return response

## Database Design
- MySQL
   * **users** - store user information.
   * **items** - store item information.
   * **category** - store item-category relationship
   * **history** - store user favorite history
