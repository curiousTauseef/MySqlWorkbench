# MySqlWorkbench  
This project is about the creation of a web-based GUI for MySql database.  
# Technologies Used:  
  **Front-End:** Html,CSS,JQuery Mobile.  
  **Back-End:** Java,Servlet,Apache-Tomcat-Server 8,MySql.  
# PREREQUISITES  
   Before you try to deploy this project on your system.make sure you have the following softwares installed and configured properly  
    1. jdk ver1.8 or higher  
    2. A Web/Application Server (Weblogic/Tomcat/Glassfish/etc).  
    3. MySql ver5.7 or higher configured to port no:3306 and localhost (If it is configured to other port/ip address,then make sure to   change these from "servletContextListener" file.)    
# HOW TO START THE APLLICATION/PROJECT:  
Now there is 2 ways to deploy this project:  

1. CREATING A .WAR FILE  
To create a .war file,open the terminal/command prompt.Navigate to the downloaded directory.Type the following command:
 `jar -cvf MyWorkbench.war`
A "MyWorkbench.war" file will created.Deploy it to the server.Check the respective Server's document on how to deploy a .war 
file on it.  

2. WITHOUT .WAR FILE  
Not every server support the deployment without .war file.Check whether the Server you are using has functionality to       
deploy it without a .war file.This method is for deploy on Tomcat ver-8 server only.Other Servers may have different       
method.Copy the download folder "MyWorkbench" to Tomcat/webapps" folder.Run your tomcat server.Visit the address           
htttp://localhost/MyWorkbench.You will be greeted with the Welcome Screen.

# Ver 0.1  
1.  Made use of JQuery Mobile for UI.  
2.  Added session for each login.  
3.  Added "sessionOut.html" page which will be displayed once the user's session is timed-out.  
4.  Added a clock to show current time on the "welcome-to-MySqlWorkbench" page.This clock is system dependent.

# Problems to be Solved in current Ver.  
1. Due to some reason,"index2.html" is running as intended in offline(i.e when running directly from system).However when it is used in application,the color on the page and "DateandTime.js" are not loaded properly.The page is needed to be refreshed to load these.
