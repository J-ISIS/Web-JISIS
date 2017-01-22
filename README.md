# Web-JISIS

Web-JISIS is a Rich Internet Application (RIA) whose goal is to develop a web top application that has the responsiveness, and look and feel of J-ISIS.
Web-JISIS uses a Three-Tier Architecture
* Tier 1: At the client side, Web 2.0 technologies are responsible for the application's graphical user interface. AJAX is used to communicate between this tier and the application server in tier 2. Requests are sent with the URL using GET or POST data. Request and Re sult data are formatted using JSON, XML, or plaintext.
* Tier 2: the middle tier is also known as the application server, which provides the business processes logic and the data access. The server in the middle tier is a servlet container—a Web server capable of running Java-based Web applications (Tomcat, Jetty, etc). The J-ISIS services (the business rules) are coded in this tier using Java and the client part of jisis-core.jar library. Requests are passed as messages to the database server and results are returned. Sockets are used to communicate between this tier with the client and the database server through TCP/IP.
* Tier 3: the J-ISIS database server provides the business data. The J-ISIS database server is listening for request on port 1111, requests and results are passed as messages through TCP/IP.
