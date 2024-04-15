# Flask Docker App
This is a simple Flask web application Dockerized for easy deployment. It provides a starting point for developing and deploying Flask applications using Docker containers.
## Getting Started
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.
## Prerequisites
 + Python 3.x
 + Docker

### Create a new application from scratch
#### 1.Create a directory with a name "Flask-Docker-App"
      mkdir Flask-Docker-App
      
#### 2.Navigate to the newly created directory
      cd Flask-Docker-App
##### 3.Create a virtual environment On EC2 Ubuntu
      python3 -m venv venv
##### 4.Activate the environment
      source venv/bin/activate
##### 5.Install Flask
      pip install Flask
##### 6.Create two files
      touch app.py Dockerfile
### How to access
      python app.py
This will start the Flask development server.
Access the app in your web browser at http://public ip:5000
### Deployment with Docker
##### 1.Build the Docker image:
     docker build -t flask-docker-app .
##### 2.Run the Docker container:
     docker run -d -p 5000:5000 flask-docker-app
This will run the Flask app within a Docker container.
##### 3.Access the app in your web browser at http://public ip:5000
### Push it to DockerHub
###### 1.Tag the image:
      docker tag <image_name>:latest <username>/<image_name>:latest
###### 2.push the image
      docker push <username>/<image_name>:latest

