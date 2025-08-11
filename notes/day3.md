# servlet
A servlet is a server side coding which is responsible for handling the request coming from the client side.
## servlet lifecylce:
1. init(): it is responible for loading the servlet into the servers memories when a request comes from the client.
2. service(): This method is responsible for processing the request and sending the respond back to the client.
3. destroy(): this method is responsible for unloading the servlet from the servers memories once its operation is over.

All this methods are present in a class called Generic Servlet.
this generic servlet class belongs to a package called javax.servlet

The genric servlet class doesnot have the support for http protocall As a result of this the servlet lifecycle was modified 
### The new servlet lifecylce consists of four methods:
1. init()
2. doGet()
3. doPost()
4. destroy()

this new cycle belongs to http servlet and this http servlet belongs to javax.servlet.http

![servlet](<WhatsApp Image 2025-08-08 at 15.04.47_d1b0bdf6.jpg>)

### steps for creating a web application
1. open netbeans
2. click on file
3. select new project
4. go to category javaweb and project  web Application

create a form which consists of following fileds
1. email
2. password
3. contact number 
4. security question
5. Answer
