# Flask Docker App
This is a simple Flask web application Dockerized for easy deployment. It provides a starting point for developing and deploying Flask applications using Docker containers.
## Getting Started
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.
## Prerequisites
 + Python 3.x
 + Docker

### Create a new application from scratch
#### Create a directory with a name "Flask-Docker-App"
      mkdir Flask-Docker-App
      
#### Navigate to the newly created directory
      cd Flask-Docker-App
#### Create a virtual environment On EC2 Ubuntu
      python3 -m venv venv
#### Activate the environment
      source venv/bin/activate
#### Install Flask
      pip install Flask
#### Create the required files
Create two files; app.py and Dockerfile
      touch app.py Dockerfile
### How to access
``` python app.py ```
This will start the Flask development server.
Access the app in your web browser at http://public ip:5000
### Deployment with Docker
#### Build the Docker image:

