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


## Step 2: Create Docker image for backend

Go to the Django API server directory and create a Dockerfile for the backend. Then build the Docker image. Finally, run the Docker container and check that the application is working properly.

## Step 3: Create Docker image for frontend

Go to the React front-end directory and create a Dockerfile for the frontend. Then build the Docker image. Finally, run the Docker container and check that the application is working properly.

## Step 4 : Create a Kubernetes Deployment

Now you have two Docker images for the backend and frontend, you can create a Kubernetes deployment for each of them. Deploy the backend and frontend to the local Kubernetes cluster using Minikube. Check that the applications are running in your kubernetes cluster.

## Step 5 : Create a Kubernetes Service

Create a Kubernetes service for each of the backend and frontend deployments. Check you can access the application from your browser.


