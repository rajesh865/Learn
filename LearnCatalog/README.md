Code Quality Reports :
--------------------
	   a)Requirements :
		-------------
		Java 1.8+
		Maven 
		Jacoco plugin in pom.xml file.

 
		b)To Run the Jacoco and send reports to SonarCube:
		------------------------------------------------
		Step1 :
		 > mvn clean test    // this will generate jacoco.exec file inside target folder.
		 
		Step2 :
		> mvn sonar:sonar  // this will load sonar libraries on local as one-time.
		
		Step3: 
		> mvn sonar:sonar -Dsonar.host.url=http://localhost:9000  // this will send the jacoco.exec to sonar server which is running on http://localhost:9000