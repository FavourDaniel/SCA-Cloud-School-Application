# SCA-Cloud-School-Application

This repository contains a Python file and Jenkins file for the first assessment exercise given to us at She Code Africa. It is solely for the task completion.

## Jenkins integration with repo
I made use of an EC2 instance which I created in AWS to directly install Jenkins and integrate my github repo to the job build ensuring to use a port 8080.

In the integration process, I created a Jenkins API token before configuring the repository. After that, I created webhooks in my Github repo as well as creating a Github token. To connect my Jenkins server with the webhook, I created an API token to authenticate from Github. Steps for this was clicking on my account, then selecting the configure option. Proceeded to selecting add new token, chose a name and generated the token.


## Configuring my GitHub repository
I created a Jenkins file with all stages declared for ease in creating the Jenkins pipeline to be triggered with the webhook. To create the webhook, I opened up my github repo and used the setting and added the webhook. Went ahead to generate a GitHub token that would be authenticated from Jenkins.

Going back to my Jenkins server, I configured the GitHub webhook and token. On completion of this process, I created a Jenkins pipeline to test my webhook then ran it manually so that the Jenkins job would be triggered by the webhook then created a new commit in my GitHub repo.

## Jenkins Credentials
The username is: favour
The password is: scacloudschool2022
My Jenkins server can be accessed at http://34.220.199.252:8080/ 

## Jenkins pipeline syntax
For the syntax, I started with a declarative pipeline, then made use of agent,stage agents and then a post section. The first stage shows what's happening in the job while the echo is the actual task being exected in the job. The pipeline is being built, then tested before its being deployed.
