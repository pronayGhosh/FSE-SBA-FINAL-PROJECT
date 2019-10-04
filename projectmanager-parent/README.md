# FSD-SBA-FINAL-PROJECT:Project Manager
<h2>Associate Name:Pronay Ghosh Cognizant ID:426184</h2>
<h2>Please refer to the "docs" folder which contain the following sub-folders</h2>
<ol>
	<li>Application_Screenshots : This contains application screenshots of all screens.</li>
	<li>MySQL Script : This contains table design and the DDL commands </li>
	<li>Emma_Coverage_Reports : This contains the junit test cases, emma code coverage report and screenshots.</li>
	<li>Load_Testing_Reports : This contains the screenshots of the jmeter execution on the rest end-point designed</li>
	<li>Docker : This contains the docker commands and screenshots of the project docker image creation and execution.</li>
	<li>Jenkins : This contains the screenshots of the jenkins pipeline creation,execution and the build report</li>
</ol>
<h3>Following are the projects which comprise of the full-stack project:Project Manager</h3>
<ol>
   <li><h4>"projectmanager-server" - The spring boot project using Rest API,hibernate etc running in the back-end </h4></li>
   <li><h4>"projectmanager-web" - The angular project using HTML5,CS3,Bootstrap4 running in the front end</h4></li>
</ol>
<h3>Instructions for cloud lab VM:</h3>
<ul>
<li>8.	The full stack projectmanager jar file(post-build) is present in the path /projectmanager-parent/projectmanager-server/target/.</li>
	<li>In order to run the application, open a command prompt(cmd.exe),navigate to the jar path mentioned above and run the command:java -jar jarname</li>
	<li>Open a web browser(google chrome) and use the URL:https://localhost:9090 to access the application</li>
</ul>
<h3>Final Build Commands:</h3>
<ul>
<li>Maven: clean install -e [The UI code is build using "frontend-maven-plugin" and is packed inside the JAR artifacts itself. Refer projectmanager-web pom.xml](Command is mvn clean install)</li>
<li>Docker: package docker:build[spotify "docker-maven-plugin" is used to create image in the remote docker. <dockerHost> configuration : pom.xml of projectmanager-server](Command is mvn package docker:build)</li>
</ul>

<h3>Local Deployment Commands:</h3>
<ul>
<li>Spring boot in projectmanager-server folder: spring-boot:run</li>
<li>Angular ui in web folder of projectmanager-web: npm install -> npm start</li>
</ul>

<h3>Jenkins:</h3>
<ol>
<li>GitHub Branches to build: */fullstack</li>
<li>Jenkins script Path: projectmanager-server/Jenkinsfile</li>
</ol>


