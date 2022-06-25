# Spring-Boot-Examples
This example is a Simple MVC Style app with only one Controller which renders the Home Page view.
You can run this by using the Maven wrapper with command ./mvnw spring-boot:run

The following is a simple diagramatic representation of Request and Response of Spring MVC:
![image](https://user-images.githubusercontent.com/95605325/175757025-1abaa4ab-6924-4972-ae8f-ba70f6116cef.png)

Here First the Client i.e. the User request's thorugh the Browser by typing the URL for e.g. let's say URL is http://localhost:8080/dashboard
After hitting enter the Request first goes to the Server(Tomcat, Jetty, any...) then the Server accepts the Request and forwards it to the
Dispatcher Servlet in the Spring App which will now handle the Further part of the app, which is resolving the Request.
Now when Dispatcher Servlet accepts the Request then it has to resolve it or find that which Controller in the app maps to the request to 
and for that purpose we have Handler Mapping which does this job of finding the particular method and when it finds the method, then it 
calls that method to perform the action and when it executes it then returns the view-name and passes the data into it.
After that Dispatcher Servlet will look for the view with help of View-Resolver which finds the specific view and data-binding is also done.
Then after the view is rendered as a Response back to the client and then on the Browser the Output is shown.
