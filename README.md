[![CircleCI](https://circleci.com/gh/khaledalhasan/udacity-boston.svg?style=svg)](https://circleci.com/gh/khaledalhasan/udacity-boston)
# Udacity Cloud DevOps Engineer Nanodegree project: Operationalize a Machine Learning Microservice API
## Project Overview

You are given a pre-trained, sklearn model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on.
This project tests the ability to operationalize a Python flask app—in a provided file, app.py—that serves out predictions (inference) about housing prices through API calls.
This project could be extended to any pre-trained machine learning model, such as those for image recognition and data labeling.

## Project Tasks

* Test the project code using linting.
* Complete a Dockerfile to containerize this application.
* Deploy the containerized application using Docker and make a prediction.
* Improve the log statements in the source code for this application.
* Configure Kubernetes and create a Kubernetes cluster.
* Deploy a container using Kubernetes and make a prediction.
* Upload a complete Github repo with CircleCI to indicate that your code has been tested.

## Clone the repository
```python

    git clone git@github.com:khaledalhasan/udacity-boston.git
    cd udacity-boston/
```
## Create a virtual environment inside the application 
```python

    python3 -m venv ~/.devops
    source ~/.devops/bin/activate
```
## Docker

- [Create a docker account](https://hub.docker.com/signup)
- [Install Docker](https://docs.docker.com/get-docker/)

verify installation:
```python
docker --version
```

## Install hadolint & Minikube

```python
wget -O /bin/hadolint https://github.com/hadolint/hadolint/releases/download/v1.16.3/hadolint-Linux-x86_64 &&\
    chmod +x /bin/hadolint
```

[Install Minikube](https://kubernetes.io/docs/tasks/tools/install-minikube/)

## Install Python modules

```python

   make install
    
```

## Run the application in Docker using

```python

    ./run_docker.sh

```

## Run the application in Kubernetes using

```python

    ./run_kubernetes.sh

```
