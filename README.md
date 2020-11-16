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

##### 2. Run Docker-Compose
Run the following command after cloning the submodules:
```console   
docker-compose up --build
```