# Spring REST API for CustomerTrack
  This application is a Spring REST API for the CustomerTrack which performs all the CRUD operations.
  
## 1)Technologies/Libraries used
- IDE: Eclipse 
- Server: Apache Tomcat v9.0
- Database: MySQL v8.0.27
- Testing the routes: Postman  v8.7.0
- The libraries used were added using dependecy injection (pom.xml), so the application was build using Maven. No XML configuration, the application it's all based on Java configuration.
	


## 2) Features
  The application it's a customer relationship manager which performs the next operations/request at the following routes:
	
| HTTP method      |                                  | CRUD Action |
| -----------------|----------------------            | ----- |
| GET              | /crm-rest/api/customers                   | Read a list of customers|
| GET              | /crm-rest/api/customers/{customerId}	    | Read a single customer |
| POST             | /crm-rest/api/customer                    | Create a new customer |
| PUT              | /crm-rest/api/customers             	    | Update an existing customer |
| DELETE           | /crm-rest/api/customers/{customerId}	    | Delete an existing customer |
  
  Also it has exception handling implemented to make sure that we can give the appropiate response in case of somebody sending a request with bad data coming in. We are using Controller Advice, in Controller Advice we will have exception handlers which will handle the exception and send back and error response as JSON.
