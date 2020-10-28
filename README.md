# Introduction
I created this project for a team workshop (8 engineers) on October 27, 2020. Its purpose was to help our team learn development outside of the internal tooling and ecosystem. 

This project specifically is building a web server and helped me become more familiar with REST API development, Postman, IntelliJ, and design patterns.

# Setup
## Postman 
Download Postman: https://www.postman.com/downloads/  
Postman Collection URL: https://www.getpostman.com/collections/ff8bc66a38693b02dc71

## Code Repo
Download IntelliJ Ultimate: https://www.jetbrains.com/idea/
Open IntelliJ, clone this git repository by going to File > New > Project form Version Control

## Glassfish
Download Glassfish: download.oracle.com/glassfish/5.0.1/release/glassfish-5.0.1-web.zip (http://download.oracle.com/glassfish/5.0.1/release/glassfish-5.0.1-web.zip)  
Open your terminal and unpack the zip in your root directory.
```zsh
cd ~/Downloads
unzip glassfish-5.0.1-web.zip
mv glassfish5 ~
```
On your IntelliJ, configure the application server following these instructions: https://www.jetbrains.com/help/idea/creating-and-running-your-first-restful-web-service.html#app-server

**Make sure you set the AS_JAVA absolute path in the glassfish5 folder's asenv.conf!**

Now you should be able to run a local server by clicking the bottom tab bar of IntelliJ > Services > Glassfish > Run. You can try opening a web page with the local port or hitting the server using Postman. The URL should be something like this: http://localhost:8080/RestClientDemo-1.0-SNAPSHOT/tweets

![IntelliJ Web Server Running with Glassfish](img/intellij-server-running.png)