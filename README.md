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
Follow these steps to setup your environment and deploy the web application. Code snippets are below and you can find more in-depth details in the step by step guide.   

1) Authenticate doctl with your DigitalOcean account
2) Create the Flask application
   - Create a new directory for your project
   - Create the app.py file with a simple Flask application
   - Create a requirements.txt file to specify dependendinces
3) Dockerize the application
   - Create a Dockerfile to containerize the app
   - Build the Docker image
   - Run the container locally to test
4) Push the Docker image to DigitalOcean
   - Create a contianer registry on DigitalOcean
   - Tag and push the Docker image
5) Create and deploy a Kubernetes cluster
   - Create a Kubernetes cluster
   - Deploy the application to Kubernetes
6) Expose the application
   - Expose the application with a load balancer to make it accessible externally
7) Enable autoscaling
   - Enable Horizontal pod autoscaling (HPA) based on CPU usage
8) Monitor and scale the application
   - Check the status of your cluster and pods
   - Scale the application
9) Cost optimization
   - Autoscaling with HPA and cluster technicques
   - Load balancing
   - Spot instances
   - Right sizing nodes based on resource utilization metrics
  
## Detailed stepp by step guide link
caymnlutz.com (fake)

## Conclusion 
This project demonstrated how to deploy a scalable, containerized web applicaiton on DigitalOcean using Kubernetes. 



   








