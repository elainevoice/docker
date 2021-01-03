# Using Docker Compose with Elaine Voice
> All default configs are set for production/live, development-environment changes should be build upon the prod/live configs.
## Getting Started

These instructions will get you a copy up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites
##### 1. Install the following software:
- [ ] [Docker](https://www.docker.com/)

### Installing
A step by step series of examples that tell you how to get a development environment running.

##### 1. Update submodules
After cloning the repository, navigate to the project folder and run the following command: 
```console   
git submodule update --init --recursive
```

### Deployment
Once the containers have been installed, the project will be ready for deployment. 
There are two deployment versions: local and production. The local build will provide a live-reloading node server, wherein the production server will build the application to a stand-alone html app.

#### Local

##### 1. Build the Docker Containers
Run the following command after cloning the submodules:
```console
docker-compose -f docker-compose.yaml -f docker-compose.local.yaml build
```

##### 2. Start the Docker Containers
Run the following command to start the containers
```console   
docker-compose -f docker-compose.yaml -f docker-compose.local.yaml up
```

#### Production/live

##### 1. Build the Docker Containers
Run the following command after cloning the submodules:
```console
docker-compose -f docker-compose.yaml -f docker-compose.live.yaml build
```

##### 2. Start the Docker Containers
Run the following command to start the containers
```console   
docker-compose -f docker-compose.yaml -f docker-compose.live.yaml up
```

### Development
Here are some useful tools to help you while developing!

##### Finding the name of a container
Run the following command to find containers
```console   
docker container ls
```

##### Entering the docker container
After that use the following command to enter the container
```console   
docker exec -it <CONTAINER_NAME> /bin/sh
```

##### Installing a new package
Enter the docker container.
```console
npm install <package>
```
