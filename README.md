# TSM-takhome

# Scalable Web-Application Deployment on DigitalOcean
This project demonstrates how to build and deploy a scalable web application on DigitalOcean using Kubernetets. The application is built with Flask, containerized using Docker, and deployed on a Kubernetes cluster. The deployment includes load balancing, autoscaling, and cost optimizaion. 

## Features
- Containerized web application using Docker
- Deployed on DigitalOcean Kubernetes (DOKS)
- Horizontal pod autoscaling (HPA) and cluster autoscaling 
- Load balancing
- Cost optimization strategies

## Prerequisites 
- DigitalOcean account
- GitHub account
- DigitalOcean CLI (doctl)
- Kubernetes CLI (kubectl)
- Docker

## Architecture 

Put snippet of diagram here


## Setup Instructions  

1) Authenticate DigitalOcean CLI
   
```
doct auth init 
```

3) Create Flask application
   - Create app.py file 

   ```
   from flask import Flask
   import os
   import socket

   app = Flask(__name__)

   @app.route("/")
   def hello():
       html = """Hello {name}!
       Hostname: {hostname}"""
       return html.format(name=os.getenv("NAME", "world"), hostname=socket.gethostname())

   if __name__ == "__main__":
       app.run(host='0.0.0.0', port=80)
    ```

   - Create a requirements.txt file

   ```
   Flask
   ```
  
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

## Conclusion 
This project demonstrated how to deploy a scalable, containerized web applicaiton on DigitalOcean using Kubernetes. 



   








