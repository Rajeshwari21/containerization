# Containerization.

#### Commands to build, run and publish the container to docker hub:
1. docker build . -t <your username>/docker-node-app
2. docker images (shows all the docker images)
3. docker run -p 49160:8080 -d <your username>/node-web-app
4. docker ps (Shows the status of the dockers images)
5. curl -i localhost:49160 (test the output of the nodejs docker image)
  
##### Process to publish your docker image to docker hub:
1. docker login
2. docker tag rajeshwari/node-web-app:latest rajeshwari21/buildnodewebapp (Creating a tag helps you to add a proper name and attach a version to it.)
3. docker push rajeshwari21/buildnodewebapp (this will push your docker image to docker hub).
