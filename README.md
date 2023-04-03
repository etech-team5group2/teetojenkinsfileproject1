# teetojenkinsfileproject1

What is a Jenkins plugins?
Jenkins plugins are piece of  program that when installed on  a Jenkins Server or application, extend the functionalities of Jenkins beyond  initial configurations. 


 Name 5 jenkins plugins and their use cases
Blue Ocean plugins :
Docker Plugins :  This Jenkins plugin allows Jenkins to build , test and use (deploy)  docker images from the Jenkins pipeline .
SonarQube Scanner : 
Jacoco Pluggins:
Maven Integration:
PIT Mutation:
Docker Plugins for Jenkins:

What is the difference between a scripted pipeline and declarative pipeline?
A scripted pipeline always starts with nodes while declarative pipeline starts with a pipeline .
A scripted pipeline usually has stages and stage while a declarative pipeline has stages, stage and steps. 
In a scripted pipeline , agent is not specified or  used while in a declarative pipeline , an agent is used and specified after the word pipeline.

 Use generic syntax to demo scripted and declarative pipeline as code

What is a stage-level variable and how is it different from top-level variables?
Stage level variable is defined and used within a particular stage of a pipeline . It does not affect other stages in the pipeline. It is different from a top-level
Variable which is also known as the Global variable because top level variables are declared at the beginning of a script. Top level variables can be referenced or called at any stage or part within a script. 

What information does Jenkins need to integrate with the github platform?
Jenkins needs a service account to integrate with the github platform. This service account is basically the username and the password for logging on to github web Platform.
Username of the github account 
Password of the github account
How do you inject scripts into your pipeline?
Script can be injected directly into a Jenkinsfile created for a pipeline. For example a bash script can be injected into a Jenkinsfile by specifying  sh  before the command. Sh is to indicate that it is a bash script.
sh ‘ line of command  ’
Here, the pipeline script method will be used in creating the pipeline. This type of pipeline would run directly on the Jenkins Server or Jenkins application . There will not be a need for a source code management system. 
Another method is also to inject the script at the backend of the Jenkins server , which is the workspace of that particular pipeline. Then you will specify the absolute part for the script in your Jenkinsfile. In this method, the Jenkinsfile is placed  in the source code management Platform like github.

What are the similarities between a dependency and a plugin?
 A dependency is a library that is needed by the application you are building, at compile and/or test and/or runtime time.

A dependency is a piece of code or library that is required by a project in order to function properly. In other words, a dependency is a software component that the project relies on.
A plugin, on the other hand, is a piece of software that can be added to a project to provide additional functionality.

How do you configure service account credentials for Jenkins?
Go to your Jenkins Dashboard 
On the left pane , click on Manage Jenkins
Then on the Security tab , click on Manage Credentials
Click on Global
On the Global credentials (unrestricted), click on add credentials at the top of the page on the side.
Indicate the kind of credential to be added : secret file , secret text , username and password , SSH or certificate.
Input your choice of  username or password , upload certificate , secret and put an identification note on it
Click on Create. Your account would be created after this.

Problem2:
Build an N-STAGE Jenkins pipeline where N=number of group members such that each stage should represent members name

Use the git flow best practice and add a ReadMe file on your steps to contribute to a project
Steps to Contribute to a Project:
If you are contributing to a project for this first time , do the following: 
Go to your Organisation on github and create a New repository with the name of the intended project for proper identification.
Click on public to make this repository accessible to other collaborators and also click on add a ReadMe File.
On your local machine clone your git repository with the url from the github environment in a folder. You clone if you are working on the project for the first time. and cd into it.
Create a new branch, switch to the new branch and tag it with the name of the Jira Ticket for that change.
 Make your changes to the project.
Commit your changes and put a descriptive message (git commit -m “ clear and concise note that describes what the new branch is doing “ ) 
Push the changes to the remote repository 
Create a pull request and assign it to Senior Engineers for Review and Approval.
Each member should write a simple two steps of (ps -ef and sudo systemctl status Jenkins)
