# Integrate Mulesoft with GitHub and GitLab

## About the project

We write this tutorial to help junior developers to learn how to integrate their mule projects with their code versioning 
platform  
(using GitHub or GitLab). Here, you can find the steps you should follow to build and deploy the mule app to CloudHub.  
The mule app will be deployed (or re-deployed) on push.

## Table of contents

 - [Getting started](#getting-started)  
 - [Step 1 : configure the pom.xml by adding cloudHubDeployment configuration](#step-one)
 - [Step 2 : write the workflow to build and deploy](#step-two)
 - [Conclusion](#conclusion)
 - [Contribution](#contribution)



## Getting started <a name="getting-started"></a>
Make sure you have a GitHub or GitLab account before you start. If not, create one.  
  - **Prerequisites** :ok_hand:  
Create a new repository without any files (no read.me no .gitignore)  
Execute the git commands to make your mule project available on your git repository.  
```
git init  
git add .  
git commit -m "initial commit"  
git branch -M main  
git remote add <URL-of-your-git-repository>  
git push -u origin main  
```
Refresh to see the updates.

## Step 1 : configure the pom.xml <a name="step-one"></a>
Return to your workspace to Anypoint Studio and add a sub-element named <configuration> if you don't have one.  
Here, you should specify the different properties you need to set up the deployment on CloudHub.  
  - Url : https://anypoint.mulesoft.com  
  - muleVersion , the mule version you use  
  - Username : **MULESOFT_USERNAME**, your mulesoft username  
  - Password: **MULESOFT_PASSWORD**, your mulesoft password  
  - Application Name: name_of_your_app, it ***should be unique***   
    Tips: use your firstname  
  - Environment : “Sandbox”  
  - workerType: by default, “MICRO”  
  - Region: your region, ex:  “us-east-2”  
  - Workers: numbers of workers you need  
  - ObjectStorev2 : by default, “true”  

## Step 2 : write the workflow to build and deploy <a name="step-two"></a>
Use one of the templates corresponding to your platform.  
  
## Conclusion <a name="conclusion"></a>

## Contribution  <a name="contribution"></a>
If you have some suggestions, please send an email to : 
  
Thank you for reading and have fun with this wonderful word of code versioning control and continuous integration. :smile:    
