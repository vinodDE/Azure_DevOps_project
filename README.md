# Overview

[![Python application test with Github Actions](https://github.com/vinodDE/Azure_DevOps_project/actions/workflows/python_app.yml/badge.svg)](https://github.com/vinodDE/Azure_DevOps_project/actions/workflows/python_app.yml)

This project is to build and demonstarate the capabilities of CI/CD pipelines using Azure and git technologies/tools and following agile methodologies. 

## Project Plan

please see below trello board and spreadhseet to go through the project plan and timelines.
https://trello.com/b/VWo4Dkj5/azuredevopsproject


## Instructions

Architectural Diagram:

![image](https://user-images.githubusercontent.com/116422392/199620324-cb4a5355-931c-4a1d-b5c8-6b3f4ee4a6e7.png)

![image](https://user-images.githubusercontent.com/116422392/200157769-09b96411-4059-44c6-9402-5dd4434c4fe3.png)


<TODO:  Instructions for running the Python project.  How could a user with no context run this project without asking you for any help.  Include screenshots with explicit steps to create that work. Be sure to at least include the following screenshots:

## Steps 

1) create a project in github.com and create makefile, requirement.txt, readme.md and others as required.
2) connect to cloud shell and clone project from git
![image](https://user-images.githubusercontent.com/116422392/200162495-606ec3ef-1f5a-49df-9468-952dbdb4d4f5.png)
![image](https://user-images.githubusercontent.com/116422392/200162609-a8671373-8a9d-4544-aeb1-6801c89db11c.png)
![image](https://user-images.githubusercontent.com/116422392/200164693-2eaefa20-0e23-4761-9414-86a9d5d841fe.png)
![image](https://user-images.githubusercontent.com/116422392/200162717-f5f4c639-f46e-43ae-9ebf-7e016ee5f5c1.png)
![image](https://user-images.githubusercontent.com/116422392/200164762-d5fba4ad-5783-427e-bd6e-2fd3beb9e4c0.png)

3) deploy webapp using azure cloud shell
![image](https://user-images.githubusercontent.com/116422392/200165719-77bf97cd-9e9d-4456-a9b6-42f2a8fdd94a.png)

![image](https://user-images.githubusercontent.com/116422392/200173955-40b79911-bd00-4785-aeaf-5979a06c531f.png)

![image](https://user-images.githubusercontent.com/116422392/200173977-1a0688bc-80ff-48a9-9bbe-4c431c2148af.png)

![image](https://user-images.githubusercontent.com/116422392/200187772-2cbdbee4-6c69-426b-93da-81c218f99704.png)


4) creating and setting up Azure pipelines and deploying sef hosted agent
  - log into https://dev.azure.com/ and create an organization and a project and setup service connetion.
  ![image](https://user-images.githubusercontent.com/116422392/200174832-f8ef8adc-d945-4ba9-a311-f32ecaea167c.png)
  
  - Install/enable the Azure Pipeline marketplace app and allow azure pipeline to access to all repos in github
  ![image](https://user-images.githubusercontent.com/116422392/200176133-e361b0fe-9a04-451d-9975-cfcc7a50aea7.png)
  ![image](https://user-images.githubusercontent.com/116422392/200176107-efa0b239-8ed3-408d-a7e9-324879ce62cf.png)

  - create azure pipeline agent
    
    create a PAT(personal access token) using https://dev.azure.com/ home and click on the top-right user icon, as shown below. once PAT created, make sure to copy  and save it.
    
    ![image](https://user-images.githubusercontent.com/116422392/200179907-5c77518a-9318-4899-b8e3-7bb87bf0fd75.png)
    
    Create an agent pool from project settings
    
    ![image](https://user-images.githubusercontent.com/116422392/200180212-ef30627a-297a-4aef-b501-e803ea673a90.png)

    Create a VM from azure portal and configure the VM as azure devops build agent using below steps
    
    - ssh <username>@<serverpublicip>
    - sudo snap install docker
    - sudo groupadd docker
    - sudo usermod -aG docker $USER
    - restart VM
 
    Go to the DevOps portal, and open the newly created Agent pool to add a new agent and follow below steps afrer logging back into VM.
    
    ![image](https://user-images.githubusercontent.com/116422392/200183534-48f07df2-37aa-4138-9104-2cf1be1d890a.png)
   
  ![image](https://user-images.githubusercontent.com/116422392/200182998-fecfa0f8-28fd-48d3-a541-1adb433c38c2.png)

  ![image](https://user-images.githubusercontent.com/116422392/200183045-a20e2505-0e11-4300-aeb8-2f39708b6551.png)

   
  5) Creating and deploying azure pipeline
  
      
    
   
  Successful run from azure pipeline
  
  ![image](https://user-images.githubusercontent.com/116422392/200184867-8e920e0d-3f53-4f18-8ff7-4de2e5c50fba.png)

  ![image](https://user-images.githubusercontent.com/116422392/200185839-aa88fcdb-e831-409c-aae8-594743f9d723.png)
  
  ![image](https://user-images.githubusercontent.com/116422392/200186241-a5df58e0-bd47-43e1-8450-22da3ea7dc83.png)

