# SCA-Cloud-School-Application

This repository contains a Python file and Jenkins file for the first assessment exercise given to us at She Code Africa. It it solely for the task completion.

# Jenkins integration with repo

I made use of an EC2 instance which I created in AWS to directly integrate my github repo to the job build ensuring to use a port 8080.

In the integration process, I created a Jenkins API token before configuring the repository.

After that, I created webhooks in my Github repo as well as creating a Github token. To connect my Jenkins server with the webhook, I created an API token to authenticate from Github. Steps for this was clicking on my account, then selecting the configure option.
![1616798938131](https://user-images.githubusercontent.com/89241109/161636474-6587b5d0-84d0-42e8-b992-b916157a2492.png)

Proceeded to selecting add new token, chose a name and generated the token.
<img width="1116" alt="1616799438274" src="https://user-images.githubusercontent.com/89241109/161636636-0e5a83b7-55cd-415a-b77c-b2c5b5499b7a.png">


## Configuring my github repository
I created a Jenkins file with all stages declared for ease in creating the Jenkins pipeline to be triggered with the webhook.
