# challenge-docker
Challenge realized @BeCode

- Type of Challenge: `Learning`
- Duration: `4 hours`
- Team challenge : `solo`

## Summary
### Mission objectives
- Create your own Dockerfile.
- Build a Docker image.
- Run a Docker container.
- Add a Docker volume to your container.
- Manage your images
- Manage your containers

### The mission
You will reproduce the architecture of your collegues. Here it is:

/app
    |-docker
    |   |-Dockerfile -> your Dockerfile
    |-pipeline
    |   |
    |   |-model
    |   |    |-model.py -> print a number between 1 and 400
    |   |-preprocessing
    |   |    |-preprocessing.py -> print a numpy array
    |   |-utils
    |   |    |-utils.py -> print "in progress..."

### Must-have features
[x] A nicely commented Dockerfile
[x] The same directory structure as above
[x] There are no more images or containers on your system

### Nice-to-have features
[x] Follow the dockerfiles best practices

## Usage
To enjoy this beautiful docker's container you can use the following commands from the root directory of the project :

- Build the image : 

  ```docker build . -t challenge-docker -f docker/Dockerfile```

- Run the docker : 

  ```docker run -t challenge-docker:latest```

* Run the docker in interactive mode and access to it by ssh:

  ```docker run -it challenge-docker:latest bash```

* Run the docker with your local volume in place of the initial copy : 

  ```docker run -t challenge-docker:latest```

* Run the docker in interactive mode with your local volume in place of the initial copy :
  ```docker run -v $PWD/pipeline:/app/pipeline -it challenge-docker bash```

## Installation

To install and run this project, you will be sure that your environnement must satisfy the following requirements :

* Docker : see [docker documentation](https://docs.docker.com/get-docker/)
* Numpy 1.19.2

