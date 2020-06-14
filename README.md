# DevOps_Microservices
[![CircleCI](https://circleci.com/gh/shivamkrsarin1996/DevOps_Microservices.svg?style=svg)](https://circleci.com/gh/shivamkrsarin1996/DevOps_Microservices)

# Operationalize-A-MachineLearning-Microservice-API

## Project Overview

You are given a pre-trained, `sklearn` model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. You can read more about the data, which was initially taken from Kaggle, on [the data source site](https://www.kaggle.com/c/boston-housing). This project tests your ability to operationalize a Python flask app—in a provided file, `app.py`—that serves out predictions (inference) about housing prices through API calls. This project could be extended to any pre-trained machine learning model, such as those for image recognition and data labeling.

### Project Tasks

* Test your project code using linting
* Create a Dockerfile for the project
* Deploy  containerized application using Docker and make a prediction
* Improve the log statements in the source code for this application
* Configure Kubernetes and create a Kubernetes cluster
* Deploy a container using Kubernetes and make a prediction
* Use  CircleCI to indicate that the code has been tested


# Steps to run the projec
## Setup the Environment
* Create a virtualenv and activate it
```
python3 -m venv ./devops
source ./devops/bin/activate
```
* Run `make install` to install the necessary dependencies

### Running `app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run in Kubernetes:  `./run_kubernetes.sh`

### Kubernetes Steps

* Setup and Configure Docker locally
* Setup and Configure Kubernetes locally
* Create Flask app in Container
* Run via kubectl

# Files Structure
* Makefile  : contain information about steps to install all the  dependencies and make tests
* Dockerfile: contain application and dependencies all in a containarized form 
* run_docker.sh: steps to build and run dockerfile
* run_kubernetes.sh: contain steps to pull image and deploy container in pod and forward port of it 
* upload_docker.sh: contain how to push application image to dockerhub
* requirements.txt: contain all the dependencies packages 
