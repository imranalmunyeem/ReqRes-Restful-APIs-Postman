# Project Name: 
ReqRes-Restful-APIs-Postman

## Project Description
This website contains different Restful API requests -- GET, POST, PUT, PATCH, DELETE

### Help + Testing
The steps below will show how you can run and test this project.

Step 1 --- Download and Install postman: (https://www.postman.com/downloads/)

Step 2 --- Signup and login to Postman

Step 3 --- Import this project (https://github.com/imranalmunyeem/ReqRes-Restful-APIs-Postman.git) in postman and open the collection file.

Step 4 --- Run the collection file from the collection runner in postman

### Report Making Guide
Step 1 --- check if node.js is already installed: Open cmd and write 
           node -v 
           npm -v
           
Step 2 --- Install nodejs (https://nodejs.org/en/download/)

Step 3 --- Install npm (https://www.npmjs.com/package/download)

Step 4 --- Run this command on windows cmd to install newman (npm install -g newman)

Step 5 --- Run this command on windows cmd to install newman html reporter (npm install -g newman-reporter-html)

Step 6 --- Run this command on windows cmd to run the collection and make html report (newman putcollectionnamehere -r html)

Step 7 --- To get more help on newman, visit here (https://www.npmjs.com/package/newman-reporter-html)

### Running from Jenkins
Step 1 --- Download and install Java and set the environment variable fot it (https://www.java.com/download/ie_manual.jsp)

Step 2 --- Download and install JDK 8 and set the environment variable for it (https://www.oracle.com/java/technologies/downloads/#jdk17-windows)

Step 3 --- Download Jenkins war file (https://www.jenkins.io/download/)

step 4 --- Go to the Jenkin's location, open cmd and write "java -jar jenkins.war" and it will run jenkins server on your local port 8080 (N.B: Don't close the cmd)

Step 5 --- Go there to use jenkins (http://localhost:8080/credentials/)

Step 6 --- Setup and login to your jenkins server.

Step 7 --- Go to 'Manage Jenkins' and then "Plugin Manager" and install all the recommended plugins.

Step 8 --- Click on "New Item" from the left side, Enter project name, select project type as your choice (Recommended: Freestyle)

Step 9 --- Running from local device: 
           -> Select source code management to NO
           -> Select 'Execute Windows Batch Command" from 'Build'
           -> Write the Current project location and collection name 
                C:\Imran\Testing\API Testing\ReqRes-Restful-APIs-Postman
                newman run collectionname.json
           -> Save 
           -> Build Project
           -> Click on plain text to see the plain view

Step 10 --- Running from Github: 
           -> Select 'Github Project" from 'General' and put github link
           -> Select source code management to Git
           -> Select 'Execute Windows Batch Command" from 'Build'
           -> Write the Current project location and collection name 
                C:\Imran\Testing\API Testing\ReqRes-Restful-APIs-Postman
                newman run collectionname.json
           -> Save 
           -> Build Project
           -> Click on plain text to see the plain view
        

