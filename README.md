Workfront Connector
==============================


INTRODUCTION
  This is a demo about pulling Hours charged to projects from WorkFront.
  
  HOW TO DEMO:
  1. Set the following system properties:
    a. URLName - This is the URL to the Workfront instance
    b. UserID = This is the User ID of your Workfront Account
  	c. Password - This is the Password of your Workfront Account
    d. Project - This is the project from which hours will be returned
    e. From Date - This is the Date for which hours logged (on or after) to the specified project will be returned.
  
  2. Include the wf-connector in a Mule project and complete the system properties. 
     Include an HTTP endpoint using port 8081.

  3. Run Mule project as Mule App
  
  4. From the browser type 'HTTP://localhost:8081/wf?project=poject name&fromdate=from date
    example : http://localhost:8081/wf?project=pz&fromdate=2015-04-18 will return the hours logged to project 'pz' on or after 2015-4-18.
  

HOW IT WORKS:
   - The connector logs into WorkFront based on the system properties
   - Hours logged to the specified project on or after the specified date retrieved and returned in a JSON Array.
