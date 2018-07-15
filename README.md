# swChallenge
For Software or Web Development Challenge

This small project - webMailClient using SendGrid and MailGun.
This project is built with Spring-Boot technology, and thymeleaf as view template engine.
The webMailClient.jar file contains the classes, source files and template. a
It is a web-based project, which runs on Spring-boot applications.
Hence, please make sure you have all following dependencies in your classpath before running it. 
1. Apache Tomcat 7 or above
2. Spring-Boot starter jar files
3. Thymeleaf jar files
4. Spring Framework Javamail jar files

Moreover, I uploaded a webMailClient-src.zip file as well. 
Inside there is pom.xml, you may use it deploy the project using Maven. Or unzip it into Spring Tools Suite or eclipse (support Spring-boot)
The application.properties set the tomcat server listening port to 8088. You may change it to your prefer listening port. 

This web-mail sending application uses SendGrid as primary server and MailGun as secondary. 
If the primary mail server is down, the secondary mail server will be used. This is handled by the EmailSendController class.
This project uses the Javamail package provided by Spring Framework. 
The reason is I want to make sure I use Spring technology as much as possible.

Usage
-----------
1. In your browser, type http://localhost:8088/
2. Type in the recipient(s) email address, cc and bcc as well if you have. 
   Take Note: Please use comma(,) if you have more than one email address to deliver the message
3. Type in the subject of the email
4. Write your message in the text area provided
5. Click submit once you have done
6. You will be informed of the send status of your message

Things TODO
----------------
1. There is no further text validation or email address validation for the main webpage.
2. No login required in order to use this web email sender. Anyone can just use it.
3. To to check SQL or Javascript injection
4. Implement database to capture the message logs or history
