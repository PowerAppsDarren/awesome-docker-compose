# README

This repository contains configuration files for various applications that can be run on a Linux server or in Docker containers. The apps are designed to be used with Docker and Docker Compose, making it easy to deploy and manage them.

## Linux Server Setup

Before setting up and using the apps which you will find the configuration files for in this repo, you need to make sure you set up your Linux server properly.

- Here are [My Linux Server Notes](https://github.com/PowerAppsDarren/Linux-Server-Notes)

# TL;DR

The tl;dr for setting up a Linux server properly (to the best of my knowledge) is:

```bash
# Update the package index:
sudo apt update

# Install required packages:
sudo apt install -y docker.io docker-compose

# Start and enable Docker:
sudo systemctl start docker

# Install required packages:  
sudo apt install -y docker.io docker-compose
  
# Start and enable Docker: 
sudo systemctl start docker
sudo systemctl enable docker

# Add your user to the Docker group:
sudo usermod -aG docker $USER

# Log out and log back in to apply the group changes.
```





