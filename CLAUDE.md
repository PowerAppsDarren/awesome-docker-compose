# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a collection of Docker Compose configurations and setup guides for various server applications. The repository is organized into numbered directories, each containing configuration for different services:

- `01-Auto-Update-Server/` - Auto-update server configuration
- `02-Security-Harden/` - Security hardening configurations  
- `03-Portainer/` - Portainer Docker management interface

## Prerequisites

This repository assumes a Linux server environment with Docker and Docker Compose installed. The main README provides the essential setup commands:

```bash
# Update package index
sudo apt update

# Install Docker and Docker Compose
sudo apt install -y docker.io docker-compose

# Start and enable Docker
sudo systemctl start docker
sudo systemctl enable docker

# Add user to Docker group
sudo usermod -aG docker $USER
```

## Architecture

Each numbered directory represents a self-contained Docker application setup:

- Each directory contains its own `readme.md` (currently minimal)
- The main `readme.md` provides Linux server setup instructions
- `terminal-commands.sh` is intended for common terminal commands (currently empty)

## Development Workflow

Since this is a Docker Compose collection repository:

1. Navigate to the specific service directory you want to work with
2. Each service should have its own Docker Compose configuration files
3. Use standard Docker Compose commands:
   - `docker-compose up -d` to start services
   - `docker-compose down` to stop services
   - `docker-compose logs` to view logs
   - `docker-compose ps` to check status

## Repository Structure

- Root level contains general setup documentation
- Numbered directories (01-, 02-, 03-) contain specific service configurations
- Each service directory is self-contained with its own documentation

## Notes

- The repository appears to be in early development stages with minimal content in service directories
- Focus on defensive security practices when working with Docker configurations
- Always review Docker Compose files for security best practices before deployment