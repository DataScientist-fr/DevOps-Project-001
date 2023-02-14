# Todo List Application

This project is a full-stack web application that provides a platform to manage your todo tasks. The application is split into two parts: the Django API server and the React front-end.


## Django API Server

The Django API server is built with the Django REST framework (DRF) and is connected to an SQLite database. It provides the backend functionality for the Todo List application, including CRUD operations for todo tasks.

## React Front-End

The React front-end provides a user-friendly interface for the Todo List application. It allows you to view, create, update, and delete todo tasks. The interface is responsive and easy to use, making it simple to manage your todo tasks.

---


# Project : Dockerize and deploy to Kubernetes

In this lab, you will be cloning the Todo List application repository and deploying the Django API server and React front-end to a local Kubernetes cluster using Minikube.


## Prerequisites
Before you begin, make sure you have the following software installed on your machine:
- Git
- Minikube
- Kubernetes CLI (kubectl)
- Docker

## Step 1: Clone the Repository

Start by cloning the Todo List application repository to your local machine using the following command:

```
git clone https://github.com/DataScientist-fr/DevOps-Project-001.git
```

## Step 2: Run applications locally

Run django backend API server and react front-end locally.
Check the application is working properly.


## Step 3: Create Docker image for backend

Go to the Django API server directory and create a Dockerfile for the backend. Then build the Docker image. Finally, run the Docker container and check that the application is working properly.

Connect your local to docker to the minikube docker ([explanations](https://minikube.sigs.k8s.io/docs/handbook/pushing/#1-pushing-directly-to-the-in-cluster-docker-daemon-docker-env)) : 
```
eval $(minikube docker-env)
```

Once your docker image is working and your docker is connected to minikube. You can push your image in order to use it in your kubernetes cluster.

## Step 4: Deploy backend on Kubernetes

Create deployment and service for backend application. Check you can access the application from your browser.

## Step 5: Create Docker image for frontend

Go to the React front-end directory and create a Dockerfile for the frontend. Then build the Docker image. Finally, run the Docker container and check that the application is working properly.

> When you will deploy the frontend on Kubernetes (minikube), you will need to change the backend url in the frontend code. You can do it by editing the file `frontend/src/App.js` and change `127.0.0.1:8000` by the cluster url of backend application.

Once your docker image is working and your docker is connected to minikube. You can push your image in order to use it in your kubernetes cluster.

## Step 6: Deploy frontend on Kubernetes

Create deployment and service for frontend application. Check you can access the application from your browser.

Ensure your frontend is working properly with the backend.

---

## Step 7: Enhance the Kubernetes Deployment

### Step 7.1: Database on persistent volume
Handle volumes for backend application in order to have the database persistent (db.sqlite3).

### Step 7.2: Enhance docker images
Enhance backend and frontend docker build in order to have a smaller images (use [.dockerignore](https://docs.docker.com/engine/reference/builder/#dockerignore-file)).
