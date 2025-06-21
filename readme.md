# README

This repository contains configuration files for various applications that can be run on a Linux server or in Docker containers. The apps are designed to be used with Docker and Docker Compose, making it easy to deploy and manage them.

## Linux Server Setup

Before setting up and using the apps which you will find the configuration files for in this repo, you need to make sure you set up your Linux server properly.

- Here are [My Linux Server Notes](https://github.com/PowerAppsDarren/Linux-Server-Notes)

# TL;DR

The tl;dr for setting up a Linux server properly (to the best of my knowledge) is:

```bash
# Update the package index to get latest package information
sudo apt update

# Install Docker and Docker Compose packages
# - docker.io: The Docker container runtime engine
# - docker-compose: Tool for defining and running multi-container Docker applications
# - The -y flag automatically answers "yes" to installation prompts
sudo apt install -y docker.io docker-compose

# Start the Docker service immediately
sudo systemctl start docker

# Enable Docker to start automatically on system boot
sudo systemctl enable docker

# Add your current user to the Docker group to run Docker commands without sudo
# $USER is a variable that contains your current username
sudo usermod -aG docker $USER

# Log out and log back in (or restart) to apply the group changes
# This is required for the Docker group membership to take effect
```





