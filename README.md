for starting the tomcat server you can go to where you have installed the tomcat.
in the conf directory you can add the settings and configs you want to your tomcat server.

for the maven to be able to connect to tomcat you should declare some roles in the tomcat `tomcat-users.xml` file. And as the default username and password for the maven to connect to the tomcat is:

        username = admin
        password = ""

you have to set these settings in the tomcat `tomcat-users.xml` file.

and also you can use this pluginfor adding the apache tomcat to your pom file:

        <plugin>
    			<groupId>org.apache.tomcat.maven</groupId>
    			<artifactId>tomcat7-maven-plugin</artifactId>
    			<version>2.2</version>
    	</plugin>
