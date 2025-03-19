TASK 1:
Installing and Configuring Nginx using Jenkins
In this assignment, I used Jenkins to automate the installation and configuration of Nginx on an Ubuntu system. I created a Freestyle Project in Jenkins and added a shell script in the build step to:

Update package lists using sudo apt update.
Install Nginx using sudo apt install -y nginx.
Enable and start the Nginx service using sudo systemctl enable nginx and sudo systemctl start nginx.
Allow HTTP traffic (port 80) through the firewall using sudo ufw allow 80/tcp and sudo ufw reload.
Verify Nginx status using sudo systemctl status nginx --no-pager.
After successfully building the project in Jenkins, I accessed Nginx’s default web page using http://127.0.0.1:80. Finally, I verified the installation using terminal commands and documented the process with screenshots.

TASK2:
# Dockerized CI/CD Pipeline with Jenkins

This project automates the process of building, tagging, and pushing a Docker image to DockerHub using Jenkins.  
The pipeline pulls source code from a GitHub repository, builds a Docker image, logs in to DockerHub, and pushes the image automatically.  

## Workflow:
1. **SCM Checkout** – Clones the latest code from the GitHub repository.  
2. **Build Docker Image** – Creates a Docker image using the project's `Dockerfile`.  
3. **Login to DockerHub** – Authenticates Jenkins with DockerHub using stored credentials.  
4. **Push Docker Image** – Uploads the built image to DockerHub for further deployment.  

This setup ensures a fully automated CI/CD workflow for containerized applications. 🚀
