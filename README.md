Workfront Connector
==============================


INTRODUCTION
  This is a demo about pulling Hours charged to projects from WorkFront.
  
  HOW TO DEMO:
  1. Set the following system properties:
    a. URLName This is the URL to the Workfront instance
    b. UserID This is the User ID of your Workfront Account
  	c. Password This is the Password of your Workfront Account
  
  2. Include the wf-connector in a Mule project and complete the system properties. 
     Include an HTTP endpoint using port 8081.

HOW IT WORKS:
   - The connector logs into WorkFront based on the system properties
   - Hours logged to projects are retrieved and returned in a JSON Array.
