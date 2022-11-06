# Overview

[![Python application test with Github Actions](https://github.com/vinodDE/Azure_DevOps_project/actions/workflows/python_app.yml/badge.svg)](https://github.com/vinodDE/Azure_DevOps_project/actions/workflows/python_app.yml)

This project is to build and demonstarate the capabilities of CI/CD pipelines using Azure and git technologies/tools and following agile methodologies. 

## Project Plan

please see below trello board and spreadhseet to go through the project plan and timelines.
https://trello.com/b/VWo4Dkj5/azuredevopsproject

* A link to a spreadsheet that includes the original and final project plan>

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
![image](https://user-images.githubusercontent.com/116422392/200165719-77bf97cd-9e9d-4456-a9b6-42f2a8fdd94a.png)




3) run make all and make sure that all tests run fine
4) 


* Project running on Azure App Service

* Project cloned into Azure Cloud Shell

* Passing tests that are displayed after running the `make all` command from the `Makefile`

* Output of a test run

* Successful deploy of the project in Azure Pipelines.  [Note the official documentation should be referred to and double checked as you setup CI/CD](https://docs.microsoft.com/en-us/azure/devops/pipelines/ecosystems/python-webapp?view=azure-devops).

* Running Azure App Service from Azure Pipelines automatic deployment

* Successful prediction from deployed flask app in Azure Cloud Shell.  [Use this file as a template for the deployed prediction](https://github.com/udacity/nd082-Azure-Cloud-DevOps-Starter-Code/blob/master/C2-AgileDevelopmentwithAzure/project/starter_files/flask-sklearn/make_predict_azure_app.sh).
The output should look similar to this:

```bash
udacity@Azure:~$ ./make_predict_azure_app.sh
Port: 443
{"prediction":[20.35373177134412]}
```

* Output of streamed log files from deployed application

> 

## Enhancements

<TODO: A short description of how to improve the project in the future>

## Demo 

<TODO: Add link Screencast on YouTube>


