# MavenDemoProject
Demo Project for Maven Learning

the setting.xml can be used for learning maven


So we can use nexus as a proxy to pull the jars from the central repository - for that in our project we have to use the repo of our nexus and the jars will be automaticall gets pulled from the central repo (https://repo1.maven.org/maven2/)

Prerequisite for that are -


1 - create a proxy for central repo using below conf

![image](https://github.com/mayankRepo01/MavenDemoProject/assets/83690350/714377cf-44a8-410f-bb7c-c806a076aae2)

2- create a nexus group in that add this this proxy and one nexus repo 

3 - in the project use just the group repo the jars will be pulled automatically from mvn central proxy and gets stored in nexus



4 - also there must be a server with id same as the repo id present in setting.xml with the cred

       <server>
            <id>nexus-group</id>
            <username>test</username>
            <password>test</password>
        </server>

This project can be used a example to test - in this group is already created 




