# Week 1 — App Containerization

This week, i took the time to rewatch the live streaming session for Week 1 class on 'App Containerization' and followed along to implement the changes to package the application to be able to run in a container. This involved the following steps:

1. I created a dockerfile in the 'frontend-react-js' directory and 'backend-flask' directory. This dockerfile is essentially defining a step by step process on how the docker image is to be built. Each step is a layer that build on top of the other to create an image.

2. I also configured environment variables to store configuration information to get the app running.

3. I created a docker-compose.yml file in the root of the project directory. This file makes it possible for multiole containers to run.