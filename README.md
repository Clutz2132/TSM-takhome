# TSM-takhome

# Scalable Web-Application Deployment on DigitalOcean
This project demonstrates how to build and deploy a scalable web application on DigitalOcean using Kubernetets. The application is built with Flask, containerized using Docker, and deployed on a Kubernetes cluster. The project includes setting up load balancing, autoscaling, and optimizing for cost and performance. 

## Features
- Containerized web app with Docker
- Deployed on DigitalOcean Kubernetes (DOKS)
- Autoscaling and load balancing
- Cost optimization strategies
- Easy to follow setup guide

## Prerequisites 
- DigitalOcean account
- GitHub account
- DigitalOcean CLI (doctl)
- Kubernetes CLI (kubectl)
- Docker

## Setup Instructions
Follow these steps to setup your environment and deploy the web application.  

1) Authenticate doctl with your DigitalOcean account
    doctl auth init
2) Create the Flask application
   A) Create a new directory for your project
      mkdir flask-app
      cd flask-app
   B) Create the app.py file with a "Hello World" Flask appication
        from flask import Flask
        app = Flask(__name__)
        
        @app.route('/')
        def hello_world():
            return 'Hello, World!'
        
        if __name__ == '__main__':
            app.run(host='0.0.0.0', port=80)
   C) Create a requiremnts.txt file for depenendices
      Flask
4) Dockerize the application
    A) Create a Dockerfile to containerize the app
      FROM python:3.8-slim
      WORKDIR /app
      COPY . .
      RUN pip install -r requirements.txt
      EXPOSE 80
      CMD ["python", "app.py"]
   B) Build the Docker image
      docker build -t flask-app .
   C)

   D)

   E)

   F)




   
