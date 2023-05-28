# Part 4: Setting up CI/CD Pipelines
## 1.0 Creating GitHub repository (containing server application & workflow files) for part 4 of the project1:

![image](https://github.com/nab1999/project1_part4_server/assets/126570628/a36a7bae-86de-41f0-833b-ed568802988d)

## 1.1 Creating “Server-CI.yml” file & its contents for GitHub actions:

![image](https://github.com/nab1999/project1_part4_server/assets/126570628/3bf08782-f4ac-4a35-b356-d5f0dc79303b)

## 1.2 Creating Actions secrets:

![image](https://github.com/nab1999/project1_part4_server/assets/126570628/783b74e4-215c-4b15-adf3-de8bc8939a61)

## 1.3 Pushing changes (committing) to run the GitHub workflow (Server-CI):

![image](https://github.com/nab1999/project1_part4_server/assets/126570628/cb1c43e4-92e7-4d41-94a7-4797baa0d2d6)

The “build” job basically builds the Docker image for server and then pushes it to the Docker Hub repository called “nab99/server-repo”.

### 1.3.1 Latest image pushed successfully to Docker Hub repository via GitHub actions:

![image](https://github.com/nab1999/project1_part4_server/assets/126570628/f480a0db-9ceb-4ee9-9d09-95f9f10f1ab3)

## 1.4 Creating “Server-CD.yml” file & its contents for GitHub actions:

![image](https://github.com/nab1999/project1_part4_server/assets/126570628/b0afa740-8a1f-4196-bfa8-1c9d79f86a4b)

This CD workflow will update the Docker Compose file, pull the new image, and deploy the updated services. Then the Slack notifications will be sent to the specified webhook URL to keep us informed about the deployments.

## 1.5 Configuring Slack webhook for deployment notifications:

![image](https://github.com/nab1999/project1_part4_server/assets/126570628/f0897e66-28a3-43d0-bd49-d0455097899b)

## 1.6 Creating Actions secret for Slack Webhook URL:

![image](https://github.com/nab1999/project1_part4_server/assets/126570628/8065730c-233f-41c6-be47-7f82bc3447e8)

## 1.7 Pushing changes (committing) to run the GitHub workflow (Server-CD):

![image](https://github.com/nab1999/project1_part4_server/assets/126570628/e42e3064-fa78-44d6-9d86-7535cd19e704)

## 1.8 Slack notifications successfully received:

![image](https://github.com/nab1999/project1_part4_server/assets/126570628/2fbe3279-c709-48f6-a612-723f6eeea51b)

