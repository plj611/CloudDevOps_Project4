[![CircleCI](https://circleci.com/gh/plj611/c4/tree/master.svg?style=svg)](https://circleci.com/gh/plj611/c4/tree/master)

### Project summary

This project is about a microservice API which is built by Python flask framework. The microservice is to provide predictions about housing prices using a pre-trained model according to several inputs such as average rooms in a home, highway access, teacher to pupil ratios etc,

The API microservice is containerized and to run in Docker and kubernetes environment.

### Service launch instruction

- Standalone:  `python app.py`
- Run in Docker:  `./run_docker.sh`
- Run in Kubernetes:  `./run_kubernetes.sh`

### Project files description

- Makefile: contains command to prepare the virtual environment, install dependencies and lint the build files
- app.py: the microservice file
- Dockerfile: contains instructions on how to containerized the microservice
- requirements.txt: dependencies for app.py
- make_prediction.sh: shell script to send json input to microservice for prediction
- run_docker.sh: shell script to containerized the microservice and run it
- upload_docker.sh: shell script to upload the containerized microservice to DockerHub
- run_kebernetes.sh: shell script to run the microservice in kebernetes cluster