# Using Docker Compose with Elaine Voice

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

##### 2. Build the Docker Containers
Run the following command after cloning the submodules:
```console   
docker-compose build
```

### Deployment
Once the containers have been installed, the project will be ready for deployment. 

##### 1. Start the Docker Containers
Run the following command to start the containers
```console   
docker-compose up
```

### Development
Here are some useful tools to help you while developing!

##### Entering the docker container
Run the following command to find containers
```console   
docker container ls
```

After that use the following command to enter the container
```console   
docker exec -it <CONTAINER_NAME> /bin/sh
```

