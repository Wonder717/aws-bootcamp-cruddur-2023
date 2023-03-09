# Week 1 — App Containerization

This week, i took the time to rewatch the live streaming session for Week 1 class on 'App Containerization' and followed along to implement the changes to package the application to be able to run in a container. This involved the following steps:

1. I created a dockerfile in the 'frontend-react-js' directory and 'backend-flask' directory. This dockerfile is essentially defining a step by step process on how the docker image is to be built. Each step is a layer that build on top of the other to create an image.

2. I also configured environment variables to store configuration information to get the app running.

3. I created a docker-compose.yml file in the root of the project directory. This file makes it possible for multiole containers to run.

Moreover, I implemented the frontend notification feature as directed to have that page working. I went on to update the docker-compose file to configure a data layer for cruddur to use both dynamodb and postgress. 

Furthermore, i picked a couple of productivity tips on how to ask for technical help by watching the video reccomended by Andrew Brown. This involved how to share code snippets using https://gist.github.com


Additionaly, I learnt about docker components i.e docker client, docker host(daemon), docker registry. I also learnt about managing and protecting secrets using AWS Secrets Manager and Hashicorp Vault. With regards to dockerfile, there is a docker security tool to mitigate against vulnerabilities in docker files stored in source repositories like github called Snyk which i also explored.

**Extra container security tools**
- AWS inspector is used for scanning amis for ec2 and images in ECR
- Clair an open source tool for scanning container images

Lastly, i installed the docker daemon on my machine so i have been able to build and run a couple of docker containers, and pulled/pushed some images from dockerhub as well as shown in the screenshot below.

![image](https://user-images.githubusercontent.com/85680026/224026858-a8718a6e-20b5-4c51-9484-44d5d808c812.png)



![image](https://user-images.githubusercontent.com/85680026/224028300-4c7169e2-069f-47d5-acd2-3c62865d8c10.png)



![image](https://user-images.githubusercontent.com/85680026/224027385-a9422448-873e-41d0-ab0c-cfce59896f73.png)


