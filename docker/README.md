# 🐳 Complete Docker Guide - Enterprise Ready

> **Dekh bhai**, ye guide tumhe Docker ke basics se lekar advanced concepts tak le jayega. Production-ready applications banane ke liye sab kuch cover kiya hai!

---

## 📑 Table of Contents

- [Chapter 1: Introduction](#chapter-1-introduction)
  - [1.1 What is Docker?](#11-what-is-docker)
  - [1.2 Why Docker? (Problems it Solves)](#12-why-docker-problems-it-solves)
  - [1.3 Docker Architecture](#13-docker-architecture)
  - [1.4 Docker vs Virtual Machines](#14-docker-vs-virtual-machines)

- [Chapter 2: Installation](#chapter-2-installation)
  - [2.1 Installing Docker on Windows](#21-installing-docker-on-windows)
  - [2.2 Installing Docker on macOS](#22-installing-docker-on-macos)
  - [2.3 Installing Docker on Linux](#23-installing-docker-on-linux)
  - [2.4 Post-Installation Setup](#24-post-installation-setup)
  - [2.5 Verifying Installation](#25-verifying-installation)

- [Chapter 3: Docker Containers and Images](#chapter-3-docker-containers-and-images)
  - [3.1 Understanding Docker Images](#31-understanding-docker-images)
  - [3.2 Understanding Docker Containers](#32-understanding-docker-containers)
  - [3.3 Image Layers and Caching](#33-image-layers-and-caching)
  - [3.4 Container Lifecycle](#34-container-lifecycle)

- [Chapter 4: Docker Hub](#chapter-4-docker-hub)
  - [4.1 What is Docker Hub?](#41-what-is-docker-hub)
  - [4.2 Creating Docker Hub Account](#42-creating-docker-hub-account)
  - [4.3 Pulling Images from Docker Hub](#43-pulling-images-from-docker-hub)
  - [4.4 Pushing Images to Docker Hub](#44-pushing-images-to-docker-hub)
  - [4.5 Docker Registry vs Docker Hub](#45-docker-registry-vs-docker-hub)

- [Chapter 5: Docker Command Line Interface (CLI)](#chapter-5-docker-command-line-interface-cli)
  - [5.1 Docker CLI Basics](#51-docker-cli-basics)
  - [5.2 Getting Help with Commands](#52-getting-help-with-commands)
  - [5.3 Docker System Commands](#53-docker-system-commands)

- [Chapter 6: Docker Image CLI](#chapter-6-docker-image-cli)
  - [6.1 Listing Images](#61-listing-images)
  - [6.2 Pulling Images](#62-pulling-images)
  - [6.3 Removing Images](#63-removing-images)
  - [6.4 Inspecting Images](#64-inspecting-images)
  - [6.5 Tagging Images](#65-tagging-images)
  - [6.6 Saving and Loading Images](#66-saving-and-loading-images)
  - [6.7 Image History](#67-image-history)
  - [6.8 Pruning Unused Images](#68-pruning-unused-images)

- [Chapter 7: Docker Container CLI](#chapter-7-docker-container-cli)
  - [7.1 Running Containers](#71-running-containers)
  - [7.2 Listing Containers](#72-listing-containers)
  - [7.3 Starting and Stopping Containers](#73-starting-and-stopping-containers)
  - [7.4 Removing Containers](#74-removing-containers)
  - [7.5 Executing Commands in Running Containers](#75-executing-commands-in-running-containers)
  - [7.6 Viewing Container Logs](#76-viewing-container-logs)
  - [7.7 Inspecting Containers](#77-inspecting-containers)
  - [7.8 Copying Files Between Host and Container](#78-copying-files-between-host-and-container)
  - [7.9 Container Resource Management](#79-container-resource-management)
  - [7.10 Container Statistics](#710-container-statistics)

- [Chapter 8: Dockerfile](#chapter-8-dockerfile)
  - [8.1 What is a Dockerfile?](#81-what-is-a-dockerfile)
  - [8.2 Dockerfile Instructions](#82-dockerfile-instructions)
  - [8.3 Building Images from Dockerfile](#83-building-images-from-dockerfile)
  - [8.4 Best Practices for Dockerfile](#84-best-practices-for-dockerfile)
  - [8.5 Multi-stage Builds](#85-multi-stage-builds)
  - [8.6 .dockerignore File](#86-dockerignore-file)

- [Chapter 9: Containerizing Applications](#chapter-9-containerizing-applications)
  - [9.1 Containerizing a Node.js Application](#91-containerizing-a-nodejs-application)
  - [9.2 Containerizing a Python Application](#92-containerizing-a-python-application)
  - [9.3 Containerizing a Java Application](#93-containerizing-a-java-application)
  - [9.4 Environment Variables in Containers](#94-environment-variables-in-containers)

- [Chapter 10: Port Mapping](#chapter-10-port-mapping)
  - [10.1 Understanding Port Mapping](#101-understanding-port-mapping)
  - [10.2 Manual Port Mapping](#102-manual-port-mapping)
  - [10.3 Automatic Port Mapping](#103-automatic-port-mapping)
  - [10.4 Exposing Multiple Ports](#104-exposing-multiple-ports)

- [Chapter 11: Pushing Custom Images](#chapter-11-pushing-custom-images)
  - [11.1 Tagging Custom Images](#111-tagging-custom-images)
  - [11.2 Logging into Docker Hub](#112-logging-into-docker-hub)
  - [11.3 Pushing Images](#113-pushing-images)
  - [11.4 Versioning Images](#114-versioning-images)

- [Chapter 12: Docker Networking](#chapter-12-docker-networking)
  - [12.1 Docker Networking Basics](#121-docker-networking-basics)
  - [12.2 Network Drivers Overview](#122-network-drivers-overview)
  - [12.3 Bridge Mode Networking (Default)](#123-bridge-mode-networking-default)
  - [12.4 Host Mode Networking](#124-host-mode-networking)
  - [12.5 Overlay Mode Networking](#125-overlay-mode-networking)
  - [12.6 ipvlan and MacVlan Mode Networking](#126-ipvlan-and-macvlan-mode-networking)
  - [12.7 None Mode Networking](#127-none-mode-networking)
  - [12.8 Custom Bridge Networks](#128-custom-bridge-networks)
  - [12.9 Container Communication](#129-container-communication)

- [Chapter 13: Docker Volumes](#chapter-13-docker-volumes)
  - [13.1 Understanding Docker Volumes](#131-understanding-docker-volumes)
  - [13.2 Types of Volumes](#132-types-of-volumes)
  - [13.3 Attaching Host Volumes (Bind Mounts)](#133-attaching-host-volumes-bind-mounts)
  - [13.4 Creating and Managing Custom Volumes](#134-creating-and-managing-custom-volumes)
  - [13.5 Volume Commands](#135-volume-commands)
  - [13.6 Backup and Restore Volumes](#136-backup-and-restore-volumes)

- [Chapter 14: Docker Compose](#chapter-14-docker-compose)
  - [14.1 What is Docker Compose?](#141-what-is-docker-compose)
  - [14.2 Installing Docker Compose](#142-installing-docker-compose)
  - [14.3 Docker Compose File Structure](#143-docker-compose-file-structure)
  - [14.4 Docker Compose Commands](#144-docker-compose-commands)
  - [14.5 Multi-Container Application Example](#145-multi-container-application-example)
  - [14.6 Environment Variables in Compose](#146-environment-variables-in-compose)
  - [14.7 Depends On and Service Dependencies](#147-depends-on-and-service-dependencies)
  - [14.8 Docker Compose Networking](#148-docker-compose-networking)
  - [14.9 Docker Compose Volumes](#149-docker-compose-volumes)

- [Chapter 15: Advanced Topics](#chapter-15-advanced-topics)
  - [15.1 Docker Security Best Practices](#151-docker-security-best-practices)
  - [15.2 Docker Logging](#152-docker-logging)
  - [15.3 Health Checks](#153-health-checks)
  - [15.4 Docker Secrets](#154-docker-secrets)
  - [15.5 Production Deployment Strategies](#155-production-deployment-strategies)

---

## Chapter 1: Introduction

### 1.1 What is Docker?

**Dekh bhai**, Docker ek platform hai jo applications ko containers me package karta hai. Container ek lightweight, portable unit hai jisme tumhari application aur uski saari dependencies hoti hain.

**Key Points:**

- Docker is a containerization platform
- Containers are isolated environments
- Write once, run anywhere philosophy
- Developed by Docker Inc. in 2013

**Real-world Example:**
Imagine you're developing a web application on your laptop. It works perfectly with Node.js v18, MongoDB 5.0, and Ubuntu. When you deploy it to production server (which might have different versions), it breaks. Docker solves this by packaging everything together.

```bash
# Without Docker: "It works on my machine" problem
Developer Machine: Node 18 + MongoDB 5.0 + Ubuntu 20.04 ✓
Production Server: Node 16 + MongoDB 4.4 + CentOS 8 ✗

# With Docker: Same container everywhere
Developer Machine: Docker Container ✓
Production Server: Same Docker Container ✓
```

---

### 1.2 Why Docker? (Problems it Solves)

**Bhai ye problems solve karta hai Docker:**

1. **Dependency Hell**
   - **Problem:** App needs specific versions of libraries, but your system has different versions
   - **Solution:** Container me sab kuch isolated hai

2. **Environment Inconsistency**
   - **Problem:** "Works on my machine" syndrome
   - **Solution:** Same container, same environment everywhere

3. **Resource Efficiency**
   - **Problem:** VMs are heavy (GBs of storage, slow startup)
   - **Solution:** Containers are lightweight (MBs of storage, instant startup)

4. **Scalability**
   - **Problem:** Scaling applications is complex
   - **Solution:** Spin up multiple containers instantly

5. **Development Speed**
   - **Problem:** Setting up dev environment takes hours/days
   - **Solution:** Pull a container, start coding in minutes

**Real-world Scenario:**

```
Your company is building a microservices application:
- Frontend: React
- Backend: Node.js + Express
- Database: PostgreSQL
- Cache: Redis
- Message Queue: RabbitMQ

Without Docker: Each developer spends 2-3 days setting up
With Docker: docker-compose up → Ready in 5 minutes!
```

---

### 1.3 Docker Architecture

**Components of Docker:**

1. **Docker Engine**
   - Core service that creates and manages containers
   - Runs as a daemon process on host OS

2. **Docker Client**
   - CLI tool to interact with Docker daemon
   - Commands like `docker run`, `docker build`

3. **Docker Registry**
   - Storage for Docker images
   - Docker Hub is the public registry

4. **Docker Objects**
   - Images: Blueprint of containers
   - Containers: Running instances of images
   - Networks: Communication between containers
   - Volumes: Persistent data storage

**Architecture Diagram (Text Representation):**

```
┌─────────────────┐
│  Docker Client  │ (CLI Commands)
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│  Docker Daemon  │ (Docker Engine)
└────────┬────────┘
         │
    ┌────┴────┬─────────┬─────────┐
    ▼         ▼         ▼         ▼
┌────────┐ ┌────────┐ ┌────────┐ ┌────────┐
│Container│ │Container│ │Container│ │Container│
└────────┘ └────────┘ └────────┘ └────────┘
```

---

### 1.4 Docker vs Virtual Machines

**Key Differences:**

| Feature | Docker Containers | Virtual Machines |
|---------|------------------|------------------|
| **Size** | Lightweight (MBs) | Heavy (GBs) |
| **Startup Time** | Seconds | Minutes |
| **Performance** | Native performance | Slower |
| **Isolation** | Process-level | OS-level |
| **OS** | Shares host OS kernel | Separate OS for each VM |
| **Resource Usage** | Minimal | High |

**Visual Comparison:**

```
VIRTUAL MACHINES:
┌──────────────────────────────────┐
│         Host Operating System    │
├──────────────────────────────────┤
│          Hypervisor (VMware)     │
├──────┬──────┬──────┬─────────────┤
│ VM 1 │ VM 2 │ VM 3 │             │
│Guest │Guest │Guest │             │
│ OS   │ OS   │ OS   │             │
│App   │App   │App   │             │
└──────┴──────┴──────┴─────────────┘

DOCKER CONTAINERS:
┌──────────────────────────────────┐
│         Host Operating System    │
├──────────────────────────────────┤
│           Docker Engine          │
├──────┬──────┬──────┬─────────────┤
│ App1 │ App2 │ App3 │ App4        │
│Libs  │Libs  │Libs  │Libs         │
└──────┴──────┴──────┴─────────────┘
```

**Real-world Example:**

```
Scenario: Running 5 microservices

VM Approach:
- 5 VMs × 2GB RAM each = 10GB RAM
- 5 VMs × 20GB disk each = 100GB disk
- Startup time: 5 minutes per VM
- Total: 10GB RAM, 100GB disk, 25 minutes

Docker Approach:
- 5 containers × 100MB RAM each = 500MB RAM
- 5 containers × 500MB disk each = 2.5GB disk
- Startup time: 2 seconds per container
- Total: 500MB RAM, 2.5GB disk, 10 seconds
```

---

## Chapter 2: Installation

### 2.1 Installing Docker on Windows

**Requirements:**

- Windows 10/11 (64-bit): Pro, Enterprise, or Education
- WSL 2 (Windows Subsystem for Linux)
- Virtualization enabled in BIOS

**Steps:**

1. **Enable WSL 2:**

```powershell
# Open PowerShell as Administrator
wsl --install
wsl --set-default-version 2
```

2. **Download Docker Desktop:**
   - Visit: <https://www.docker.com/products/docker-desktop>
   - Download Docker Desktop for Windows
   - Run the installer

3. **Installation:**
   - Follow the installation wizard
   - Check "Use WSL 2 instead of Hyper-V"
   - Restart your computer

4. **Verify:**

```bash
docker --version
docker run hello-world
```

**Common Issues:**

- **Virtualization not enabled:** Go to BIOS and enable Intel VT-x or AMD-V
- **WSL 2 not installed:** Run `wsl --install` in PowerShell as admin

---

### 2.2 Installing Docker on macOS

**Requirements:**

- macOS 10.15 or newer
- Apple Silicon (M1/M2) or Intel chip

**Steps:**

1. **Download Docker Desktop:**
   - Visit: <https://www.docker.com/products/docker-desktop>
   - Choose Mac with Intel chip or Mac with Apple chip

2. **Installation:**
   - Open the .dmg file
   - Drag Docker icon to Applications folder
   - Open Docker from Applications
   - Grant necessary permissions

3. **Verify:**

```bash
docker --version
docker run hello-world
```

---

### 2.3 Installing Docker on Linux

**For Ubuntu/Debian:**

```bash
# Update package index
sudo apt-get update

# Install dependencies
sudo apt-get install \
    ca-certificates \
    curl \
    gnupg \
    lsb-release

# Add Docker's official GPG key
sudo mkdir -p /etc/apt/keyrings
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg

# Set up repository
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu \
  $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

# Install Docker Engine
sudo apt-get update
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin

# Verify installation
sudo docker run hello-world
```

**For CentOS/RHEL:**

```bash
# Install dependencies
sudo yum install -y yum-utils

# Add Docker repository
sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo

# Install Docker
sudo yum install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin

# Start Docker
sudo systemctl start docker
sudo systemctl enable docker

# Verify
sudo docker run hello-world
```

---

### 2.4 Post-Installation Setup

**Dekh bhai, ye important hai - sudo ke bina Docker chalane ke liye:**

**Linux Post-Installation:**

```bash
# Create docker group (usually exists)
sudo groupadd docker

# Add your user to docker group
sudo usermod -aG docker $USER

# Log out and log back in, or run:
newgrp docker

# Verify you can run without sudo
docker run hello-world
```

**Configure Docker to Start on Boot:**

```bash
# Linux
sudo systemctl enable docker.service
sudo systemctl enable containerd.service
```

---

### 2.5 Verifying Installation

**Comprehensive Verification:**

```bash
# 1. Check Docker version
docker --version
# Output: Docker version 24.0.5, build ced0996

# 2. Check Docker Compose version
docker compose version
# Output: Docker Compose version v2.20.2

# 3. Check Docker info
docker info

# 4. Run test container
docker run hello-world

# 5. Check running containers
docker ps

# 6. Check all containers
docker ps -a
```

**Real-world Check:**

```bash
# Run a real web server
docker run -d -p 8080:80 nginx

# Check if it's running
docker ps

# Open browser: http://localhost:8080
# You should see Nginx welcome page

# Stop and remove
docker stop <container-id>
docker rm <container-id>
```

---

## Chapter 3: Docker Containers and Images

### 3.1 Understanding Docker Images

**Kya hai ye Image?**
Docker image ek read-only template hai jo instructions contain karta hai ek container create karne ke liye. Ye blueprint hai tumhare application ka.

**Image Characteristics:**

- Immutable (cannot be changed)
- Made up of layers
- Can be versioned with tags
- Stored in registries (Docker Hub, private registries)

**Image Naming Convention:**

```
registry/repository:tag

Examples:
- nginx:latest
- ubuntu:22.04
- myusername/myapp:v1.0
- gcr.io/google-containers/nginx:1.14.2
```

**Real-world Analogy:**

```
Image = Recipe for a cake
Container = Actual cake made from that recipe

You can make multiple cakes (containers) from one recipe (image)
Each cake is independent, but all follow the same recipe
```

---

### 3.2 Understanding Docker Containers

**Container kya hai?**
Container ek running instance hai image ka. Ye isolated environment hai jisme tumhari application execute hoti hai.

**Container Properties:**

- Ephemeral (temporary by nature)
- Isolated from host and other containers
- Can be started, stopped, moved, and deleted
- Lightweight and fast

**Container States:**

```
Created → Running → Paused → Stopped → Deleted

┌─────────┐    start    ┌─────────┐
│ Created │ ──────────> │ Running │
└─────────┘             └────┬────┘
                             │
                          pause
                             │
                             ▼
                        ┌────────┐
                        │ Paused │
                        └────┬───┘
                             │
                          unpause
                             │
                             ▼
                        ┌────────┐
                        │ Stopped│
                        └────┬───┘
                             │
                            rm
                             │
                             ▼
                        ┌────────┐
                        │Deleted │
                        └────────┘
```

**Real-world Example:**

```bash
# Create container from nginx image
docker run -d --name my-web-server nginx

# This creates and starts a container:
# - Image: nginx
# - Container name: my-web-server
# - Mode: detached (-d means runs in background)
# - State: Running

# Check it's running
docker ps

# Stop it
docker stop my-web-server
# State: Stopped

# Start again
docker start my-web-server
# State: Running

# Remove it
docker rm -f my-web-server
# State: Deleted
```

---

### 3.3 Image Layers and Caching

**Layers ka concept - Bahut important hai!**

Docker images are built in layers. Har instruction Dockerfile me ek layer create karta hai.

**How Layers Work:**

```
Dockerfile:
FROM ubuntu:20.04       ← Layer 1 (Base OS)
RUN apt-get update      ← Layer 2 (Update packages)
RUN apt-get install -y python3  ← Layer 3 (Install Python)
COPY app.py /app/       ← Layer 4 (Copy app)
CMD ["python3", "/app/app.py"]  ← Layer 5 (Set command)
```

**Layer Benefits:**

1. **Caching:**
   - If a layer hasn't changed, Docker reuses it
   - Speeds up builds dramatically

2. **Storage Efficiency:**
   - Multiple images can share layers
   - Saves disk space

3. **Fast Distribution:**
   - Only changed layers are downloaded/uploaded

**Real-world Example:**

```bash
# First build - All layers created
docker build -t myapp:v1 .
# Time: 5 minutes

# You modify only app.py
# Second build - Layers 1-3 cached, only layer 4-5 rebuilt
docker build -t myapp:v2 .
# Time: 10 seconds

# View image layers
docker history myapp:v2
```

**Best Practice:**

```dockerfile
# ❌ Bad - Creates many layers
RUN apt-get update
RUN apt-get install -y python3
RUN apt-get install -y python3-pip
RUN apt-get clean

# ✅ Good - Single layer, efficient
RUN apt-get update && \
    apt-get install -y python3 python3-pip && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*
```

---

### 3.4 Container Lifecycle

**Complete Lifecycle Management:**

**1. Create:**

```bash
# Create without starting
docker create --name mycontainer nginx
```

**2. Start:**

```bash
# Start an existing container
docker start mycontainer

# Create and start in one command
docker run --name mycontainer nginx
```

**3. Running Operations:**

```bash
# Execute command in running container
docker exec -it mycontainer bash

# View logs
docker logs mycontainer

# View resource usage
docker stats mycontainer
```

**4. Pause/Unpause:**

```bash
# Pause all processes in container
docker pause mycontainer

# Resume
docker unpause mycontainer
```

**5. Stop:**

```bash
# Graceful shutdown (SIGTERM, then SIGKILL after 10s)
docker stop mycontainer

# Force shutdown (SIGKILL immediately)
docker kill mycontainer
```

**6. Remove:**

```bash
# Remove stopped container
docker rm mycontainer

# Force remove running container
docker rm -f mycontainer
```

**Real-world Scenario:**

```bash
# Development workflow
# 1. Start database
docker run -d --name dev-db postgres:14

# 2. Start your app (linked to database)
docker run -d --name dev-app --link dev-db:postgres myapp:latest

# 3. Make code changes, restart app
docker restart dev-app

# 4. Debug issues
docker logs dev-app
docker exec -it dev-app bash

# 5. End of day - stop everything
docker stop dev-app dev-db

# 6. Next day - start everything
docker start dev-db dev-app

# 7. Clean up when done
docker rm -f dev-app dev-db
```

---

## Chapter 4: Docker Hub

### 4.1 What is Docker Hub?

**Dekh bhai**, Docker Hub is like GitHub for Docker images. It's a cloud-based registry service where you can find, share, and manage Docker images.

**Key Features:**

- 100,000+ official and community images
- Public and private repositories
- Automated builds
- Webhooks and team collaboration
- Free for public repositories

**Registry Hierarchy:**

```
Docker Hub
├── Official Images (e.g., nginx, ubuntu, postgres)
├── Verified Publishers (e.g., microsoft, oracle)
└── Community Images (e.g., username/imagename)
```

---

### 4.2 Creating Docker Hub Account

**Steps:**

1. Visit <https://hub.docker.com>
2. Click "Sign Up"
3. Fill in details:
   - Username
   - Email
   - Password
4. Verify email
5. Create your first repository (optional)

**Account Types:**

- **Free:** Unlimited public repos, 1 private repo
- **Pro:** Unlimited private repos, parallel builds
- **Team:** For organizations, advanced features

---

### 4.3 Pulling Images from Docker Hub

**Basic Pull:**

```bash
# Pull latest version
docker pull nginx

# Pull specific version
docker pull nginx:1.24

# Pull from specific registry
docker pull ubuntu:22.04

# Pull all tags of an image
docker pull --all-tags nginx
```

**Search Images:**

```bash
# Search on Docker Hub
docker search nginx

# Search with filters
docker search --filter stars=100 nginx
docker search --filter is-official=true nginx
```

**Real-world Example:**

```bash
# Scenario: Setting up a development environment

# 1. Pull database
docker pull postgres:14-alpine
# alpine = smaller size, faster download

# 2. Pull caching layer
docker pull redis:7-alpine

# 3. Pull web server
docker pull nginx:alpine

# 4. Check all downloaded images
docker images
```

**Understanding Image Tags:**

```bash
# Common tagging patterns:
nginx:latest          # Latest stable version
nginx:1.24           # Specific version
nginx:1.24.0         # Specific patch version
nginx:alpine         # Alpine Linux base (smaller)
nginx:1.24-alpine    # Version + Alpine
postgres:14          # Major version
postgres:14.9        # Specific patch
node:18-slim         # Slim variant (smaller)
```

---

### 4.4 Pushing Images to Docker Hub

**Complete Workflow:**

**Step 1: Login**

```bash
# Login to Docker Hub
docker login

# Enter username and password
# Login Succeeded
```

**Step 2: Tag Your Image**

```bash
# Build your image
docker build -t myapp:latest .

# Tag it with your username
docker tag myapp:latest username/myapp:latest
docker tag myapp:latest username/myapp:v1.0
```

**Step 3: Push**

```bash
# Push to Docker Hub
docker push username/myapp:latest
docker push username/myapp:v1.0
```

**Step 4: Verify**

- Go to hub.docker.com
- Check your repositories
- Verify the image is there

**Real-world Example:**

```bash
# You've built a Node.js application

# 1. Build image
docker build -t my-node-app .

# 2. Test locally
docker run -p 3000:3000 my-node-app

# 3. Tag for Docker Hub
docker tag my-node-app johndoe/my-node-app:1.0
docker tag my-node-app johndoe/my-node-app:latest

# 4. Login
docker login

# 5. Push
docker push johndoe/my-node-app:1.0
docker push johndoe/my-node-app:latest

# 6. Now anyone can use it
# Someone else can now run:
# docker pull johndoe/my-node-app:latest
# docker run johndoe/my-node-app:latest
```

---

### 4.5 Docker Registry vs Docker Hub

**Docker Registry:**

- Generic term for any image storage
- Can be public or private
- Self-hosted or cloud-based

**Docker Hub:**

- Specific registry service by Docker Inc.
- Public registry with community images
- Free and paid tiers

**Other Registries:**

1. **Amazon ECR (Elastic Container Registry)**

```bash
# Login to ECR
aws ecr get-login-password --region us-east-1 | docker login --username AWS --password-stdin 123456789.dkr.ecr.us-east-1.amazonaws.com

# Push to ECR
docker tag myapp:latest 123456789.dkr.ecr.us-east-1.amazonaws.com/myapp:latest
docker push 123456789.dkr.ecr.us-east-1.amazonaws.com/myapp:latest
```

2. **Google Container Registry (GCR)**

```bash
# Configure Docker for GCR
gcloud auth configure-docker

# Push to GCR
docker tag myapp:latest gcr.io/my-project/myapp:latest
docker push gcr.io/my-project/myapp:latest
```

3. **Azure Container Registry (ACR)**

```bash
# Login to ACR
az acr login --name myregistry

# Push to ACR
docker tag myapp:latest myregistry.azurecr.io/myapp:latest
docker push myregistry.azurecr.io/myapp:latest
```

4. **Private Registry (Self-hosted)**

```bash
# Run your own registry
docker run -d -p 5000:5000 --name registry registry:2

# Push to private registry
docker tag myapp:latest localhost:5000/myapp:latest
docker push localhost:5000/myapp:latest
```

**When to Use What:**

| Registry | Use Case |
|----------|----------|
| **Docker Hub** | Open source projects, learning, public images |
| **AWS ECR** | AWS infrastructure, private images, CI/CD with AWS |
| **GCR** | Google Cloud projects, Kubernetes on GKE |
| **ACR** | Azure infrastructure, AKS deployments |
| **Private Registry** | High security, compliance, on-premise |

---

## Chapter 5: Docker Command Line Interface (CLI)

### 5.1 Docker CLI Basics

**Samajh le bhai**, Docker CLI tumhara main tool hai Docker ke saath interact karne ka. Sab kuch yahi se hota hai!

**Basic Command Structure:**

```bash
docker [OPTIONS] COMMAND [ARG...]

Examples:
docker run nginx                    # Run a container
docker ps                          # List containers
docker images                      # List images
docker build -t myapp .           # Build an image
```

**Command Categories:**

```
Container Management:
├── docker run        # Create and start container
├── docker ps         # List containers
├── docker stop       # Stop container
├── docker start      # Start container
├── docker rm         # Remove container
└── docker exec       # Execute command in container

Image Management:
├── docker images     # List images
├── docker pull       # Pull image
├── docker push       # Push image
├── docker build      # Build image
├── docker rmi        # Remove image
└── docker tag        # Tag image

System Management:
├── docker info       # System information
├── docker version    # Docker version
├── docker system df  # Disk usage
└── docker system prune  # Clean up

Network Management:
├── docker network ls     # List networks
├── docker network create # Create network
└── docker network rm     # Remove network

Volume Management:
├── docker volume ls      # List volumes
├── docker volume create  # Create volume
└── docker volume rm      # Remove volume
```

**CLI Tips:**

```bash
# Use autocomplete (add to ~/.bashrc or ~/.zshrc)
# For bash:
# eval "$(docker completion bash)"

# For zsh:
# eval "$(docker completion zsh)"

# Short commands (aliases)
docker ps = docker container ls
docker images = docker image ls
docker rmi = docker image rm
```

---

### 5.2 Getting Help with Commands

**Har command ke saath help available hai:**

```bash
# General help
docker --help

# Command-specific help
docker run --help
docker build --help
docker network --help

# Subcommand help
docker container --help
docker image --help
docker volume --help
```

**Reading Help Output:**

```bash
$ docker run --help

Usage:  docker run [OPTIONS] IMAGE [COMMAND] [ARG...]

Options:
  -d, --detach          Run container in background
  -p, --publish list    Publish container's port(s)
  -e, --env list        Set environment variables
  -v, --volume list     Bind mount a volume
  --name string         Assign a name to the container
  --rm                  Remove container when it exits
  -it                   Interactive terminal

# Square brackets [] = Optional
# ... = Can be repeated
```

**Quick Reference:**

```bash
# Common patterns
docker COMMAND --help           # Help for any command
docker COMMAND SUBCOMMAND --help  # Help for subcommand

# Examples
docker run --help              # All run options
docker network create --help   # Network creation options
docker volume ls --help        # List volumes options
```

---

### 5.3 Docker System Commands

**System-wide Operations:**

**1. System Information:**

```bash
# Detailed Docker info
docker info

# Output includes:
# - Number of containers (running, paused, stopped)
# - Number of images
# - Storage driver
# - Docker version
# - OS/Arch
# - CPUs, Memory

# Check Docker version
docker version

# Get Docker version (short)
docker --version
```

**2. Disk Usage:**

```bash
# Check disk usage
docker system df

# Output:
TYPE            TOTAL     ACTIVE    SIZE      RECLAIMABLE
Images          10        5         2.5GB     1.2GB (48%)
Containers      15        3         500MB     300MB (60%)
Local Volumes   5         2         1GB       500MB (50%)
Build Cache     20        0         800MB     800MB (100%)

# Detailed disk usage
docker system df -v
```

**3. System Cleanup:**

```bash
# Remove all unused data (containers, images, networks, volumes)
docker system prune

# Remove everything (including volumes)
docker system prune -a --volumes

# Prune with force (no confirmation)
docker system prune -f

# Prune only older than certain time
docker system prune --filter "until=24h"
```

**4. Real-time Events:**

```bash
# Monitor Docker events
docker events

# Filter events
docker events --filter 'type=container'
docker events --filter 'event=start'
docker events --filter 'container=myapp'

# Events since certain time
docker events --since '2023-01-01'
```

**Real-world Maintenance Script:**

```bash
#!/bin/bash
# docker-cleanup.sh

echo "🧹 Starting Docker cleanup..."

echo "📊 Before cleanup:"
docker system df

echo "🗑️  Removing stopped containers..."
docker container prune -f

echo "🗑️  Removing unused images..."
docker image prune -a -f

echo "🗑️  Removing unused volumes..."
docker volume prune -f

echo "🗑️  Removing unused networks..."
docker network prune -f

echo "📊 After cleanup:"
docker system df

echo "✅ Cleanup complete!"
```

**System Monitoring:**

```bash
# Real-time stats for all containers
docker stats

# Stats for specific container
docker stats mycontainer

# Stats in non-streaming mode
docker stats --no-stream

# Custom format
docker stats --format "table {{.Container}}\t{{.CPUPerc}}\t{{.MemUsage}}"
```

---

## Chapter 6: Docker Image CLI

### 6.1 Listing Images

**List karo apne sare images:**

```bash
# List all images
docker images

# Alternative command
docker image ls

# Output format:
REPOSITORY    TAG       IMAGE ID       CREATED         SIZE
nginx         latest    605c77e624dd   2 weeks ago     141MB
postgres      14        e5db4b7c6e6c   3 weeks ago     376MB
myapp         v1.0      1234567890ab   1 hour ago      500MB
```

**Advanced Listing:**

```bash
# Show all images including intermediates
docker images -a

# Show only image IDs
docker images -q

# Filter images
docker images --filter "dangling=true"    # Untagged images
docker images --filter "before=nginx"     # Images created before nginx
docker images --filter "since=nginx"      # Images created after nginx
docker images --filter "reference=*app*"  # Images with 'app' in name

# Custom format
docker images --format "{{.Repository}}:{{.Tag}}"
docker images --format "table {{.Repository}}\t{{.Tag}}\t{{.Size}}"

# Sort by size
docker images --format "{{.Size}}\t{{.Repository}}:{{.Tag}}" | sort -h
```

**Real-world Example:**

```bash
# Find large images consuming space
docker images --format "{{.Size}}\t{{.Repository}}:{{.Tag}}" | sort -hr | head -10

# Find dangling images (no tag)
docker images --filter "dangling=true"

# List images by specific repository
docker images nginx
docker images postgres
```

---

### 6.2 Pulling Images

**Download karo images Docker Hub se:**

```bash
# Pull latest tag
docker pull ubuntu

# Pull specific tag
docker pull ubuntu:22.04
docker pull postgres:14-alpine

# Pull from specific registry
docker pull gcr.io/google-samples/hello-app:1.0

# Pull with digest (exact version)
docker pull nginx@sha256:1234567890abcdef...

# Pull all tags
docker pull -a nginx

# Pull with platform specification
docker pull --platform linux/amd64 nginx
docker pull --platform linux/arm64 postgres
```

**Pull with Progress:**

```bash
# Pull shows download progress
docker pull postgres:14

# Output:
14: Pulling from library/postgres
a2abf6c4d29d: Pull complete
e1769f49f910: Pull complete
33a59cfee47c: Pull complete
461b2090c345: Downloading [========>                ] 45.5MB/156.3MB
8ed8ab6290ac: Download complete
```

**Verify Pulled Image:**

```bash
# After pulling
docker pull redis:alpine

# Verify it's there
docker images redis

# Inspect the image
docker inspect redis:alpine

# Check image history
docker history redis:alpine
```

---

### 6.3 Removing Images

**Delete karo unwanted images:**

```bash
# Remove by name:tag
docker rmi nginx:latest

# Remove by image ID
docker rmi 605c77e624dd

# Force remove (even if containers exist)
docker rmi -f nginx:latest

# Remove multiple images
docker rmi nginx postgres redis

# Remove all images
docker rmi $(docker images -q)

# Remove dangling images
docker image prune

# Remove all unused images
docker image prune -a

# Remove images older than 24 hours
docker image prune -a --filter "until=24h"
```

**Common Errors and Solutions:**

```bash
# Error: image is being used by container
$ docker rmi nginx
Error: conflict: unable to remove repository reference "nginx" (must force)

# Solution 1: Stop and remove containers first
docker rm -f $(docker ps -aq --filter ancestor=nginx)
docker rmi nginx

# Solution 2: Force remove
docker rmi -f nginx

# Error: image has dependent child images
$ docker rmi ubuntu:20.04
Error: conflict: unable to delete (cannot be forced)

# Solution: Remove child images first
docker images --filter "since=ubuntu:20.04"
docker rmi <child-images>
docker rmi ubuntu:20.04
```

---

### 6.4 Inspecting Images

**Deep dive into image details:**

```bash
# Complete inspection
docker inspect nginx:latest

# Output is JSON format with:
# - Image ID
# - Created date
# - Architecture
# - OS
# - Layers
# - Environment variables
# - Exposed ports
# - Entry point
# - Command

# Extract specific information
docker inspect --format='{{.Architecture}}' nginx
docker inspect --format='{{.Os}}' nginx
docker inspect --format='{{.Size}}' nginx

# Get environment variables
docker inspect --format='{{.Config.Env}}' nginx

# Get exposed ports
docker inspect --format='{{.Config.ExposedPorts}}' nginx

# Get creation date
docker inspect --format='{{.Created}}' nginx
```

**Practical Inspection Examples:**

```bash
# Check which ports an image exposes
docker inspect --format='{{json .Config.ExposedPorts}}' nginx | jq

# Check default command
docker inspect --format='{{.Config.Cmd}}' nginx

# Check entry point
docker inspect --format='{{.Config.Entrypoint}}' nginx

# Get all layers
docker inspect --format='{{json .RootFS.Layers}}' nginx | jq

# Check image labels
docker inspect --format='{{json .Config.Labels}}' nginx | jq
```

---

### 6.5 Tagging Images

**Image ko naam aur version do:**

```bash
# Tag format: REGISTRY/REPOSITORY:TAG

# Basic tagging
docker tag nginx:latest mynginx:v1.0

# Tag for Docker Hub
docker tag myapp:latest username/myapp:latest
docker tag myapp:latest username/myapp:v1.0
docker tag myapp:latest username/myapp:stable

# Tag for private registry
docker tag myapp:latest myregistry.com:5000/myapp:latest

# Tag for cloud registries
docker tag myapp:latest gcr.io/my-project/myapp:latest
docker tag myapp:latest 123456.dkr.ecr.us-east-1.amazonaws.com/myapp:latest
```

**Semantic Versioning:**

```bash
# Version tagging strategy
docker tag myapp:latest myapp:1.0.0    # Specific version
docker tag myapp:latest myapp:1.0      # Minor version
docker tag myapp:latest myapp:1        # Major version
docker tag myapp:latest myapp:latest   # Latest stable

# Environment tags
docker tag myapp:latest myapp:dev
docker tag myapp:latest myapp:staging
docker tag myapp:latest myapp:production
```

**Real-world Tagging Workflow:**

```bash
# Build new version
docker build -t myapp .

# Tag with multiple versions
docker tag myapp:latest myapp:2.1.0
docker tag myapp:latest myapp:2.1
docker tag myapp:latest myapp:2
docker tag myapp:latest myapp:latest

# Tag for Docker Hub
docker tag myapp:latest username/myapp:2.1.0
docker tag myapp:latest username/myapp:latest

# Push all tags
docker push username/myapp:2.1.0
docker push username/myapp:latest
```

---

### 6.6 Saving and Loading Images

**Images ko file me save karo aur load karo:**

**Save Image:**

```bash
# Save single image
docker save nginx:latest > nginx.tar
docker save -o nginx.tar nginx:latest

# Save multiple images
docker save -o images.tar nginx:latest postgres:14 redis:alpine

# Save with compression
docker save nginx:latest | gzip > nginx.tar.gz
```

**Load Image:**

```bash
# Load from tar file
docker load < nginx.tar
docker load -i nginx.tar

# Load compressed image
gunzip -c nginx.tar.gz | docker load
```

**Real-world Use Cases:**

**1. Transfer images without internet:**

```bash
# On machine with internet
docker pull postgres:14
docker save -o postgres14.tar postgres:14

# Transfer postgres14.tar via USB/network

# On offline machine
docker load -i postgres14.tar
docker images  # Verify it's loaded
```

**2. Backup important images:**

```bash
# Backup script
#!/bin/bash
BACKUP_DIR="/backup/docker-images"
DATE=$(date +%Y%m%d)

mkdir -p $BACKUP_DIR

# Save production images
docker save myapp:production | gzip > $BACKUP_DIR/myapp-prod-$DATE.tar.gz
docker save database:latest | gzip > $BACKUP_DIR/database-$DATE.tar.gz

echo "Backup completed: $BACKUP_DIR"
```

**3. Share custom images:**

```bash
# Developer 1 creates custom image
docker build -t custom-dev-env .
docker save -o custom-dev-env.tar custom-dev-env:latest

# Share tar file with team

# Developer 2 loads it
docker load -i custom-dev-env.tar
docker run -it custom-dev-env:latest
```

---

### 6.7 Image History

**Image ki puri history dekho:**

```bash
# View image history
docker history nginx:latest

# Output shows:
IMAGE          CREATED       CREATED BY                                      SIZE
605c77e624dd   2 weeks ago   /bin/sh -c #(nop)  CMD ["nginx" "-g" "daemon…   0B
<missing>      2 weeks ago   /bin/sh -c #(nop)  EXPOSE 80                    0B
<missing>      2 weeks ago   /bin/sh -c apt-get update && apt-get install…   54.3MB

# No truncation
docker history --no-trunc nginx:latest

# Human-readable sizes
docker history --human=true nginx:latest

# Show only size
docker history --format "{{.Size}}" nginx:latest
```

**Analyze Layer Sizes:**

```bash
# Find largest layers
docker history --format "{{.Size}}\t{{.CreatedBy}}" nginx:latest | sort -hr

# Check specific image
docker history myapp:latest

# Identify optimization opportunities
# Large layers = candidates for optimization
```

---

### 6.8 Pruning Unused Images

**Safai karo - cleanup unused images:**

```bash
# Remove dangling images (untagged)
docker image prune

# Remove all unused images
docker image prune -a

# Force prune (no confirmation)
docker image prune -f

# Prune with filters
docker image prune --filter "until=24h"    # Older than 24 hours
docker image prune --filter "until=720h"   # Older than 30 days
docker image prune --filter "label=stage=build"  # With specific label
```

**Cleanup Script:**

```bash
#!/bin/bash
# docker-image-cleanup.sh

echo "🧹 Cleaning Docker images..."

echo "📊 Current disk usage:"
docker system df

echo ""
echo "🗑️  Removing dangling images..."
docker image prune -f

echo ""
echo "🗑️  Removing images older than 30 days..."
docker image prune -a --filter "until=720h" -f

echo ""
echo "📊 After cleanup:"
docker system df

# Calculate space saved
echo ""
echo "✅ Cleanup complete!"
```

**Automated Cleanup (Cron Job):**

```bash
# Add to crontab (run daily at 2 AM)
# crontab -e

0 2 * * * /usr/local/bin/docker image prune -a --filter "until=168h" -f
```

---

## Chapter 7: Docker Container CLI

### 7.1 Running Containers

**Container chalana - sabse important command!**

**Basic Run:**

```bash
# Simple run
docker run nginx

# Run in background (detached mode)
docker run -d nginx

# Run with name
docker run -d --name my-nginx nginx

# Run with port mapping
docker run -d -p 8080:80 nginx

# Run and remove after exit
docker run --rm nginx

# Run interactively
docker run -it ubuntu bash
```

**Common Flags:**

```bash
-d, --detach          # Run in background
-it                   # Interactive terminal
-p, --publish         # Port mapping (host:container)
-e, --env             # Environment variables
-v, --volume          # Mount volumes
--name                # Container name
--rm                  # Auto-remove when stopped
--network             # Connect to network
--restart             # Restart policy
-m, --memory          # Memory limit
--cpus                # CPU limit
```

**Real-world Examples:**

**1. Web Server:**

```bash
# Run Nginx web server
docker run -d \
  --name my-website \
  -p 80:80 \
  -v $(pwd)/html:/usr/share/nginx/html:ro \
  nginx:alpine

# Access: http://localhost
```

**2. Database:**

```bash
# Run PostgreSQL database
docker run -d \
  --name postgres-db \
  -e POSTGRES_PASSWORD=secret123 \
  -e POSTGRES_DB=myapp \
  -p 5432:5432 \
  -v pgdata:/var/lib/postgresql/data \
  postgres:14
```

**3. Development Environment:**

```bash
# Run Node.js development environment
docker run -it --rm \
  --name node-dev \
  -v $(pwd):/app \
  -w /app \
  -p 3000:3000 \
  node:18 \
  bash

# Inside container:
# npm install
# npm start
```

**4. Temporary Testing:**

```bash
# Quick test with auto-cleanup
docker run --rm -it ubuntu:22.04 bash

# Test Python script
docker run --rm -v $(pwd):/app python:3.11 python /app/script.py

# Run one-off command
docker run --rm alpine:latest echo "Hello Docker!"
```

---

### 7.2 Listing Containers

**Apne containers ki list dekho:**

```bash
# List running containers
docker ps

# List all containers (including stopped)
docker ps -a

# List with specific format
docker ps --format "table {{.ID}}\t{{.Names}}\t{{.Status}}"

# List only container IDs
docker ps -q

# List with size information
docker ps -s
```

**Advanced Filtering:**

```bash
# Filter by status
docker ps --filter "status=running"
docker ps --filter "status=exited"
docker ps --filter "status=paused"

# Filter by name
docker ps --filter "name=nginx"

# Filter by ancestor (image)
docker ps --filter "ancestor=nginx"

# Filter by label
docker ps --filter "label=environment=production"

# Combine filters
docker ps --filter "status=running" --filter "ancestor=nginx"
```

**Custom Formats:**

```bash
# Show specific columns
docker ps --format "{{.Names}}: {{.Status}}"

# Table format with custom columns
docker ps --format "table {{.Names}}\t{{.Image}}\t{{.Ports}}\t{{.Status}}"

# JSON output
docker ps --format "{{json .}}" | jq
```

**Real-world Monitoring:**

```bash
# Monitor script
#!/bin/bash

echo "🐳 Docker Container Status"
echo "=========================="
docker ps --format "table {{.Names}}\t{{.Status}}\t{{.Ports}}"

echo ""
echo "📊 Resource Usage:"
docker stats --no-stream --format "table {{.Container}}\t{{.CPUPerc}}\t{{.MemUsage}}"
```

---

### 7.3 Starting and Stopping Containers

**Container ko start aur stop karo:**

**Stop Container:**

```bash
# Graceful stop (sends SIGTERM, waits 10s, then SIGKILL)
docker stop mycontainer

# Stop multiple containers
docker stop container1 container2 container3

# Stop all running containers
docker stop $(docker ps -q)

# Stop with custom timeout
docker stop -t 30 mycontainer  # Wait 30 seconds before SIGKILL
```

**Start Container:**

```bash
# Start stopped container
docker start mycontainer

# Start multiple containers
docker start container1 container2

# Start and attach to container
docker start -a mycontainer

# Start with interactive terminal
docker start -ai mycontainer
```

**Restart Container:**

```bash
# Restart container
docker restart mycontainer

# Restart with timeout
docker restart -t 30 mycontainer

# Restart all running containers
docker restart $(docker ps -q)
```

**Kill Container:**

```bash
# Force kill (immediate SIGKILL)
docker kill mycontainer

# Kill with specific signal
docker kill --signal=SIGINT mycontainer
```

**Restart Policies:**

```bash
# No restart (default)
docker run -d --restart=no nginx

# Always restart
docker run -d --restart=always nginx

# Restart on failure
docker run -d --restart=on-failure nginx

# Restart on failure with max retries
docker run -d --restart=on-failure:5 nginx

# Restart unless stopped manually
docker run -d --restart=unless-stopped nginx
```

**Real-world Scenarios:**

```bash
# Production web server (always restart)
docker run -d \
  --name prod-web \
  --restart=always \
  -p 80:80 \
  nginx:alpine

# Development database (restart unless stopped)
docker run -d \
  --name dev-db \
  --restart=unless-stopped \
  -p 5432:5432 \
  postgres:14

# Batch job (restart on failure, max 3 times)
docker run -d \
  --name batch-job \
  --restart=on-failure:3 \
  myapp:latest
```

---

### 7.4 Removing Containers

**Containers ko delete karo:**

```bash
# Remove stopped container
docker rm mycontainer

# Force remove running container
docker rm -f mycontainer

# Remove multiple containers
docker rm container1 container2 container3

# Remove all stopped containers
docker rm $(docker ps -aq --filter "status=exited")

# Container prune (remove all stopped)
docker container prune

# Force prune
docker container prune -f

# Prune with filter
docker container prune --filter "until=24h"
```

**Auto-removal:**

```bash
# Container removes itself on exit
docker run --rm ubuntu echo "Hello World"

# Useful for testing
docker run --rm -it python:3.11 python
```

**Cleanup Script:**

```bash
#!/bin/bash
# cleanup-containers.sh

echo "🗑️  Removing exited containers..."
docker rm $(docker ps -aq --filter "status=exited")

echo "🗑️  Removing created containers..."
docker rm $(docker ps -aq --filter "status=created")

echo "✅ Cleanup complete!"
docker ps -a
```

---

### 7.5 Executing Commands in Running Containers

**Running container me command chalao:**

```bash
# Execute command
docker exec mycontainer ls -la

# Interactive bash shell
docker exec -it mycontainer bash

# Execute as specific user
docker exec -u root mycontainer apt-get update

# Execute with environment variable
docker exec -e MY_VAR=value mycontainer env

# Execute in specific directory
docker exec -w /app mycontainer ls
```

**Common Use Cases:**

**1. Debugging:**

```bash
# Access container shell
docker exec -it my-app bash

# Check logs inside container
docker exec my-app cat /var/log/app.log

# Check processes
docker exec my-app ps aux

# Check network
docker exec my-app netstat -tulpn
```

**2. Database Operations:**

```bash
# PostgreSQL
docker exec -it postgres-db psql -U postgres

# MySQL
docker exec -it mysql-db mysql -u root -p

# MongoDB
docker exec -it mongo-db mongo

# Redis
docker exec -it redis-cache redis-cli
```

**3. File Operations:**

```bash
# Create file
docker exec my-container touch /tmp/testfile

# View file
docker exec my-container cat /etc/nginx/nginx.conf

# Edit file (if vim is installed)
docker exec -it my-container vim /app/config.yaml
```

**4. Application Management:**

```bash
# Restart application inside container
docker exec my-app supervisorctl restart app

# Clear cache
docker exec my-app php artisan cache:clear

# Run migrations
docker exec my-app python manage.py migrate
```

---

### 7.6 Viewing Container Logs

**Container logs dekho:**

```bash
# View logs
docker logs mycontainer

# Follow logs (live tail)
docker logs -f mycontainer

# Show timestamps
docker logs -t mycontainer

# Show last N lines
docker logs --tail 100 mycontainer

# Show logs since timestamp
docker logs --since 2024-01-01T00:00:00 mycontainer

# Show logs until timestamp
docker logs --until 2024-01-01T12:00:00 mycontainer

# Combine options
docker logs -f --tail 50 -t mycontainer
```

**Advanced Log Management:**

```bash
# Logs since duration
docker logs --since 10m mycontainer  # Last 10 minutes
docker logs --since 1h mycontainer   # Last 1 hour
docker logs --since 24h mycontainer  # Last 24 hours

# Filter logs (using grep)
docker logs mycontainer 2>&1 | grep ERROR
docker logs mycontainer 2>&1 | grep -i warning

# Save logs to file
docker logs mycontainer > container.log

# Follow and save
docker logs -f mycontainer | tee container.log
```

**Real-world Monitoring:**

```bash
# Monitor multiple containers
#!/bin/bash

# Follow logs from multiple containers with labels
docker logs -f --tail 20 web-app 2>&1 | sed 's/^/[WEB] /' &
docker logs -f --tail 20 api-app 2>&1 | sed 's/^/[API] /' &
docker logs -f --tail 20 db-app 2>&1 | sed 's/^/[DB] /' &

wait
```

**Log Drivers:**

```bash
# Run with specific log driver
docker run -d \
  --name myapp \
  --log-driver json-file \
  --log-opt max-size=10m \
  --log-opt max-file=3 \
  nginx

# Logging to syslog
docker run -d \
  --log-driver syslog \
  --log-opt syslog-address=tcp://192.168.1.100:514 \
  nginx

# Disable logging
docker run -d --log-driver none nginx
```

---

### 7.7 Inspecting Containers

**Container ki complete details dekho:**

```bash
# Full inspection
docker inspect mycontainer

# Specific information
docker inspect --format='{{.State.Status}}' mycontainer
docker inspect --format='{{.NetworkSettings.IPAddress}}' mycontainer
docker inspect --format='{{.Config.Image}}' mycontainer

# Environment variables
docker inspect --format='{{range .Config.Env}}{{println .}}{{end}}' mycontainer

# Mounts/Volumes
docker inspect --format='{{json .Mounts}}' mycontainer | jq

# Network settings
docker inspect --format='{{json .NetworkSettings}}' mycontainer | jq
```

**Useful Inspection Commands:**

```bash
# Get container IP
docker inspect -f '{{range .NetworkSettings.Networks}}{{.IPAddress}}{{end}}' mycontainer

# Get port mappings
docker inspect --format='{{json .NetworkSettings.Ports}}' mycontainer | jq

# Get container start time
docker inspect --format='{{.State.StartedAt}}' mycontainer

# Check if container is running
docker inspect --format='{{.State.Running}}' mycontainer

# Get exit code
docker inspect --format='{{.State.ExitCode}}' mycontainer

# Get resource limits
docker inspect --format='{{.HostConfig.Memory}}' mycontainer
docker inspect --format='{{.HostConfig.NanoCpus}}' mycontainer
```

---

### 7.8 Copying Files Between Host and Container

**Files copy karo host aur container ke beech:**

```bash
# Copy from host to container
docker cp /path/on/host/file.txt mycontainer:/path/in/container/

# Copy from container to host
docker cp mycontainer:/path/in/container/file.txt /path/on/host/

# Copy directory
docker cp /path/to/directory mycontainer:/app/

# Copy from container directory
docker cp mycontainer:/app/logs/ ./local-logs/

# Preserve permissions
docker cp -a mycontainer:/app/ ./backup/
```

**Real-world Examples:**

**1. Deploy Configuration:**

```bash
# Copy updated config to running container
docker cp ./config/app.yaml my-app:/etc/app/config.yaml

# Restart app to load new config
docker restart my-app
```

**2. Extract Logs:**

```bash
# Copy logs from container
docker cp my-app:/var/log/app.log ./logs/

# Copy entire log directory
docker cp my-app:/var/log/ ./backup-logs/
```

**3. Development Workflow:**

```bash
# Copy built files into container
docker cp ./dist/ my-app:/usr/share/nginx/html/

# Extract generated files
docker cp my-app:/app/generated ./local-generated/
```

**4. Backup Data:**

```bash
# Backup database data
docker cp postgres-db:/var/lib/postgresql/data ./db-backup/

# Restore backup
docker cp ./db-backup/ postgres-db:/var/lib/postgresql/data/
```

---

### 7.9 Container Resource Management

**Container ko resources allocate karo:**

**Memory Limits:**

```bash
# Set memory limit
docker run -d -m 512m nginx  # 512 MB limit

# Memory with swap
docker run -d -m 512m --memory-swap 1g nginx

# Memory reservation (soft limit)
docker run -d --memory-reservation 256m nginx

# OOM killer control
docker run -d -m 512m --oom-kill-disable nginx
```

**CPU Limits:**

```bash
# CPU shares (relative weight)
docker run -d --cpu-shares 512 nginx  # Default is 1024

# CPU limit (percentage)
docker run -d --cpus 1.5 nginx  # 1.5 CPUs

# CPU period and quota
docker run -d --cpu-period 100000 --cpu-quota 50000 nginx  # 50% of one CPU

# CPU set (specific CPUs)
docker run -d --cpuset-cpus 0,1 nginx  # Only use CPU 0 and 1
```

**Real-world Resource Allocation:**

```bash
# Web server (moderate resources)
docker run -d \
  --name web-server \
  -m 1g \
  --cpus 2 \
  -p 80:80 \
  nginx:alpine

# Database (high resources)
docker run -d \
  --name database \
  -m 4g \
  --memory-reservation 2g \
  --cpus 4 \
  -p 5432:5432 \
  postgres:14

# Background worker (low resources)
docker run -d \
  --name worker \
  -m 256m \
  --cpus 0.5 \
  myapp:worker

# Development container (limited resources)
docker run -it \
  --name dev-env \
  -m 512m \
  --cpus 1 \
  -v $(pwd):/workspace \
  node:18
```

**Update Resource Limits:**

```bash
# Update running container memory
docker update --memory 2g mycontainer

# Update CPU limit
docker update --cpus 2 mycontainer

# Update multiple containers
docker update --memory 1g --cpus 1.5 container1 container2

# Update all containers
docker update --restart=always $(docker ps -q)
```

---

### 7.10 Container Statistics

**Container ki real-time stats dekho:**

```bash
# Stats for all running containers
docker stats

# Stats for specific container
docker stats mycontainer

# One-time stats (not streaming)
docker stats --no-stream

# Stats with custom format
docker stats --format "table {{.Container}}\t{{.CPUPerc}}\t{{.MemUsage}}\t{{.NetIO}}"

# Stats without container names
docker stats $(docker ps -q)
```

**Understanding Stats Output:**

```
CONTAINER ID   NAME        CPU %     MEM USAGE / LIMIT   MEM %     NET I/O       BLOCK I/O
1234567890ab   web-app     2.50%     150MB / 1GB         15.00%    1.2MB / 800KB  0B / 0B
```

**Monitoring Script:**

```bash
#!/bin/bash
# monitor-containers.sh

echo "🐳 Docker Container Monitoring"
echo "=============================="

while true; do
    clear
    echo "📊 Resource Usage ($(date))"
    echo ""
    docker stats --no-stream --format "table {{.Name}}\t{{.CPUPerc}}\t{{.MemUsage}}\t{{.MemPerc}}\t{{.NetIO}}"
    
    echo ""
    echo "📦 Container Status:"
    docker ps --format "table {{.Names}}\t{{.Status}}\t{{.Ports}}"
    
    sleep 5
done
```

---

## Chapter 8: Dockerfile

### 8.1 What is a Dockerfile?

**Dekh bhai**, Dockerfile ek text file hai jo instructions contain karta hai Docker image build karne ke liye. Ye blueprint hai tumhare custom image ka.

**Basic Structure:**

```dockerfile
# Start from a base image
FROM ubuntu:22.04

# Set working directory
WORKDIR /app

# Copy files
COPY . .

# Install dependencies
RUN apt-get update && apt-get install -y python3

# Expose port
EXPOSE 8080

# Command to run
CMD ["python3", "app.py"]
```

**Dockerfile Benefits:**

- Version control your infrastructure
- Reproducible builds
- Automated image creation
- Documentation of image contents

---

### 8.2 Dockerfile Instructions

**Har instruction ka meaning:**

**FROM - Base Image:**

```dockerfile
# Official image
FROM node:18

# Specific version
FROM python:3.11-slim

# Multi-stage build
FROM node:18 AS builder
FROM nginx:alpine AS runtime
```

**WORKDIR - Set Working Directory:**

```dockerfile
# Set and create working directory
WORKDIR /app

# All subsequent commands run in /app
# If directory doesn't exist, it's created
```

**COPY - Copy Files:**

```dockerfile
# Copy single file
COPY app.py /app/

# Copy directory
COPY ./src /app/src

# Copy with specific ownership
COPY --chown=user:group app.py /app/

# Copy from build stage (multi-stage)
COPY --from=builder /app/dist /app/
```

**ADD - Add Files (with extra features):**

```dockerfile
# Similar to COPY but can:
# - Extract tar files
# - Download from URLs

ADD archive.tar.gz /app/  # Automatically extracts
ADD https://example.com/file.txt /app/

# Prefer COPY over ADD unless you need these features
```

**RUN - Execute Commands:**

```dockerfile
# Shell form
RUN apt-get update && apt-get install -y python3

# Exec form (preferred)
RUN ["apt-get", "update"]

# Multiple commands
RUN apt-get update && \
    apt-get install -y \
        python3 \
        python3-pip \
        git && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*
```

**CMD - Default Command:**

```dockerfile
# Exec form (preferred)
CMD ["python3", "app.py"]

# Shell form
CMD python3 app.py

# Can be overridden at runtime
# docker run myimage node server.js  # Overrides CMD
```

**ENTRYPOINT - Main Executable:**

```dockerfile
# Exec form
ENTRYPOINT ["python3"]

# Combined with CMD
ENTRYPOINT ["python3"]
CMD ["app.py"]

# Result: python3 app.py
# Can append: docker run myimage script.py → python3 script.py
```

**ENV - Environment Variables:**

```dockerfile
# Single variable
ENV NODE_ENV=production

# Multiple variables
ENV NODE_ENV=production \
    PORT=3000 \
    DB_HOST=localhost
```

**EXPOSE - Document Ports:**

```dockerfile
# Single port
EXPOSE 8080

# Multiple ports
EXPOSE 8080 9090

# With protocol
EXPOSE 8080/tcp
EXPOSE 53/udp

# Note: EXPOSE doesn't actually publish ports
# Use -p flag when running: docker run -p 8080:8080 myimage
```

**VOLUME - Create Mount Points:**

```dockerfile
# Single volume
VOLUME /data

# Multiple volumes
VOLUME ["/data", "/logs"]

# Creates anonymous volume if not specified at runtime
```

**ARG - Build-time Variables:**

```dockerfile
# Define argument
ARG VERSION=latest
ARG BUILD_DATE

# Use in Dockerfile
FROM node:${VERSION}
LABEL build_date=${BUILD_DATE}

# Pass during build:
# docker build --build-arg VERSION=18 --build-arg BUILD_DATE=2024-01-01 .
```

**LABEL - Metadata:**

```dockerfile
# Add metadata
LABEL maintainer="you@example.com"
LABEL version="1.0"
LABEL description="My awesome app"

# Multiple labels
LABEL maintainer="you@example.com" \
      version="1.0" \
      description="My awesome app"
```

**USER - Set User:**

```dockerfile
# Switch to non-root user
USER node

# All subsequent commands run as this user
# Good security practice!
```

**SHELL - Change Default Shell:**

```dockerfile
# Default is ["/bin/sh", "-c"]
SHELL ["/bin/bash", "-c"]

# Now RUN commands use bash
RUN source ~/.bashrc && echo $MY_VAR
```

---

### 8.3 Building Images from Dockerfile

**Image build karo:**

**Basic Build:**

```bash
# Build from current directory
docker build .

# Build with tag
docker build -t myapp:latest .

# Build with multiple tags
docker build -t myapp:latest -t myapp:v1.0 .

# Build from specific Dockerfile
docker build -f Dockerfile.prod -t myapp:prod .

# Build with build arguments
docker build --build-arg VERSION=18 -t myapp .
```

**Build Options:**

```bash
# No cache (fresh build)
docker build --no-cache -t myapp .

# Pull latest base image
docker build --pull -t myapp .

# Specify platform
docker build --platform linux/amd64 -t myapp .

# Set target stage (multi-stage builds)
docker build --target builder -t myapp:builder .

# View build output
docker build --progress=plain -t myapp .

# Limit build resources
docker build --memory 2g --cpu-shares 512 -t myapp .
```

**Real-world Build Example:**

```dockerfile
# Dockerfile
FROM node:18-alpine AS builder

WORKDIR /app
COPY package*.json ./
RUN npm ci --only=production

COPY . .
RUN npm run build

FROM nginx:alpine
COPY --from=builder /app/dist /usr/share/nginx/html
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
```

```bash
# Build commands
docker build -t myapp:latest .
docker build -t myapp:v1.0.0 .
docker build --no-cache -t myapp:latest .  # Fresh build
docker build --target builder -t myapp:builder .  # Build only builder stage
```

---

### 8.4 Best Practices for Dockerfile

**Achhi Dockerfile likhne ke tips:**

**1. Use Specific Base Image Tags:**

```dockerfile
# ❌ Bad - version changes unexpectedly
FROM node:latest

# ✅ Good - specific version
FROM node:18.17-alpine
```

**2. Minimize Layers:**

```dockerfile
# ❌ Bad - multiple layers
RUN apt-get update
RUN apt-get install -y python3
RUN apt-get install -y pip

# ✅ Good - single layer
RUN apt-get update && \
    apt-get install -y python3 pip && \
    rm -rf /var/lib/apt/lists/*
```

**3. Order Instructions for Cache:**

```dockerfile
# ✅ Good - dependency files first
FROM node:18-alpine
WORKDIR /app

# These change rarely - good cache
COPY package*.json ./
RUN npm ci

# These change often - at the end
COPY . .

CMD ["node", "server.js"]
```

**4. Use .dockerignore:**

```
# .dockerignore
node_modules
npm-debug.log
.git
.env
*.md
.DS_Store
```

**5. Don't Run as Root:**

```dockerfile
# ✅ Good - create and use non-root user
FROM node:18-alpine

RUN addgroup -g 1001 -S nodejs && \
    adduser -S nodejs -u 1001

WORKDIR /app
COPY --chown=nodejs:nodejs . .

USER nodejs
CMD ["node", "server.js"]
```

**6. Use Multi-stage Builds:**

```dockerfile
# ✅ Good - smaller final image
FROM node:18 AS builder
WORKDIR /app
COPY package*.json ./
RUN npm ci
COPY . .
RUN npm run build

FROM node:18-alpine
WORKDIR /app
COPY --from=builder /app/dist ./dist
COPY --from=builder /app/node_modules ./node_modules
CMD ["node", "dist/server.js"]
```

**7. Leverage Build Cache:**

```dockerfile
# ✅ Good - separate steps for better caching
COPY package*.json ./
RUN npm ci  # Only runs if package.json changes

COPY src/ ./src/
RUN npm run build  # Only runs if src changes
```

**8. Clean Up in Same Layer:**

```dockerfile
# ✅ Good - cleanup in same RUN command
RUN apt-get update && \
    apt-get install -y python3 && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
```

---

### 8.5 Multi-stage Builds

**Chote aur efficient images banao:**

**Why Multi-stage?**

- Smaller final image (only runtime dependencies)
- Separate build and runtime environments
- Better security (no build tools in production)

**Basic Multi-stage:**

```dockerfile
# Stage 1: Build
FROM golang:1.21 AS builder
WORKDIR /app
COPY . .
RUN go build -o myapp

# Stage 2: Runtime
FROM alpine:latest
WORKDIR /app
COPY --from=builder /app/myapp .
CMD ["./myapp"]
```

**Node.js Example:**

```dockerfile
# Build stage
FROM node:18 AS builder
WORKDIR /app
COPY package*.json ./
RUN npm ci
COPY . .
RUN npm run build
RUN npm prune --production

# Production stage
FROM node:18-alpine
WORKDIR /app

# Copy only necessary files
COPY --from=builder /app/dist ./dist
COPY --from=builder /app/node_modules ./node_modules
COPY --from=builder /app/package.json ./

USER node
EXPOSE 3000
CMD ["node", "dist/server.js"]
```

**Size Comparison:**

```bash
# Without multi-stage
docker build -t myapp:single .
# Size: 1.2GB (includes build tools, source files, etc.)

# With multi-stage
docker build -t myapp:multi .
# Size: 150MB (only runtime dependencies)
```

**Python Example:**

```dockerfile
# Build stage
FROM python:3.11 AS builder
WORKDIR /app
COPY requirements.txt .
RUN pip install --user --no-cache-dir -r requirements.txt

# Runtime stage
FROM python:3.11-slim
WORKDIR /app

# Copy installed packages
COPY --from=builder /root/.local /root/.local
COPY . .

# Update PATH
ENV PATH=/root/.local/bin:$PATH

CMD ["python", "app.py"]
```

**Named Stages and Multiple Outputs:**

```dockerfile
# Build frontend
FROM node:18 AS frontend-builder
WORKDIR /frontend
COPY frontend/package*.json ./
RUN npm ci
COPY frontend/ ./
RUN npm run build

# Build backend
FROM golang:1.21 AS backend-builder
WORKDIR /backend
COPY backend/ ./
RUN go build -o server

# Final runtime stage
FROM alpine:latest
WORKDIR /app

# Copy from both stages
COPY --from=frontend-builder /frontend/dist ./public
COPY --from=backend-builder /backend/server ./

EXPOSE 8080
CMD ["./server"]
```

**Build Specific Stage:**

```bash
# Build only the builder stage (for testing)
docker build --target builder -t myapp:builder .

# Build final stage (default)
docker build -t myapp:latest .
```

---

### 8.6 .dockerignore File

**.dockerignore - Kya include nahi karna:**

**Why .dockerignore?**

- Faster builds (less data to copy)
- Smaller build context
- Avoid copying sensitive files
- Prevent unnecessary cache invalidation

**Basic .dockerignore:**

```
# .dockerignore

# Version control
.git
.gitignore
.gitattributes

# Dependencies
node_modules
vendor
venv
__pycache__

# Build outputs
dist
build
*.egg-info
target

# Logs
*.log
logs

# OS files
.DS_Store
Thumbs.db

# IDE
.vscode
.idea
*.swp
*.swo

# Environment files
.env
.env.local
*.pem
*.key

# Documentation
README.md
CHANGELOG.md
docs

# Tests
tests
*.test.js
__tests__

# CI/CD
.github
.gitlab-ci.yml
.travis.yml

# Docker files (if present)
Dockerfile*
docker-compose*.yml
```

**Project-specific Examples:**

**Node.js Project:**

```
node_modules
npm-debug.log
.npm
coverage
.nyc_output
.cache
dist
build
```

**Python Project:**

```
__pycache__
*.py[cod]
*$py.class
*.so
.Python
venv
ENV
.venv
*.egg-info
dist
build
```

**Go Project:**

```
vendor
*.exe
*.test
*.prof
.go
bin
pkg
```

**Pattern Matching:**

```
# Ignore all markdown files
*.md

# But don't ignore README.md
!README.md

# Ignore everything in temp directory
temp/**

# Ignore all .log files in any directory
**/*.log

# Ignore specific files
secret.txt
credentials.json
```

**Verification:**

```bash
# Check what files are being sent to build context
docker build --no-cache --progress=plain . 2>&1 | grep "^#"

# Or use docker context
docker context ls
```

---

## Chapter 9: Containerizing Applications

### 9.1 Containerizing a Node.js Application

**Node.js app ko containerize karo:**

**Project Structure:**

```
my-node-app/
├── src/
│   ├── server.js
│   └── routes/
├── package.json
├── package-lock.json
├── .dockerignore
└── Dockerfile
```

**Simple Node.js App (server.js):**

```javascript
// src/server.js
const express = require('express');
const app = express();
const PORT = process.env.PORT || 3000;

app.get('/', (req, res) => {
  res.json({ message: 'Hello from Docker!' });
});

app.get('/health', (req, res) => {
  res.json({ status: 'healthy' });
});

app.listen(PORT, '0.0.0.0', () => {
  console.log(`Server running on port ${PORT}`);
});
```

**package.json:**

```json
{
  "name": "my-node-app",
  "version": "1.0.0",
  "main": "src/server.js",
  "scripts": {
    "start": "node src/server.js",
    "dev": "nodemon src/server.js"
  },
  "dependencies": {
    "express": "^4.18.2"
  }
}
```

**Dockerfile (Production-ready):**

```dockerfile
# Build stage
FROM node:18-alpine AS builder

WORKDIR /app

# Copy dependency files
COPY package*.json ./

# Install dependencies
RUN npm ci --only=production

# Copy application code
COPY src/ ./src/

# Production stage
FROM node:18-alpine

# Create non-root user
RUN addgroup -g 1001 -S nodejs && \
    adduser -S nodejs -u 1001

WORKDIR /app

# Copy from builder
COPY --from=builder --chown=nodejs:nodejs /app/node_modules ./node_modules
COPY --chown=nodejs:nodejs package*.json ./
COPY --chown=nodejs:nodejs src/ ./src/

# Switch to non-root user
USER nodejs

# Expose port
EXPOSE 3000

# Health check
HEALTHCHECK --interval=30s --timeout=3s --start-period=5s --retries=3 \
  CMD node -e "require('http').get('http://localhost:3000/health', (r) => {process.exit(r.statusCode === 200 ? 0 : 1)})"

# Start application
CMD ["node", "src/server.js"]
```

**.dockerignore:**

```
node_modules
npm-debug.log
.git
.env
README.md
```

**Build and Run:**

```bash
# Build image
docker build -t my-node-app:latest .

# Run container
docker run -d \
  --name node-app \
  -p 3000:3000 \
  -e PORT=3000 \
  my-node-app:latest

# Test
curl http://localhost:3000
# Output: {"message":"Hello from Docker!"}

# View logs
docker logs -f node-app

# Stop and remove
docker stop node-app
docker rm node-app
```

**Development Dockerfile:**

```dockerfile
# Dockerfile.dev
FROM node:18-alpine

WORKDIR /app

COPY package*.json ./
RUN npm install

COPY . .

EXPOSE 3000

CMD ["npm", "run", "dev"]
```

**Development Setup:**

```bash
# Build dev image
docker build -f Dockerfile.dev -t my-node-app:dev .

# Run with volume mount for hot reload
docker run -d \
  --name node-dev \
  -p 3000:3000 \
  -v $(pwd)/src:/app/src \
  my-node-app:dev
```

---

### 9.2 Containerizing a Python Application

**Python app ko containerize karo:**

**Project Structure:**

```
my-python-app/
├── app/
│   ├── __init__.py
│   ├── main.py
│   └── routes.py
├── requirements.txt
├── .dockerignore
└── Dockerfile
```

**Simple Flask App (app/main.py):**

```python
# app/main.py
from flask import Flask, jsonify
import os

app = Flask(__name__)

@app.route('/')
def home():
    return jsonify({"message": "Hello from Docker Python!"})

@app.route('/health')
def health():
    return jsonify({"status": "healthy"})

if __name__ == '__main__':
    port = int(os.environ.get('PORT', 5000))
    app.run(host='0.0.0.0', port=port, debug=False)
```

**requirements.txt:**

```
Flask==2.3.3
gunicorn==21.2.0
```

**Dockerfile (Production-ready):**

```dockerfile
# Build stage
FROM python:3.11-slim AS builder

WORKDIR /app

# Install dependencies
COPY requirements.txt .
RUN pip install --user --no-cache-dir -r requirements.txt

# Runtime stage
FROM python:3.11-slim

# Create non-root user
RUN useradd -m -u 1000 appuser

WORKDIR /app

# Copy installed packages from builder
COPY --from=builder /root/.local /home/appuser/.local

# Copy application code
COPY --chown=appuser:appuser app/ ./app/

# Update PATH
ENV PATH=/home/appuser/.local/bin:$PATH

# Switch to non-root user
USER appuser

# Expose port
EXPOSE 5000

# Health check
HEALTHCHECK --interval=30s --timeout=3s --start-period=5s \
  CMD python -c "import urllib.request; urllib.request.urlopen('http://localhost:5000/health')"

# Run with gunicorn
CMD ["gunicorn", "--bind", "0.0.0.0:5000", "--workers", "4", "app.main:app"]
```

**.dockerignore:**

```
__pycache__
*.pyc
*.pyo
*.pyd
.Python
venv
ENV
.venv
*.egg-info
dist
build
.pytest_cache
.coverage
htmlcov
.git
.env
README.md
```

**Build and Run:**

```bash
# Build image
docker build -t my-python-app:latest .

# Run container
docker run -d \
  --name python-app \
  -p 5000:5000 \
  -e PORT=5000 \
  my-python-app:latest

# Test
curl http://localhost:5000
# Output: {"message":"Hello from Docker Python!"}

# View logs
docker logs -f python-app
```

**Django Example:**

```dockerfile
FROM python:3.11-slim

WORKDIR /app

# Install system dependencies
RUN apt-get update && \
    apt-get install -y --no-install-recommends \
        postgresql-client && \
    rm -rf /var/lib/apt/lists/*

# Install Python dependencies
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy project
COPY . .

# Collect static files
RUN python manage.py collectstatic --noinput

EXPOSE 8000

CMD ["gunicorn", "--bind", "0.0.0.0:8000", "myproject.wsgi:application"]
```

---

### 9.3 Containerizing a Java Application

**Java app ko containerize karo:**

**Project Structure:**

```
my-java-app/
├── src/
│   └── main/
│       ├── java/
│       └── resources/
├── pom.xml
├── Dockerfile
└── .dockerignore
```

**Spring Boot Application:**

**Dockerfile (Maven):**

```dockerfile
# Build stage
FROM maven:3.9-openjdk-17 AS builder

WORKDIR /app

# Copy dependency files
COPY pom.xml .
RUN mvn dependency:go-offline

# Copy source and build
COPY src ./src
RUN mvn clean package -DskipTests

# Runtime stage
FROM openjdk:17-jdk-slim

WORKDIR /app

# Create non-root user
RUN useradd -m -u 1000 javauser

# Copy JAR from builder
COPY --from=builder /app/target/*.jar app.jar

# Change ownership
RUN chown javauser:javauser app.jar

USER javauser

EXPOSE 8080

# Health check
HEALTHCHECK --interval=30s --timeout=3s --start-period=40s \
  CMD curl -f http://localhost:8080/actuator/health || exit 1

ENTRYPOINT ["java", "-jar", "app.jar"]
```

**Dockerfile (Gradle):**

```dockerfile
# Build stage
FROM gradle:8.4-jdk17 AS builder

WORKDIR /app

# Copy gradle files
COPY build.gradle settings.gradle ./
COPY gradle ./gradle

# Download dependencies
RUN gradle dependencies --no-daemon

# Copy source and build
COPY src ./src
RUN gradle bootJar --no-daemon

# Runtime stage
FROM openjdk:17-jdk-slim

WORKDIR /app

RUN useradd -m -u 1000 javauser

COPY --from=builder /app/build/libs/*.jar app.jar

RUN chown javauser:javauser app.jar

USER javauser

EXPOSE 8080

ENTRYPOINT ["java", "-jar", "app.jar"]
```

**Optimized with JLink (Smaller Image):**

```dockerfile
FROM openjdk:17-jdk-slim AS builder

WORKDIR /app

COPY pom.xml .
COPY src ./src

RUN apt-get update && apt-get install -y maven
RUN mvn clean package -DskipTests

# Create custom JRE
RUN jlink \
    --add-modules java.base,java.logging,java.xml,jdk.unsupported \
    --strip-debug \
    --no-man-pages \
    --no-header-files \
    --compress=2 \
    --output /javaruntime

# Runtime stage
FROM debian:bullseye-slim

ENV JAVA_HOME=/opt/java/openjdk
ENV PATH "${JAVA_HOME}/bin:${PATH}"

COPY --from=builder /javaruntime $JAVA_HOME
COPY --from=builder /app/target/*.jar app.jar

EXPOSE 8080

ENTRYPOINT ["java", "-jar", "app.jar"]
```

**.dockerignore:**

```
target
build
.gradle
*.class
*.log
.git
.idea
*.iml
.settings
.classpath
.project
```

**Build and Run:**

```bash
# Build image
docker build -t my-java-app:latest .

# Run container
docker run -d \
  --name java-app \
  -p 8080:8080 \
  -e SPRING_PROFILES_ACTIVE=prod \
  -e JAVA_OPTS="-Xmx512m -Xms256m" \
  my-java-app:latest

# View logs
docker logs -f java-app
```

---

### 9.4 Environment Variables in Containers

**Environment variables ka use:**

**Setting Environment Variables:**

```bash
# Single variable
docker run -e PORT=3000 my-app

# Multiple variables
docker run \
  -e NODE_ENV=production \
  -e DB_HOST=postgres \
  -e DB_PORT=5432 \
  my-app

# From file
docker run --env-file .env my-app
```

**.env File:**

```bash
# .env
NODE_ENV=production
PORT=3000
DB_HOST=postgres
DB_PORT=5432
DB_NAME=myapp
DB_USER=admin
DB_PASSWORD=secret123
```

**In Dockerfile:**

```dockerfile
# Set default environment variables
ENV NODE_ENV=production \
    PORT=3000 \
    LOG_LEVEL=info

# Can be overridden at runtime
CMD ["node", "server.js"]
```

**Access in Application:**

```javascript
// Node.js
const port = process.env.PORT || 3000;
const dbHost = process.env.DB_HOST;
```

```python
# Python
import os

port = os.environ.get('PORT', 5000)
db_host = os.environ.get('DB_HOST')
```

```java
// Java
String port = System.getenv("PORT");
String dbHost = System.getenv("DB_HOST");
```

**Real-world Example:**

```bash
# Development
docker run -d \
  --name app-dev \
  -e NODE_ENV=development \
  -e DB_HOST=localhost \
  -e LOG_LEVEL=debug \
  my-app

# Production
docker run -d \
  --name app-prod \
  -e NODE_ENV=production \
  -e DB_HOST=prod-db.example.com \
  -e LOG_LEVEL=error \
  my-app
```

---

## Chapter 10: Port Mapping

### 10.1 Understanding Port Mapping

**Port mapping kya hai?**
Container ke internal port ko host machine ke port se connect karna. Isse tum container ki services ko bahar se access kar sakte ho.

**Why Port Mapping?**

- Containers are isolated by default
- Need to expose services to host/network
- Multiple containers can use same internal port
- Host port must be unique

**Container Port vs Host Port:**

```
Host Machine (Your Computer)
Port 8080
    ↓
    ↓ (Mapping)
    ↓
Container
Port 80 (Nginx)
```

---

### 10.2 Manual Port Mapping

**Specific ports ko map karo:**

**Basic Syntax:**

```bash
docker run -p HOST_PORT:CONTAINER_PORT image

# Example
docker run -p 8080:80 nginx
# Host port 8080 → Container port 80
```

**Common Patterns:**

```bash
# Web server
docker run -d -p 80:80 nginx
# Access: http://localhost

# Custom port
docker run -d -p 8080:80 nginx
# Access: http://localhost:8080

# Different ports
docker run -d -p 3000:8080 myapp
# Container listens on 8080, accessible via 3000

# Multiple port mappings
docker run -d \
  -p 80:80 \
  -p 443:443 \
  nginx
```

**Bind to Specific Interface:**

```bash
# Bind to localhost only
docker run -d -p 127.0.0.1:8080:80 nginx
# Only accessible from localhost

# Bind to specific IP
docker run -d -p 192.168.1.100:8080:80 nginx
# Only accessible from that IP

# Bind to all interfaces (default)
docker run -d -p 8080:80 nginx
# Same as 0.0.0.0:8080:80
```

**Protocol Specification:**

```bash
# TCP (default)
docker run -d -p 8080:80/tcp nginx

# UDP
docker run -d -p 53:53/udp dns-server

# Both TCP and UDP
docker run -d \
  -p 53:53/tcp \
  -p 53:53/udp \
  dns-server
```

**Real-world Examples:**

```bash
# Web application stack
# Frontend
docker run -d --name frontend -p 80:3000 frontend-app

# API
docker run -d --name api -p 8080:8080 api-app

# Database (careful with exposing!)
docker run -d --name db -p 5432:5432 postgres

# Redis cache
docker run -d --name cache -p 6379:6379 redis
```

---

### 10.3 Automatic Port Mapping

**Docker ko automatically port assign karne do:**

```bash
# Publish all exposed ports
docker run -d -P nginx

# Docker assigns random host ports
# Check assigned ports:
docker ps
# or
docker port container_name
```

**Check Port Mappings:**

```bash
# View all port mappings for a container
docker port my-container

# Output example:
80/tcp -> 0.0.0.0:32768
443/tcp -> 0.0.0.0:32769

# Check specific port
docker port my-container 80
# Output: 0.0.0.0:32768
```

**Get Port Programmatically:**

```bash
# Get first mapped port
docker inspect --format='{{(index (index .NetworkSettings.Ports "80/tcp") 0).HostPort}}' my-container

# Get all port mappings
docker inspect --format='{{json .NetworkSettings.Ports}}' my-container | jq
```

---

### 10.4 Exposing Multiple Ports

**Multiple services ko expose karo:**

**In Dockerfile:**

```dockerfile
FROM nginx:alpine

# Expose multiple ports in Dockerfile
EXPOSE 80
EXPOSE 443
EXPOSE 8080

# Or in single line
EXPOSE 80 443 8080

CMD ["nginx", "-g", "daemon off;"]
```

**At Runtime:**

```bash
# Map multiple ports
docker run -d \
  --name multi-port-app \
  -p 80:80 \
  -p 443:443 \
  -p 8080:8080 \
  -p 9090:9090 \
  my-app

# Or use -P to publish all EXPOSE'd ports
docker run -d -P my-app
```

**Range of Ports:**

```bash
# Map port range
docker run -d -p 8000-8010:8000-8010 my-app
# Maps 8000→8000, 8001→8001, ..., 8010→8010
```

**Real-world Multi-Port Application:**

```dockerfile
# Dockerfile for app with multiple services
FROM node:18-alpine

WORKDIR /app

COPY package*.json ./
RUN npm ci

COPY . .

# Main app
EXPOSE 3000
# Admin panel
EXPOSE 4000
# Metrics endpoint
EXPOSE 9090
# WebSocket
EXPOSE 8080

CMD ["node", "server.js"]
```

```bash
# Run with all ports mapped
docker run -d \
  --name full-stack-app \
  -p 3000:3000 \
  -p 4000:4000 \
  -p 9090:9090 \
  -p 8080:8080 \
  my-full-stack-app
```

**Port Mapping Troubleshooting:**

```bash
# Error: Port already in use
# Check what's using the port
netstat -tuln | grep 8080
lsof -i :8080

# Kill process using port (Linux/Mac)
kill -9 $(lsof -t -i:8080)

# Windows
netstat -ano | findstr :8080
taskkill /PID <PID> /F

# Use different host port
docker run -d -p 8081:80 nginx  # Use 8081 instead
```

---

## Chapter 11: Pushing Custom Images

### 11.1 Tagging Custom Images

**Apne images ko properly tag karo:**

**Tagging Conventions:**

```bash
# Basic format
[REGISTRY/]REPOSITORY[:TAG]

# Docker Hub (default registry)
username/myapp:v1.0

# Private registry
myregistry.com:5000/myapp:v1.0

# Cloud registries
gcr.io/project-id/myapp:v1.0
123456.dkr.ecr.us-east-1.amazonaws.com/myapp:v1.0
```

**Tag After Building:**

```bash
# Build image
docker build -t myapp .

# Tag for Docker Hub
docker tag myapp username/myapp:latest
docker tag myapp username/myapp:v1.0.0
docker tag myapp username/myapp:stable

# Tag for different environments
docker tag myapp username/myapp:dev
docker tag myapp username/myapp:staging
docker tag myapp username/myapp:production
```

**Tag During Build:**

```bash
# Tag while building
docker build -t username/myapp:v1.0.0 .
docker build -t username/myapp:latest -t username/myapp:v1.0.0 .
```

**Semantic Versioning Strategy:**

```bash
# Build new version
docker build -t myapp .

# Tag with semantic version
docker tag myapp username/myapp:2.1.0
docker tag myapp username/myapp:2.1
docker tag myapp username/myapp:2
docker tag myapp username/myapp:latest

# Now you have:
# username/myapp:2.1.0   (specific patch)
# username/myapp:2.1     (minor version)
# username/myapp:2       (major version)
# username/myapp:latest  (latest stable)
```

---

### 11.2 Logging into Docker Hub

**Docker Hub me login karo:**

**Command Line Login:**

```bash
# Interactive login
docker login
# Enter username
# Enter password
# Login Succeeded

# Login with username
docker login -u username

# Login with password (not recommended)
docker login -u username -p password

# Login to specific registry
docker login myregistry.com
```

**Using Access Tokens (Recommended):**

```bash
# Create access token on Docker Hub:
# 1. Go to hub.docker.com
# 2. Account Settings → Security → New Access Token
# 3. Copy the token

# Login with token
docker login -u username -p YOUR_ACCESS_TOKEN

# Or use stdin for security
echo "YOUR_ACCESS_TOKEN" | docker login -u username --password-stdin
```

**Store Credentials Securely:**

```bash
# Credentials stored in:
# Linux: ~/.docker/config.json
# macOS: ~/.docker/config.json
# Windows: %USERPROFILE%\.docker\config.json

# Use credential helper (more secure)
# Install docker-credential-helpers
# Configure in ~/.docker/config.json:
{
  "credsStore": "osxkeychain"  // macOS
  "credsStore": "wincred"       // Windows
  "credsStore": "pass"          // Linux
}
```

**Logout:**

```bash
# Logout from Docker Hub
docker logout

# Logout from specific registry
docker logout myregistry.com
```

---

### 11.3 Pushing Images

**Images ko registry me push karo:**

**Push to Docker Hub:**

```bash
# 1. Login
docker login

# 2. Tag image
docker tag myapp username/myapp:v1.0

# 3. Push
docker push username/myapp:v1.0

# Push multiple tags
docker push username/myapp:v1.0
docker push username/myapp:latest
```

**Push All Tags:**

```bash
# Push all tags of a repository
docker push username/myapp --all-tags
```

**Complete Workflow:**

```bash
# Build application
docker build -t myapp .

# Tag with multiple versions
docker tag myapp yourusername/myapp:1.2.0
docker tag myapp yourusername/myapp:1.2
docker tag myapp yourusername/myapp:1
docker tag myapp yourusername/myapp:latest

# Login to Docker Hub
docker login

# Push all versions
docker push yourusername/myapp:1.2.0
docker push yourusername/myapp:1.2
docker push yourusername/myapp:1
docker push yourusername/myapp:latest

# Or push all at once
docker push yourusername/myapp --all-tags
```

**Monitor Push Progress:**

```bash
docker push username/myapp:latest

# Output shows layers being pushed:
The push refers to repository [docker.io/username/myapp]
5f70bf18a086: Pushed
d5faef5cdfa7: Pushed
1.0: digest: sha256:abc123... size: 1234
```

**Verify Push:**

```bash
# Check on Docker Hub
# Visit: https://hub.docker.com/r/username/myapp

# Or pull to verify
docker pull username/myapp:latest
```

---

### 11.4 Versioning Images

**Proper versioning strategy:**

**Semantic Versioning (MAJOR.MINOR.PATCH):**

```bash
# Version 1.0.0
docker build -t username/myapp:1.0.0 .
docker tag username/myapp:1.0.0 username/myapp:1.0
docker tag username/myapp:1.0.0 username/myapp:1
docker tag username/myapp:1.0.0 username/myapp:latest

# Version 1.0.1 (patch - bug fix)
docker build -t username/myapp:1.0.1 .
docker tag username/myapp:1.0.1 username/myapp:1.0
docker tag username/myapp:1.0.1 username/myapp:1
docker tag username/myapp:1.0.1 username/myapp:latest

# Version 1.1.0 (minor - new feature)
docker build -t username/myapp:1.1.0 .
docker tag username/myapp:1.1.0 username/myapp:1.1
docker tag username/myapp:1.1.0 username/myapp:1
docker tag username/myapp:1.1.0 username/myapp:latest

# Version 2.0.0 (major - breaking changes)
docker build -t username/myapp:2.0.0 .
docker tag username/myapp:2.0.0 username/myapp:2.0
docker tag username/myapp:2.0.0 username/myapp:2
docker tag username/myapp:2.0.0 username/myapp:latest
```

**Environment-Based Tagging:**

```bash
# Development
docker build -t username/myapp:dev .
docker build -t username/myapp:dev-$(date +%Y%m%d) .

# Staging
docker build -t username/myapp:staging .
docker build -t username/myapp:staging-v1.2 .

# Production
docker build -t username/myapp:prod .
docker build -t username/myapp:prod-v1.2.0 .
```

**Git-Based Versioning:**

```bash
# Use git commit hash
GIT_HASH=$(git rev-parse --short HEAD)
docker build -t username/myapp:$GIT_HASH .
docker tag username/myapp:$GIT_HASH username/myapp:latest

# Use git tag
GIT_TAG=$(git describe --tags --abbrev=0)
docker build -t username/myapp:$GIT_TAG .

# Use branch name
GIT_BRANCH=$(git rev-parse --abbrev-ref HEAD)
docker build -t username/myapp:$GIT_BRANCH .
```

**Automated Versioning Script:**

```bash
#!/bin/bash
# build-and-push.sh

# Get version from package.json or similar
VERSION=$(cat VERSION)
GIT_HASH=$(git rev-parse --short HEAD)
DATE=$(date +%Y%m%d)

IMAGE_NAME="username/myapp"

echo "Building version $VERSION..."

# Build image
docker build -t $IMAGE_NAME:$VERSION .

# Tag with multiple versions
docker tag $IMAGE_NAME:$VERSION $IMAGE_NAME:latest
docker tag $IMAGE_NAME:$VERSION $IMAGE_NAME:$VERSION-$GIT_HASH
docker tag $IMAGE_NAME:$VERSION $IMAGE_NAME:$VERSION-$DATE

# Push all tags
echo "Pushing to Docker Hub..."
docker push $IMAGE_NAME:$VERSION
docker push $IMAGE_NAME:latest
docker push $IMAGE_NAME:$VERSION-$GIT_HASH
docker push $IMAGE_NAME:$VERSION-$DATE

echo "✅ Done! Pushed version $VERSION"
```

**Best Practices:**

```bash
# ✅ Good
username/myapp:1.2.3           # Specific version
username/myapp:1.2             # Minor version
username/myapp:1               # Major version
username/myapp:latest          # Latest stable
username/myapp:stable          # Current stable
username/myapp:dev             # Development

# ❌ Avoid
username/myapp:test            # Too vague
username/myapp:new             # Not descriptive
username/myapp:final           # Nothing is final
username/myapp:prod            # Use version numbers
```

---

## Chapter 12: Docker Networking

### 12.1 Docker Networking Basics

**Docker networking samjho:**

**Why Networking?**

- Containers need to communicate
- Isolate different applications
- Connect containers to external networks
- Service discovery

**Network Components:**

```
┌─────────────────────────────────────┐
│         Host Machine                │
│                                     │
│  ┌──────────────────────────────┐  │
│  │    Docker Network (bridge)    │  │
│  │                               │  │
│  │  ┌──────┐  ┌──────┐  ┌─────┐│  │
│  │  │ Web  │  │ API  │  │ DB  ││  │
│  │  │Container│Container│Container││
│  │  └──────┘  └──────┘  └─────┘│  │
│  └──────────────────────────────┘  │
│                                     │
└─────────────────────────────────────┘
```

**Basic Commands:**

```bash
# List networks
docker network ls

# Inspect network
docker network inspect bridge

# Create network
docker network create my-network

# Remove network
docker network rm my-network

# Connect container to network
docker network connect my-network container-name

# Disconnect container from network
docker network disconnect my-network container-name
```

---

### 12.2 Network Drivers Overview

**Different types of network drivers:**

| Driver | Use Case | Scope |
|--------|----------|-------|
| **bridge** | Default, single host | Local |
| **host** | Remove network isolation | Local |
| **overlay** | Multi-host, Swarm | Global |
| **macvlan** | Physical network connection | Local |
| **ipvlan** | Control over IPv4/IPv6 | Local |
| **none** | Disable networking | Local |

**List Available Drivers:**

```bash
docker network ls

# Output:
NETWORK ID     NAME      DRIVER    SCOPE
abc123         bridge    bridge    local
def456         host      host      local
ghi789         none      none      local
```

---

### 12.3 Bridge Mode Networking (Default)

**Bridge network - Default mode:**

**What is Bridge Mode?**

- Default network driver
- Private internal network on host
- Containers can communicate with each other
- Isolated from host network

**Default Bridge Network:**

```bash
# Containers automatically connect to default bridge
docker run -d --name web nginx
docker run -d --name api node-app

# They can communicate using IP addresses
# But NOT using container names (no DNS)
```

**Limitations of Default Bridge:**

- No automatic DNS resolution
- Must use IP addresses
- Less secure

**Inspect Default Bridge:**

```bash
docker network inspect bridge

# Shows connected containers and their IPs
```

---

### 12.4 Host Mode Networking

**Host network - Direct host access:**

**What is Host Mode?**

- Container shares host's network
- No network isolation
- Container uses host's IP
- Better performance (no NAT overhead)

**Use Cases:**

- High-performance applications
- Network monitoring tools
- When you need host network access

**Example:**

```bash
# Run with host network
docker run -d --network host nginx

# Container uses host's ports directly
# No need for -p flag
# Access via host IP: http://host-ip:80
```

**Limitations:**

- No port isolation
- Can't run multiple containers on same port
- Less secure
- Not available on Docker Desktop (Mac/Windows)

**When to Use:**

```bash
# ✅ Good use cases
# - Network monitoring
docker run -d --network host monitoring-tool

# - High-performance database
docker run -d --network host redis

# ❌ Not recommended
# - Web applications (use bridge)
# - Multiple services on same port
```

---

### 12.5 Overlay Mode Networking

**Overlay network - Multi-host:**

**What is Overlay?**

- Connects multiple Docker hosts
- Used in Docker Swarm
- Containers on different hosts can communicate
- Encrypted by default

**Requirements:**

- Docker Swarm mode
- Multiple Docker hosts
- Open ports: 2377, 7946, 4789

**Create Overlay Network:**

```bash
# Initialize Swarm
docker swarm init

# Create overlay network
docker network create \
  --driver overlay \
  --attachable \
  my-overlay-network

# Deploy service on overlay network
docker service create \
  --name web \
  --network my-overlay-network \
  --replicas 3 \
  nginx
```

**Use Case - Multi-host Application:**

```bash
# Node 1 (Manager)
docker swarm init
docker network create --driver overlay app-network

# Node 2 (Worker)
docker swarm join --token <token> <manager-ip>:2377

# Deploy services
docker service create --name db --network app-network postgres
docker service create --name api --network app-network api-app
docker service create --name web --network app-network nginx
```

---

### 12.6 ipvlan and MacVlan Mode Networking

**Advanced networking modes:**

**MacVlan - Physical Network:**

```bash
# Create macvlan network
docker network create -d macvlan \
  --subnet=192.168.1.0/24 \
  --gateway=192.168.1.1 \
  -o parent=eth0 \
  my-macvlan

# Run container with own MAC address
docker run -d \
  --network my-macvlan \
  --ip 192.168.1.100 \
  nginx
```

**IPVlan - IP Control:**

```bash
# Create ipvlan network
docker network create -d ipvlan \
  --subnet=192.168.1.0/24 \
  --gateway=192.168.1.1 \
  -o parent=eth0 \
  my-ipvlan

# Run container
docker run -d \
  --network my-ipvlan \
  --ip 192.168.1.101 \
  nginx
```

**Use Cases:**

- Legacy applications expecting physical network
- Network monitoring
- DHCP servers
- IoT devices

---

### 12.7 None Mode Networking

**Disable networking completely:**

```bash
# Run container with no network
docker run -d --network none alpine sleep 1000

# Container has:
# - No external connectivity
# - Only loopback interface
# - Completely isolated
```

**Use Cases:**

- Maximum security
- Batch processing
- Testing
- Isolated computations

---

### 12.8 Custom Bridge Networks

**Create your own networks - Best practice!**

**Why Custom Bridge?**

- Automatic DNS resolution
- Better isolation
- Easy container discovery
- More secure

**Create Custom Network:**

```bash
# Create network
docker network create my-app-network

# Run containers on network
docker run -d --name db --network my-app-network postgres
docker run -d --name api --network my-app-network api-app
docker run -d --name web --network my-app-network nginx

# Containers can communicate using names!
# api can connect to: postgres://db:5432
# web can connect to: http://api:8080
```

**Network with Options:**

```bash
# Create network with custom subnet
docker network create \
  --driver bridge \
  --subnet 172.25.0.0/16 \
  --gateway 172.25.0.1 \
  --ip-range 172.25.1.0/24 \
  my-custom-network

# Run container with specific IP
docker run -d \
  --name web \
  --network my-custom-network \
  --ip 172.25.1.10 \
  nginx
```

**Network Labels:**

```bash
# Create network with labels
docker network create \
  --label environment=production \
  --label team=backend \
  prod-network
```

---

### 12.9 Container Communication

**Containers ko connect karo:**

**Same Network Communication:**

```bash
# Create network
docker network create app-network

# Run database
docker run -d \
  --name postgres-db \
  --network app-network \
  -e POSTGRES_PASSWORD=secret \
  postgres:14

# Run API (connects to database using hostname)
docker run -d \
  --name api \
  --network app-network \
  -e DB_HOST=postgres-db \
  -e DB_PORT=5432 \
  my-api-app

# Run frontend (connects to API)
docker run -d \
  --name frontend \
  --network app-network \
  -e API_URL=http://api:8080 \
  -p 80:3000 \
  my-frontend-app
```

**Connect to Multiple Networks:**

```bash
# Create networks
docker network create frontend-network
docker network create backend-network

# Database only on backend
docker run -d \
  --name db \
  --network backend-network \
  postgres

# API on both networks
docker run -d \
  --name api \
  --network backend-network \
  my-api-app

docker network connect frontend-network api

# Frontend only on frontend network
docker run -d \
  --name web \
  --network frontend-network \
  -p 80:80 \
  nginx
```

**Testing Container Communication:**

```bash
# Create network and containers
docker network create test-network
docker run -d --name container1 --network test-network alpine sleep 1000
docker run -d --name container2 --network test-network alpine sleep 1000

# Test communication from container1 to container2
docker exec container1 ping container2
# Should work! DNS resolves container2's name

# Test from container2 to container1
docker exec container2 ping container1
# Works both ways!
```

**Real-world Multi-tier Application:**

```bash
#!/bin/bash
# setup-app-network.sh

echo "🌐 Setting up application network..."

# Create networks
docker network create frontend-net
docker network create backend-net

echo "🗄️  Starting database..."
docker run -d \
  --name postgres-db \
  --network backend-net \
  -e POSTGRES_PASSWORD=secret123 \
  -e POSTGRES_DB=myapp \
  -v pgdata:/var/lib/postgresql/data \
  postgres:14

echo "📦 Starting Redis cache..."
docker run -d \
  --name redis-cache \
  --network backend-net \
  redis:alpine

echo "🚀 Starting API server..."
docker run -d \
  --name api-server \
  --network backend-net \
  -e DB_HOST=postgres-db \
  -e REDIS_HOST=redis-cache \
  myapp:api

# Connect API to frontend network too
docker network connect frontend-net api-server

echo "🌐 Starting web server..."
docker run -d \
  --name web-server \
  --network frontend-net \
  -p 80:80 \
  -e API_URL=http://api-server:8080 \
  myapp:frontend

echo "✅ Application stack is running!"
echo "Frontend: http://localhost"
docker ps
```

**Network Troubleshooting:**

```bash
# Check container's network
docker inspect container-name | grep -A 20 Networks

# Check network details
docker network inspect network-name

# Test connectivity
docker exec container1 ping -c 3 container2
docker exec container1 wget -O- http://container2:8080/health
docker exec container1 curl http://container2:8080

# Check DNS resolution
docker exec container1 nslookup container2
docker exec container1 cat /etc/hosts

# View network traffic
docker exec container1 netstat -tuln
```

**Network Aliases:**

```bash
# Create container with network alias
docker run -d \
  --name db1 \
  --network my-network \
  --network-alias database \
  postgres

docker run -d \
  --name db2 \
  --network my-network \
  --network-alias database \
  postgres

# Both accessible via 'database' hostname
# Load balanced automatically!
docker exec api ping database
```

**Port Publishing vs Network:**

```bash
# Port publishing (-p) - Host to container
docker run -d -p 8080:80 nginx
# Access from host: localhost:8080

# Network - Container to container
docker network create app-net
docker run -d --name web --network app-net nginx
docker run -d --name api --network app-net myapp
# API can access: http://web:80
# But host cannot access without -p
```

---

## Chapter 13: Docker Volumes

### 13.1 Understanding Docker Volumes

**Volume kya hai?**
Volumes are the preferred way to persist data in Docker containers. Container delete hone ke baad bhi data safe rahta hai.

**Why Volumes?**

- Data persistence
- Share data between containers
- Backup and restore
- Better performance than bind mounts
- Host-independent

**Volume vs Container Filesystem:**

```
Container Filesystem (Ephemeral):
Container Created → Data Stored → Container Deleted → Data Lost ❌

With Volume (Persistent):
Container Created → Data in Volume → Container Deleted → Data Safe ✅
```

**Types of Data Storage:**

1. **Volumes** - Managed by Docker (Best)
2. **Bind Mounts** - Direct host directory
3. **tmpfs** - Memory only (temporary)

---

### 13.2 Types of Volumes

**Three main types:**

**1. Named Volumes (Recommended):**

```bash
# Create named volume
docker volume create my-data

# Use in container
docker run -d \
  --name app \
  -v my-data:/app/data \
  myapp

# Managed by Docker in: /var/lib/docker/volumes/
```

**2. Anonymous Volumes:**

```bash
# Docker creates random name
docker run -d -v /app/data myapp

# List shows random name
docker volume ls
# DRIVER    VOLUME NAME
# local     abc123def456...
```

**3. Bind Mounts:**

```bash
# Mount host directory
docker run -d \
  -v /host/path:/container/path \
  myapp

# Or use --mount (more explicit)
docker run -d \
  --mount type=bind,source=/host/path,target=/container/path \
  myapp
```

**Comparison:**

| Type | Management | Use Case | Path |
|------|------------|----------|------|
| **Named Volume** | Docker | Production, data persistence | Docker managed |
| **Anonymous Volume** | Docker | Temporary data | Docker managed |
| **Bind Mount** | User | Development, config files | User specified |

---

### 13.3 Attaching Host Volumes (Bind Mounts)

**Host directory ko mount karo:**

**Basic Bind Mount:**

```bash
# Mount current directory
docker run -d \
  -v $(pwd):/app \
  myapp

# Mount with read-only
docker run -d \
  -v $(pwd):/app:ro \
  myapp

# Mount specific directory
docker run -d \
  -v /home/user/data:/app/data \
  myapp
```

**Development Workflow:**

```bash
# Node.js development with live reload
docker run -d \
  --name node-dev \
  -v $(pwd)/src:/app/src \
  -v $(pwd)/package.json:/app/package.json \
  -p 3000:3000 \
  node:18 \
  npm run dev

# Changes in ./src reflect immediately!
```

**Using --mount (Clearer Syntax):**

```bash
# Bind mount with --mount
docker run -d \
  --mount type=bind,source=$(pwd),target=/app \
  myapp

# Read-only bind mount
docker run -d \
  --mount type=bind,source=$(pwd),target=/app,readonly \
  myapp

# Bind mount with specific options
docker run -d \
  --mount type=bind,source=$(pwd),target=/app,consistency=cached \
  myapp
```

**Multiple Bind Mounts:**

```bash
# Mount multiple directories
docker run -d \
  --name web-app \
  -v $(pwd)/src:/app/src \
  -v $(pwd)/public:/app/public \
  -v $(pwd)/config:/app/config:ro \
  -p 3000:3000 \
  myapp
```

**Real-world Development Setup:**

```bash
# Full-stack development
docker run -d \
  --name dev-frontend \
  -v $(pwd)/frontend/src:/app/src \
  -v $(pwd)/frontend/public:/app/public \
  -v /app/node_modules \
  -p 3000:3000 \
  node:18 \
  npm start

# Note: -v /app/node_modules prevents overwriting
# This keeps node_modules from container, not host
```

**Windows Path Syntax:**

```bash
# Windows (PowerShell)
docker run -d -v ${PWD}:/app myapp

# Windows (CMD)
docker run -d -v %cd%:/app myapp

# Windows (Git Bash)
docker run -d -v $(pwd):/app myapp

# Windows (Absolute path)
docker run -d -v C:/Users/username/project:/app myapp
```

---

### 13.4 Creating and Managing Custom Volumes

**Named volumes create aur manage karo:**

**Create Volume:**

```bash
# Create volume
docker volume create my-volume

# Create with driver options
docker volume create \
  --driver local \
  --opt type=none \
  --opt device=/path/on/host \
  --opt o=bind \
  my-volume

# Create with labels
docker volume create \
  --label environment=production \
  --label team=backend \
  prod-data
```

**Use Volume:**

```bash
# Use in container
docker run -d \
  --name app \
  -v my-volume:/app/data \
  myapp

# Multiple containers can share same volume
docker run -d --name app1 -v shared-data:/data myapp
docker run -d --name app2 -v shared-data:/data myapp
# Both access same data!
```

**Volume with Database:**

```bash
# PostgreSQL with persistent data
docker run -d \
  --name postgres-db \
  -v pgdata:/var/lib/postgresql/data \
  -e POSTGRES_PASSWORD=secret \
  postgres:14

# Data persists even if container is removed
docker rm -f postgres-db
docker run -d \
  --name postgres-db-new \
  -v pgdata:/var/lib/postgresql/data \
  -e POSTGRES_PASSWORD=secret \
  postgres:14
# Same data available!
```

**MongoDB Example:**

```bash
# Create volume for MongoDB
docker volume create mongo-data

# Run MongoDB with volume
docker run -d \
  --name mongodb \
  -v mongo-data:/data/db \
  -p 27017:27017 \
  -e MONGO_INITDB_ROOT_USERNAME=admin \
  -e MONGO_INITDB_ROOT_PASSWORD=secret \
  mongo:6

# Data persists across container restarts
```

**MySQL Example:**

```bash
# Create MySQL with persistent data
docker volume create mysql-data

docker run -d \
  --name mysql-db \
  -v mysql-data:/var/lib/mysql \
  -e MYSQL_ROOT_PASSWORD=rootpass \
  -e MYSQL_DATABASE=myapp \
  -e MYSQL_USER=user \
  -e MYSQL_PASSWORD=pass \
  -p 3306:3306 \
  mysql:8
```

---

### 13.5 Volume Commands

**Volume management commands:**

**List Volumes:**

```bash
# List all volumes
docker volume ls

# Filter volumes
docker volume ls --filter dangling=true
docker volume ls --filter label=environment=production
docker volume ls --filter driver=local
```

**Inspect Volume:**

```bash
# Detailed information
docker volume inspect my-volume

# Output (JSON):
[
    {
        "CreatedAt": "2024-01-15T10:30:00Z",
        "Driver": "local",
        "Labels": {},
        "Mountpoint": "/var/lib/docker/volumes/my-volume/_data",
        "Name": "my-volume",
        "Options": {},
        "Scope": "local"
    }
]

# Get mountpoint
docker volume inspect --format '{{.Mountpoint}}' my-volume
```

**Remove Volume:**

```bash
# Remove single volume
docker volume rm my-volume

# Remove multiple volumes
docker volume rm vol1 vol2 vol3

# Remove all unused volumes
docker volume prune

# Force prune
docker volume prune -f

# Prune with filter
docker volume prune --filter label=temporary=true
```

**Volume Usage:**

```bash
# Check which containers use a volume
docker ps -a --filter volume=my-volume

# Check volume size
docker system df -v

# Get volume details from container
docker inspect container-name | grep -A 10 Mounts
```

**Copy Data to/from Volume:**

```bash
# Copy data to volume using a temporary container
docker run --rm \
  -v my-volume:/data \
  -v $(pwd):/backup \
  alpine \
  cp -r /backup/* /data/

# Copy data from volume
docker run --rm \
  -v my-volume:/data \
  -v $(pwd):/backup \
  alpine \
  cp -r /data/* /backup/
```

---

### 13.6 Backup and Restore Volumes

**Volume ka backup aur restore:**

**Backup Volume:**

```bash
# Backup volume to tar file
docker run --rm \
  -v my-volume:/data \
  -v $(pwd):/backup \
  alpine \
  tar czf /backup/backup.tar.gz -C /data .

# Verify backup
ls -lh backup.tar.gz
```

**Restore Volume:**

```bash
# Create new volume
docker volume create my-restored-volume

# Restore from backup
docker run --rm \
  -v my-restored-volume:/data \
  -v $(pwd):/backup \
  alpine \
  tar xzf /backup/backup.tar.gz -C /data
```

**Database Backup Script:**

```bash
#!/bin/bash
# backup-postgres.sh

VOLUME_NAME="pgdata"
BACKUP_DIR="./backups"
DATE=$(date +%Y%m%d_%H%M%S)
BACKUP_FILE="$BACKUP_DIR/postgres_backup_$DATE.tar.gz"

mkdir -p $BACKUP_DIR

echo "🗄️  Backing up PostgreSQL volume: $VOLUME_NAME"

docker run --rm \
  -v $VOLUME_NAME:/data \
  -v $(pwd)/$BACKUP_DIR:/backup \
  alpine \
  tar czf /backup/postgres_backup_$DATE.tar.gz -C /data .

echo "✅ Backup completed: $BACKUP_FILE"
ls -lh $BACKUP_FILE
```

**Automated Backup with Cron:**

```bash
# Add to crontab
# Daily backup at 2 AM
0 2 * * * /path/to/backup-volumes.sh

# backup-volumes.sh
#!/bin/bash
BACKUP_DIR="/backups/docker-volumes"
DATE=$(date +%Y%m%d)

mkdir -p $BACKUP_DIR

# Backup all important volumes
for VOLUME in pgdata mongo-data redis-data; do
    docker run --rm \
      -v $VOLUME:/data \
      -v $BACKUP_DIR:/backup \
      alpine \
      tar czf /backup/${VOLUME}_${DATE}.tar.gz -C /data .
done

# Keep only last 7 days
find $BACKUP_DIR -name "*.tar.gz" -mtime +7 -delete

echo "Backup completed: $(date)"
```

**Restore Script:**

```bash
#!/bin/bash
# restore-postgres.sh

if [ -z "$1" ]; then
    echo "Usage: $0 <backup-file>"
    exit 1
fi

BACKUP_FILE=$1
VOLUME_NAME="pgdata-restored"

echo "🔄 Creating volume: $VOLUME_NAME"
docker volume create $VOLUME_NAME

echo "📦 Restoring from: $BACKUP_FILE"
docker run --rm \
  -v $VOLUME_NAME:/data \
  -v $(pwd):/backup \
  alpine \
  tar xzf /backup/$BACKUP_FILE -C /data

echo "✅ Restore completed!"
echo "Start container with: docker run -v $VOLUME_NAME:/var/lib/postgresql/data postgres:14"
```

**Volume Migration:**

```bash
# Migrate volume between hosts

# Host 1: Export volume
docker run --rm \
  -v source-volume:/data \
  alpine \
  tar cz -C /data . > volume-backup.tar.gz

# Transfer file to Host 2
scp volume-backup.tar.gz user@host2:/path/

# Host 2: Import volume
docker volume create target-volume

cat volume-backup.tar.gz | docker run --rm -i \
  -v target-volume:/data \
  alpine \
  tar xz -C /data
```

---

## Chapter 14: Docker Compose

### 14.1 What is Docker Compose?

**Docker Compose kya hai?**
Docker Compose ek tool hai jo multi-container applications ko define aur run karne ke liye use hota hai. YAML file me puri application define karo, ek command se sab kuch start karo!

**Why Docker Compose?**

- Define entire application in one file
- Start all services with single command
- Manage complex multi-container apps easily
- Version control your infrastructure
- Reproducible environments

**Without Compose vs With Compose:**

```bash
# ❌ Without Compose (manual)
docker network create myapp-net
docker volume create pgdata
docker run -d --name db --network myapp-net -v pgdata:/var/lib/postgresql/data postgres
docker run -d --name redis --network myapp-net redis
docker run -d --name api --network myapp-net -p 8080:8080 myapi
docker run -d --name web --network myapp-net -p 80:80 myweb

# ✅ With Compose (easy!)
docker compose up -d
```

---

### 14.2 Installing Docker Compose

**Docker Compose install karo:**

**Check if Already Installed:**

```bash
docker compose version
# Output: Docker Compose version v2.20.2
```

**Linux Installation:**

```bash
# Docker Compose v2 (Plugin)
# Usually comes with Docker Desktop

# If not installed:
sudo apt-get update
sudo apt-get install docker-compose-plugin

# Verify
docker compose version
```

**Standalone Installation (if needed):**

```bash
# Download binary
sudo curl -L "https://github.com/docker/compose/releases/latest/download/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose

# Make executable
sudo chmod +x /usr/local/bin/docker-compose

# Verify
docker-compose --version
```

**Note:** Modern Docker includes Compose as a plugin. Use `docker compose` instead of `docker-compose`.

---

### 14.3 Docker Compose File Structure

**docker-compose.yml ka structure:**

**Basic Structure:**

```yaml
version: '3.8'  # Compose file version

services:  # Define containers
  service-name:
    image: image-name
    ports:
      - "host:container"
    environment:
      - KEY=value
    volumes:
      - volume-name:/path
    networks:
      - network-name

volumes:  # Define volumes
  volume-name:

networks:  # Define networks
  network-name:
```

**Simple Example:**

```yaml
# docker-compose.yml
version: '3.8'

services:
  web:
    image: nginx:alpine
    ports:
      - "80:80"
    volumes:
      - ./html:/usr/share/nginx/html

  database:
    image: postgres:14
    environment:
      POSTGRES_PASSWORD: secret
    volumes:
      - pgdata:/var/lib/postgresql/data

volumes:
  pgdata:
```

**Start Application:**

```bash
# Start all services
docker compose up -d

# View running services
docker compose ps

# View logs
docker compose logs

# Stop all services
docker compose down
```

---

### 14.4 Docker Compose Commands

**Important Compose commands:**

**Start and Stop:**

```bash
# Start services
docker compose up           # Foreground
docker compose up -d        # Background (detached)

# Start specific service
docker compose up -d web

# Stop services
docker compose stop         # Stop without removing
docker compose down         # Stop and remove containers
docker compose down -v      # Stop and remove volumes too
```

**View and Monitor:**

```bash
# List services
docker compose ps

# List all containers (including stopped)
docker compose ps -a

# View logs
docker compose logs
docker compose logs -f           # Follow logs
docker compose logs -f web       # Specific service
docker compose logs --tail=100   # Last 100 lines
```

**Service Management:**

```bash
# Restart services
docker compose restart
docker compose restart web       # Specific service

# Pause services
docker compose pause
docker compose unpause

# Stop specific service
docker compose stop web
```

**Build and Rebuild:**

```bash
# Build images
docker compose build

# Build without cache
docker compose build --no-cache

# Build specific service
docker compose build web

# Pull latest images
docker compose pull
```

**Execute Commands:**

```bash
# Execute command in running service
docker compose exec web sh
docker compose exec db psql -U postgres

# Run one-off command
docker compose run web npm install
docker compose run --rm web python manage.py migrate
```

**Scale Services:**

```bash
# Scale service to multiple instances
docker compose up -d --scale web=3

# Scale multiple services
docker compose up -d --scale web=3 --scale worker=5
```

**Other Useful Commands:**

```bash
# Validate compose file
docker compose config

# View compose file with variables resolved
docker compose config --services

# List images
docker compose images

# Remove stopped containers
docker compose rm

# Top processes
docker compose top
```

---

### 14.5 Multi-Container Application Example

**Complete full-stack application:**

**Project Structure:**

```
my-fullstack-app/
├── docker-compose.yml
├── frontend/
│   ├── Dockerfile
│   ├── package.json
│   └── src/
├── backend/
│   ├── Dockerfile
│   ├── requirements.txt
│   └── app/
└── nginx/
    └── nginx.conf
```

**docker-compose.yml:**

```yaml
version: '3.8'

services:
  # PostgreSQL Database
  database:
    image: postgres:14-alpine
    container_name: myapp-db
    environment:
      POSTGRES_DB: myapp
      POSTGRES_USER: admin
      POSTGRES_PASSWORD: secret123
    volumes:
      - postgres-data:/var/lib/postgresql/data
    networks:
      - backend
    healthcheck:
      test: ["CMD-SHELL", "pg_isready -U admin"]
      interval: 10s
      timeout: 5s
      retries: 5

  # Redis Cache
  cache:
    image: redis:7-alpine
    container_name: myapp-cache
    command: redis-server --appendonly yes
    volumes:
      - redis-data:/data
    networks:
      - backend
    healthcheck:
      test: ["CMD", "redis-cli", "ping"]
      interval: 10s
      timeout: 3s
      retries: 5

  # Backend API
  api:
    build:
      context: ./backend
      dockerfile: Dockerfile
    container_name: myapp-api
    environment:
      DATABASE_URL: postgresql://admin:secret123@database:5432/myapp
      REDIS_URL: redis://cache:6379
      SECRET_KEY: your-secret-key
    depends_on:
      database:
        condition: service_healthy
      cache:
        condition: service_healthy
    volumes:
      - ./backend:/app
      - /app/node_modules
    networks:
      - frontend
      - backend
    ports:
      - "8080:8080"
    restart: unless-stopped

  # Frontend
  frontend:
    build:
      context: ./frontend
      dockerfile: Dockerfile
    container_name: myapp-frontend
    environment:
      API_URL: http://api:8080
    volumes:
      - ./frontend/src:/app/src
      - /app/node_modules
    networks:
      - frontend
    ports:
      - "3000:3000"
    depends_on:
      - api
    restart: unless-stopped

  # Nginx Reverse Proxy
  nginx:
    image: nginx:alpine
    container_name: myapp-nginx
    volumes:
      - ./nginx/nginx.conf:/etc/nginx/nginx.conf:ro
    ports:
      - "80:80"
    networks:
      - frontend
    depends_on:
      - frontend
      - api
    restart: unless-stopped

volumes:
  postgres-data:
  redis-data:

networks:
  frontend:
  backend:
```

**Backend Dockerfile:**

```dockerfile
# backend/Dockerfile
FROM python:3.11-slim

WORKDIR /app

COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

COPY . .

EXPOSE 8080

CMD ["gunicorn", "--bind", "0.0.0.0:8080", "--workers", "4", "app:app"]
```

**Frontend Dockerfile:**

```dockerfile
# frontend/Dockerfile
FROM node:18-alpine

WORKDIR /app

COPY package*.json ./
RUN npm ci

COPY . .

EXPOSE 3000

CMD ["npm", "start"]
```

**Nginx Configuration:**

```nginx
# nginx/nginx.conf
events {
    worker_connections 1024;
}

http {
    upstream frontend {
        server frontend:3000;
    }

    upstream api {
        server api:8080;
    }

    server {
        listen 80;

        location / {
            proxy_pass http://frontend;
            proxy_set_header Host $host;
            proxy_set_header X-Real-IP $remote_addr;
        }

        location /api {
            proxy_pass http://api;
            proxy_set_header Host $host;
            proxy_set_header X-Real-IP $remote_addr;
        }
    }
}
```

**Start Application:**

```bash
# Build and start
docker compose up -d --build

# View logs
docker compose logs -f

# Check status
docker compose ps

# Access:
# Frontend: http://localhost
# API: http://localhost/api
```

**Development Commands:**

```bash
# Rebuild specific service
docker compose up -d --build api

# View API logs
docker compose logs -f api

# Access database
docker compose exec database psql -U admin -d myapp

# Access Redis
docker compose exec cache redis-cli

# Run migrations
docker compose exec api python manage.py migrate

# Install npm packages
docker compose exec frontend npm install package-name

# Restart service
docker compose restart api

# Stop everything
docker compose down

# Stop and remove volumes (clean start)
docker compose down -v
```

---

### 14.6 Environment Variables in Compose

**Environment variables ka proper use:**

**Method 1: Inline in docker-compose.yml**  

```yaml
version: '3.8'

services:
  web:
    image: nginx:alpine
    environment:
      - NODE_ENV=production
      - PORT=3000
      - DEBUG=false
```

**Method 2: Using .env File (Recommended)**  

```bash
# .env file (in same directory as docker-compose.yml)
NODE_ENV=production
DB_HOST=postgres
DB_PORT=5432
DB_NAME=myapp
DB_USER=admin
DB_PASSWORD=secret123
API_KEY=your-api-key-here
SECRET_KEY=your-secret-key
```

```yaml
# docker-compose.yml
version: '3.8'

services:
  api:
    image: myapi:latest
    environment:
      - NODE_ENV=${NODE_ENV}
      - DB_HOST=${DB_HOST}
      - DB_PORT=${DB_PORT}
      - DB_NAME=${DB_NAME}
      - DB_USER=${DB_USER}
      - DB_PASSWORD=${DB_PASSWORD}
```

**Method 3: External env_file**  

```yaml
version: '3.8'

services:
  web:
    image: myapp:latest
    env_file:
      - ./config/.env.production
      - ./config/.env.local

  api:
    image: myapi:latest
    env_file:
      - ./config/api.env
```

**Multiple Environment Files:**

```bash
# .env.development
NODE_ENV=development
DEBUG=true
LOG_LEVEL=debug
DB_HOST=localhost

# .env.production
NODE_ENV=production
DEBUG=false
LOG_LEVEL=error
DB_HOST=prod-db.example.com
```

```yaml
# docker-compose.yml
version: '3.8'

services:
  app:
    image: myapp:latest
    env_file:
      - .env.${ENV:-development}
    environment:
      - APP_VERSION=1.0.0
```

**Start with specific environment:**

```bash
# Development
ENV=development docker compose up -d

# Production
ENV=production docker compose up -d
```

**Override with Command Line:**

```bash
# Override specific variables
docker compose up -d -e DB_HOST=custom-host -e DB_PORT=3306

# Use different env file
docker compose --env-file .env.staging up -d
```

**Variable Substitution:**

```yaml
version: '3.8'

services:
  web:
    image: nginx:${NGINX_VERSION:-alpine}
    ports:
      - "${WEB_PORT:-80}:80"
    environment:
      - API_URL=http://api:${API_PORT:-8080}
```

**Best Practices:**

```yaml
# ✅ Good - Use defaults
environment:
  - PORT=${PORT:-3000}
  - NODE_ENV=${NODE_ENV:-development}

# ✅ Good - Keep secrets in .env (gitignored)
# .gitignore should include:
# .env
# .env.local
# .env.*.local

# ❌ Bad - Hardcoded secrets
environment:
  - DB_PASSWORD=secret123  # Don't do this!
```

**Complete Example:**

```bash
# .env
POSTGRES_VERSION=14-alpine
POSTGRES_DB=myapp
POSTGRES_USER=admin
POSTGRES_PASSWORD=secret123
API_PORT=8080
FRONTEND_PORT=3000
NGINX_PORT=80
```

```yaml
# docker-compose.yml
version: '3.8'

services:
  database:
    image: postgres:${POSTGRES_VERSION}
    environment:
      - POSTGRES_DB=${POSTGRES_DB}
      - POSTGRES_USER=${POSTGRES_USER}
      - POSTGRES_PASSWORD=${POSTGRES_PASSWORD}
    volumes:
      - pgdata:/var/lib/postgresql/data

  api:
    build: ./backend
    ports:
      - "${API_PORT}:8080"
    environment:
      - DATABASE_URL=postgresql://${POSTGRES_USER}:${POSTGRES_PASSWORD}@database:5432/${POSTGRES_DB}
      - NODE_ENV=production
    depends_on:
      - database

  frontend:
    build: ./frontend
    ports:
      - "${FRONTEND_PORT}:3000"
    environment:
      - REACT_APP_API_URL=http://localhost:${API_PORT}

  nginx:
    image: nginx:alpine
    ports:
      - "${NGINX_PORT}:80"
    depends_on:
      - frontend
      - api

volumes:
  pgdata:
```

---

### 14.7 Depends On and Service Dependencies

**Service dependencies ko manage karo:**

**Basic depends_on:**

```yaml
version: '3.8'

services:
  database:
    image: postgres:14

  api:
    image: myapi:latest
    depends_on:
      - database
    # api starts AFTER database

  frontend:
    image: myfrontend:latest
    depends_on:
      - api
    # frontend starts AFTER api
```

**Startup Order:**

```
1. database starts first
2. api starts after database
3. frontend starts after api
```

**⚠️ Important Note:**
`depends_on` only waits for container to START, not for it to be READY!

**Health Check with depends_on:**

```yaml
version: '3.8'

services:
  database:
    image: postgres:14
    environment:
      POSTGRES_PASSWORD: secret
    healthcheck:
      test: ["CMD-SHELL", "pg_isready -U postgres"]
      interval: 5s
      timeout: 5s
      retries: 5

  api:
    image: myapi:latest
    depends_on:
      database:
        condition: service_healthy
    # api starts AFTER database is healthy!
```

**Health Check Conditions:**

```yaml
depends_on:
  service-name:
    condition: service_started    # Default: just started
    condition: service_healthy    # Wait for health check
    condition: service_completed_successfully  # For one-off tasks
```

**Complex Dependencies:**

```yaml
version: '3.8'

services:
  # Database
  postgres:
    image: postgres:14
    healthcheck:
      test: ["CMD-SHELL", "pg_isready"]
      interval: 10s
      timeout: 5s
      retries: 5

  # Cache
  redis:
    image: redis:alpine
    healthcheck:
      test: ["CMD", "redis-cli", "ping"]
      interval: 10s
      timeout: 3s
      retries: 5

  # Message Queue
  rabbitmq:
    image: rabbitmq:3-management
    healthcheck:
      test: ["CMD", "rabbitmq-diagnostics", "ping"]
      interval: 10s
      timeout: 5s
      retries: 5

  # API depends on all infrastructure
  api:
    build: ./backend
    depends_on:
      postgres:
        condition: service_healthy
      redis:
        condition: service_healthy
      rabbitmq:
        condition: service_healthy
    environment:
      - DB_HOST=postgres
      - REDIS_HOST=redis
      - RABBITMQ_HOST=rabbitmq

  # Worker depends on same infrastructure
  worker:
    build: ./backend
    command: celery worker
    depends_on:
      postgres:
        condition: service_healthy
      redis:
        condition: service_healthy
      rabbitmq:
        condition: service_healthy

  # Frontend depends on API
  frontend:
    build: ./frontend
    depends_on:
      api:
        condition: service_started
    ports:
      - "3000:3000"
```

**Wait-for Scripts (Alternative):**

For services without health checks, use wait-for scripts:

```dockerfile
# Dockerfile
FROM node:18-alpine

# Install wait-for-it
RUN apk add --no-cache bash
ADD https://raw.githubusercontent.com/vishnubob/wait-for-it/master/wait-for-it.sh /wait-for-it.sh
RUN chmod +x /wait-for-it.sh

WORKDIR /app
COPY . .

CMD ["/wait-for-it.sh", "database:5432", "--", "node", "server.js"]
```

```yaml
version: '3.8'

services:
  database:
    image: postgres:14

  api:
    build: ./backend
    command: sh -c '/wait-for-it.sh database:5432 -- node server.js'
    depends_on:
      - database
```

**Custom Wait Script:**

```bash
#!/bin/bash
# wait-for-postgres.sh

set -e

host="$1"
shift
cmd="$@"

until PGPASSWORD=$POSTGRES_PASSWORD psql -h "$host" -U "$POSTGRES_USER" -c '\q'; do
  >&2 echo "Postgres is unavailable - sleeping"
  sleep 1
done

>&2 echo "Postgres is up - executing command"
exec $cmd
```

```yaml
services:
  database:
    image: postgres:14
    environment:
      POSTGRES_PASSWORD: secret

  api:
    build: ./backend
    command: ["./wait-for-postgres.sh", "database", "node", "server.js"]
    depends_on:
      - database
    environment:
      POSTGRES_PASSWORD: secret
      POSTGRES_USER: postgres
```

**Real-world Example with Multiple Dependencies:**

```yaml
version: '3.8'

services:
  # Infrastructure
  postgres:
    image: postgres:14-alpine
    environment:
      POSTGRES_PASSWORD: secret
    healthcheck:
      test: ["CMD-SHELL", "pg_isready -U postgres"]
      interval: 5s
      timeout: 5s
      retries: 5
    volumes:
      - pgdata:/var/lib/postgresql/data

  redis:
    image: redis:7-alpine
    healthcheck:
      test: ["CMD", "redis-cli", "ping"]
      interval: 5s
      timeout: 3s
      retries: 5
    volumes:
      - redis-data:/data

  # Application
  backend:
    build: ./backend
    depends_on:
      postgres:
        condition: service_healthy
      redis:
        condition: service_healthy
    environment:
      DATABASE_URL: postgresql://postgres:secret@postgres:5432/myapp
      REDIS_URL: redis://redis:6379
    ports:
      - "8080:8080"
    restart: unless-stopped

  frontend:
    build: ./frontend
    depends_on:
      backend:
        condition: service_started
    environment:
      API_URL: http://backend:8080
    ports:
      - "3000:3000"
    restart: unless-stopped

  nginx:
    image: nginx:alpine
    depends_on:
      - frontend
      - backend
    volumes:
      - ./nginx.conf:/etc/nginx/nginx.conf:ro
    ports:
      - "80:80"
    restart: unless-stopped

volumes:
  pgdata:
  redis-data:
```

---

### 14.8 Docker Compose Networking

**Networks in Compose:**

**Default Network:**

```yaml
version: '3.8'

services:
  web:
    image: nginx
  
  api:
    image: myapi:latest

  db:
    image: postgres:14

# Docker Compose automatically creates a default network
# All services can communicate using service names
# web can access: http://api:8080
# api can access: postgresql://db:5432
```

**Custom Networks:**

```yaml
version: '3.8'

services:
  frontend:
    image: nginx
    networks:
      - frontend-net

  api:
    image: myapi:latest
    networks:
      - frontend-net
      - backend-net

  database:
    image: postgres:14
    networks:
      - backend-net

  cache:
    image: redis:alpine
    networks:
      - backend-net

networks:
  frontend-net:
  backend-net:

# frontend ↔ api (frontend-net)
# api ↔ database (backend-net)
# api ↔ cache (backend-net)
# frontend CANNOT access database (isolated)
```

**Network Configuration:**

```yaml
version: '3.8'

services:
  web:
    image: nginx
    networks:
      app-network:
        ipv4_address: 172.20.0.10

networks:
  app-network:
    driver: bridge
    ipam:
      driver: default
      config:
        - subnet: 172.20.0.0/16
          gateway: 172.20.0.1
```

**Network Aliases:**

```yaml
version: '3.8'

services:
  api:
    image: myapi:latest
    networks:
      app-net:
        aliases:
          - backend
          - api-server

  # Other services can access via:
  # http://api:8080
  # http://backend:8080
  # http://api-server:8080

networks:
  app-net:
```

**External Networks:**

```yaml
version: '3.8'

services:
  web:
    image: nginx
    networks:
      - existing-network

networks:
  existing-network:
    external: true
    name: my-pre-existing-network
```

**Complete Networking Example:**

```yaml
version: '3.8'

services:
  # Public-facing services
  nginx:
    image: nginx:alpine
    networks:
      - public
    ports:
      - "80:80"
      - "443:443"

  frontend:
    build: ./frontend
    networks:
      - public
      - internal

  # Internal services
  api:
    build: ./backend
    networks:
      - internal
      - database-net
    environment:
      - DB_HOST=postgres

  # Database tier
  postgres:
    image: postgres:14
    networks:
      - database-net
    environment:
      - POSTGRES_PASSWORD=secret

  redis:
    image: redis:alpine
    networks:
      - database-net

networks:
  public:
    driver: bridge
  internal:
    driver: bridge
    internal: true  # No external access
  database-net:
    driver: bridge
    internal: true  # Isolated database network
```

**Network Communication Flow:**

```
Internet
   ↓
nginx (public network)
   ↓
frontend (public + internal)
   ↓
api (internal + database-net)
   ↓
postgres/redis (database-net only)
```

---

### 14.9 Docker Compose Volumes

**Volumes in Compose:**

**Named Volumes:**

```yaml
version: '3.8'

services:
  database:
    image: postgres:14
    volumes:
      - postgres-data:/var/lib/postgresql/data

  redis:
    image: redis:alpine
    volumes:
      - redis-data:/data

volumes:
  postgres-data:
  redis-data:
```

**Volume Configuration:**

```yaml
version: '3.8'

services:
  app:
    image: myapp:latest
    volumes:
      - app-data:/app/data

volumes:
  app-data:
    driver: local
    driver_opts:
      type: none
      o: bind
      device: /path/on/host

  logs:
    driver: local
    driver_opts:
      type: nfs
      o: addr=10.0.0.1,rw
      device: ":/path/on/nfs"
```

**Bind Mounts:**

```yaml
version: '3.8'

services:
  web:
    image: nginx
    volumes:
      - ./html:/usr/share/nginx/html
      - ./nginx.conf:/etc/nginx/nginx.conf:ro

  api:
    build: ./backend
    volumes:
      - ./backend:/app
      - /app/node_modules  # Anonymous volume
      - ./logs:/app/logs
```

**Read-only Volumes:**

```yaml
version: '3.8'

services:
  web:
    image: nginx
    volumes:
      - ./config:/etc/nginx:ro  # Read-only
      - ./html:/usr/share/nginx/html  # Read-write
```

**Volume from another container:**

```yaml
version: '3.8'

services:
  data-container:
    image: alpine
    volumes:
      - shared-data:/data

  app1:
    image: myapp:latest
    volumes_from:
      - data-container

  app2:
    image: myapp:latest
    volumes_from:
      - data-container

volumes:
  shared-data:
```

**Tmpfs Mounts (Memory):**

```yaml
version: '3.8'

services:
  app:
    image: myapp:latest
    tmpfs:
      - /tmp
      - /run

  # Or with options
  cache:
    image: redis:alpine
    tmpfs:
      - type: tmpfs
        target: /cache
        tmpfs:
          size: 1000000000  # 1GB
```

**Complete Volumes Example:**

```yaml
version: '3.8'

services:
  # Database with persistent storage
  postgres:
    image: postgres:14
    volumes:
      - postgres-data:/var/lib/postgresql/data
      - ./init-scripts:/docker-entrypoint-initdb.d:ro
    environment:
      POSTGRES_PASSWORD: secret

  # Application with code and logs
  api:
    build: ./backend
    volumes:
      # Source code (development)
      - ./backend:/app
      # Node modules (don't overwrite)
      - /app/node_modules
      # Logs
      - app-logs:/app/logs
      # Config (read-only)
      - ./config:/app/config:ro
    depends_on:
      - postgres

  # File uploads storage
  storage:
    image: myapp:latest
    volumes:
      - uploads:/app/uploads
      - ./static:/app/static:ro

  # Nginx with config
  nginx:
    image: nginx:alpine
    volumes:
      - ./nginx/nginx.conf:/etc/nginx/nginx.conf:ro
      - ./nginx/ssl:/etc/nginx/ssl:ro
      - nginx-cache:/var/cache/nginx
      - nginx-logs:/var/log/nginx
    ports:
      - "80:80"
      - "443:443"

volumes:
  postgres-data:
    driver: local
  app-logs:
  uploads:
  nginx-cache:
  nginx-logs:
```

**External Volumes:**

```yaml
version: '3.8'

services:
  db:
    image: postgres:14
    volumes:
      - existing-data:/var/lib/postgresql/data

volumes:
  existing-data:
    external: true
    name: my-existing-volume
```

**Volume Labels:**

```yaml
version: '3.8'

volumes:
  postgres-data:
    labels:
      com.example.description: "PostgreSQL database data"
      com.example.department: "backend"
      com.example.environment: "production"
```

---

## Chapter 15: Advanced Topics

### 15.1 Docker Security Best Practices

**Security ko seriously lo!**

**1. Use Official Images:**

```dockerfile
# ✅ Good - Official image
FROM node:18-alpine

# ❌ Bad - Random image
FROM some-random-user/node
```

**2. Don't Run as Root:**

```dockerfile
# Create non-root user
FROM node:18-alpine

RUN addgroup -g 1001 -S nodejs && \
    adduser -S nodejs -u 1001

WORKDIR /app

COPY --chown=nodejs:nodejs . .

USER nodejs

CMD ["node", "server.js"]
```

**3. Scan Images for Vulnerabilities:**

```bash
# Docker Scout (built-in)
docker scout cves myapp:latest

# Trivy scanner
docker run --rm \
  -v /var/run/docker.sock:/var/run/docker.sock \
  aquasec/trivy image myapp:latest

# Snyk
docker scan myapp:latest
```

**4. Use .dockerignore:**

```
# .dockerignore
.git
.env
*.log
node_modules
secrets/
*.key
*.pem
.ssh
```

**5. Minimize Image Layers:**

```dockerfile
# ❌ Bad - Many layers
RUN apt-get update
RUN apt-get install -y python3
RUN apt-get install -y pip
RUN apt-get clean

# ✅ Good - Single layer
RUN apt-get update && \
    apt-get install -y python3 pip && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*
```

**6. Use Multi-stage Builds:**

```dockerfile
# Build stage - has build tools
FROM node:18 AS builder
WORKDIR /app
COPY package*.json ./
RUN npm ci
COPY . .
RUN npm run build

# Runtime stage - minimal
FROM node:18-alpine
WORKDIR /app
COPY --from=builder /app/dist ./dist
COPY --from=builder /app/node_modules ./node_modules
USER node
CMD ["node", "dist/server.js"]
```

**7. Set Resource Limits:**

```yaml
# docker-compose.yml
version: '3.8'

services:
  app:
    image: myapp:latest
    deploy:
      resources:
        limits:
          cpus: '2'
          memory: 1G
        reservations:
          cpus: '1'
          memory: 512M
```

```bash
# Command line
docker run -d \
  --memory="512m" \
  --cpus="1.5" \
  --pids-limit=100 \
  myapp:latest
```

**8. Use Read-only Filesystem:**

```yaml
services:
  app:
    image: myapp:latest
    read_only: true
    tmpfs:
      - /tmp
      - /run
```

**9. Drop Capabilities:**

```yaml
services:
  app:
    image: myapp:latest
    cap_drop:
      - ALL
    cap_add:
      - NET_BIND_SERVICE
```

**10. Use Secrets Management:**

```yaml
# docker-compose.yml
version: '3.8'

services:
  app:
    image: myapp:latest
    secrets:
      - db_password
      - api_key

secrets:
  db_password:
    file: ./secrets/db_password.txt
  api_key:
    external: true
```

**11. Enable Docker Content Trust:**

```bash
# Enable content trust
export DOCKER_CONTENT_TRUST=1

# Only signed images can be pulled/run
docker pull nginx:latest
```

**12. Network Isolation:**

```yaml
version: '3.8'

services:
  frontend:
    networks:
      - public

  api:
    networks:
      - public
      - backend

  database:
    networks:
      - backend

networks:
  public:
  backend:
    internal: true  # No external access
```

**13. Update Regularly:**

```bash
# Pull latest images
docker compose pull

# Rebuild with latest
docker compose build --pull

# Update base images in Dockerfile
FROM node:18-alpine  # Keep updated
```

**Security Checklist:**

```bash
# ✅ Security checklist
[ ] Use official base images
[ ] Run as non-root user
[ ] Scan for vulnerabilities
[ ] Use .dockerignore
[ ] Multi-stage builds
[ ] Set resource limits
[ ] Read-only filesystem where possible
[ ] Drop unnecessary capabilities
[ ] Use secrets for sensitive data
[ ] Keep images updated
[ ] Network isolation
[ ] Enable content trust
[ ] Minimal image size
[ ] No secrets in images
[ ] Health checks configured
```

---

### 15.2 Docker Logging

**Logging best practices:**

**Default Logging:**

```bash
# View logs
docker logs container-name

# Follow logs
docker logs -f container-name

# Last 100 lines
docker logs --tail 100 container-name

# Since timestamp
docker logs --since 2024-01-01T00:00:00 container-name

# With timestamps
docker logs -t container-name
```

**Log Drivers:**

```bash
# JSON file (default)
docker run -d \
  --log-driver json-file \
  --log-opt max-size=10m \
  --log-opt max-file=3 \
  nginx

# Syslog
docker run -d \
  --log-driver syslog \
  --log-opt syslog-address=tcp://192.168.1.100:514 \
  nginx

# Journald (systemd)
docker run -d \
  --log-driver journald \
  nginx

# None (disable logging)
docker run -d --log-driver none nginx
```

**Docker Compose Logging:**

```yaml
version: '3.8'

services:
  web:
    image: nginx
    logging:
      driver: json-file
      options:
        max-size: "10m"
        max-file: "3"
        labels: "production,web"

  api:
    image: myapi:latest
    logging:
      driver: syslog
      options:
        syslog-address: "tcp://192.168.1.100:514"
        tag: "api"

  worker:
    image: worker:latest
    logging:
      driver: none  # No logs for this service
```

**Centralized Logging with ELK Stack:**

```yaml
version: '3.8'

services:
  # Elasticsearch
  elasticsearch:
    image: docker.elastic.co/elasticsearch/elasticsearch:8.10.0
    environment:
      - discovery.type=single-node
      - "ES_JAVA_OPTS=-Xms512m -Xmx512m"
    volumes:
      - es-data:/usr/share/elasticsearch/data
    networks:
      - elk

  # Logstash
  logstash:
    image: docker.elastic.co/logstash/logstash:8.10.0
    volumes:
      - ./logstash/pipeline:/usr/share/logstash/pipeline
    depends_on:
      - elasticsearch
    networks:
      - elk

  # Kibana
  kibana:
    image: docker.elastic.co/kibana/kibana:8.10.0
    ports:
      - "5601:5601"
    depends_on:
      - elasticsearch
    networks:
      - elk

  # Your application
  app:
    image: myapp:latest
    logging:
      driver: json-file
      options:
        max-size: "10m"
    depends_on:
      - logstash
    networks:
      - elk

volumes:
  es-data:

networks:
  elk:
```

**Application-level Logging:**

```javascript
// Node.js with Winston
const winston = require('winston');

const logger = winston.createLogger({
  level: 'info',
  format: winston.format.json(),
  transports: [
    new winston.transports.Console({
      format: winston.format.simple()
    })
  ]
});

logger.info('Application started');
logger.error('Something went wrong', { error: err });
```

```python
# Python with logging
import logging
import sys

logging.basicConfig(
    level=logging.INFO,
    format='%(asctime)s - %(name)s - %(levelname)s - %(message)s',
    handlers=[
        logging.StreamHandler(sys.stdout)
    ]
)

logger = logging.getLogger(__name__)
logger.info('Application started')
logger.error('Something went wrong', exc_info=True)
```

**Log Rotation Script:**

```bash
#!/bin/bash
# rotate-logs.sh

# Find all Docker log files older than 7 days and compress them
find /var/lib/docker/containers -name "*.log" -mtime +7 -exec gzip {} \;

# Remove compressed logs older than 30 days
find /var/lib/docker/containers -name "*.log.gz" -mtime +30 -delete

echo "Log rotation completed: $(date)"
```

---

### 15.3 Health Checks

**Container health monitoring:**

**Dockerfile Health Check:**

```dockerfile
FROM node:18-alpine

WORKDIR /app
COPY . .

EXPOSE 3000

# Health check
HEALTHCHECK --interval=30s --timeout=3s --start-period=5s --retries=3 \
  CMD node healthcheck.js || exit 1

CMD ["node", "server.js"]
```

**healthcheck.js:**

```javascript
// healthcheck.js
const http = require('http');

const options = {
  hostname: 'localhost',
  port: 3000,
  path: '/health',
  method: 'GET',
  timeout: 2000
};

const req = http.request(options, (res) => {
  if (res.statusCode === 200) {
    process.exit(0);
  } else {
    process.exit(1);
  }
});

req.on('error', () => {
  process.exit(1);
});

req.on('timeout', () => {
  req.destroy();
  process.exit(1);
});

req.end();
```

**Docker Compose Health Checks:**

```yaml
version: '3.8'

services:
  database:
    image: postgres:14
    healthcheck:
      test: ["CMD-SHELL", "pg_isready -U postgres"]
      interval: 10s
      timeout: 5s
      retries: 5
      start_period: 10s

  redis:
    image: redis:alpine
    healthcheck:
      test: ["CMD", "redis-cli", "ping"]
      interval: 10s
      timeout: 3s
      retries: 3

  api:
    build: ./backend
    healthcheck:
      test: ["CMD", "curl", "-f", "http://localhost:8080/health"]
      interval: 30s
      timeout: 10s
      retries: 3
      start_period: 40s
    depends_on:
      database:
        condition: service_healthy
      redis:
        condition: service_healthy

  frontend:
    build: ./frontend
    healthcheck:
      test: ["CMD", "wget", "--no-verbose", "--tries=1", "--spider", "http://localhost:3000"]
      interval: 30s
      timeout: 10s
      retries: 3
```

**Health Check Endpoint (Express.js):**

```javascript
// Health check route
app.get('/health', async (req, res) => {
  try {
    // Check database connection
    await db.query('SELECT 1');
    
    // Check Redis connection
    await redis.ping();
    
    res.status(200).json({
      status: 'healthy',
      timestamp: new Date().toISOString(),
      uptime: process.uptime(),
      database: 'connected',
      cache: 'connected'
    });
  } catch (error) {
    res.status(503).json({
      status: 'unhealthy',
      error: error.message
    });
  }
});
```

**Check Container Health:**

```bash
# View health status
docker ps

# Detailed health info
docker inspect --format='{{json .State.Health}}' container-name | jq

# Health status only
docker inspect --format='{{.State.Health.Status}}' container-name
```

**Health Check Commands:**

```yaml
# HTTP endpoint
healthcheck:
  test: ["CMD", "curl", "-f", "http://localhost/health"]

# PostgreSQL
healthcheck:
  test: ["CMD-SHELL", "pg_isready -U ${POSTGRES_USER}"]

# MySQL
healthcheck:
  test: ["CMD", "mysqladmin", "ping", "-h", "localhost"]

# MongoDB
healthcheck:
  test: ["CMD", "mongosh", "--eval", "db.adminCommand('ping')"]

# Redis
healthcheck:
  test: ["CMD", "redis-cli", "ping"]

# Custom script
healthcheck:
  test: ["CMD", "/app/healthcheck.sh"]
```

---

### 15.4 Docker Secrets

**Sensitive data ko securely manage karo:**

**Docker Swarm Secrets:**

```bash
# Initialize Swarm
docker swarm init

# Create secret from file
echo "mysecretpassword" | docker secret create db_password -

# Create from file
docker secret create db_config ./config.json

# List secrets
docker secret ls

# Inspect secret (value not shown)
docker secret inspect db_password
```

**Use Secrets in Service:**

```bash
# Create service with secrets
docker service create \
  --name myapp \
  --secret db_password \
  --secret api_key \
  myapp:latest
```

**Access Secrets in Container:**

```bash
# Secrets mounted at /run/secrets/
cat /run/secrets/db_password
cat /run/secrets/api_key
```

**Docker Compose with Secrets:**

```yaml
version: '3.8'

services:
  database:
    image: postgres:14
    secrets:
      - db_password
    environment:
      POSTGRES_PASSWORD_FILE: /run/secrets/db_password

  api:
    image: myapi:latest
    secrets:
      - db_password
      - api_key
    environment:
      DB_PASSWORD_FILE: /run/secrets/db_password
      API_KEY_FILE: /run/secrets/api_key

secrets:
  db_password:
    file: ./secrets/db_password.txt
  api_key:
    file: ./secrets/api_key.txt
```

**Read Secrets in Application:**

```javascript
// Node.js
const fs = require('fs');

const dbPassword = fs.readFileSync('/run/secrets/db_password', 'utf8').trim();
const apiKey = fs.readFileSync('/run/secrets/api_key', 'utf8').trim();

console.log('Secrets loaded successfully');
```

```python
# Python
def read_secret(secret_name):
    try:
        with open(f'/run/secrets/{secret_name}', 'r') as f:
            return f.read().strip()
    except FileNotFoundError:
        return None

db_password = read_secret('db_password')
api_key = read_secret('api_key')
```

**External Secrets:**

```yaml
version: '3.8'

services:
  app:
    image: myapp:latest
    secrets:
      - production_key

secrets:
  production_key:
    external: true
```

**Environment Variables vs Secrets:**

```yaml
# ❌ Bad - Secrets in env vars
services:
  app:
    environment:
      - DB_PASSWORD=mysecretpassword  # Visible in docker inspect!

# ✅ Good - Use secrets
services:
  app:
    secrets:
      - db_password
    environment:
      - DB_PASSWORD_FILE=/run/secrets/db_password
```

---

### 15.5 Production Deployment Strategies

**Production me deploy karne ke best practices:**

**1. Use Docker Swarm or Kubernetes:**

**Docker Swarm:**

```bash
# Initialize Swarm
docker swarm init

# Add workers
docker swarm join --token <token> <manager-ip>:2377

# Deploy stack
docker stack deploy -c docker-compose.yml myapp

# Scale service
docker service scale myapp_web=5

# Update service
docker service update --image myapp:v2 myapp_web

# Rolling update
docker service update \
  --update-parallelism 2 \
  --update-delay 10s \
  --image myapp:v2 \
  myapp_web
```

**docker-compose.yml for Swarm:**

```yaml
version: '3.8'

services:
  web:
    image: myapp:latest
    deploy:
      replicas: 3
      update_config:
        parallelism: 1
        delay: 10s
        failure_action: rollback
      restart_policy:
        condition: on-failure
        delay: 5s
        max_attempts: 3
      resources:
        limits:
          cpus: '0.5'
          memory: 512M
        reservations:
          cpus: '0.25'
          memory: 256M
    ports:
      - "80:80"
    networks:
      - app-network
    secrets:
      - db_password

  database:
    image: postgres:14
    deploy:
      replicas: 1
      placement:
        constraints:
          - node.role == manager
    volumes:
      - pgdata:/var/lib/postgresql/data
    networks:
      - app-network
    secrets:
      - db_password

secrets:
  db_password:
    external: true

networks:
  app-network:
    driver: overlay

volumes:
  pgdata:
```

**2. CI/CD Pipeline:**

**GitHub Actions Example:**

```yaml
# .github/workflows/deploy.yml
name: Build and Deploy

on:
  push:
    branches: [main]

jobs:
  build:
    runs-on: ubuntu-latest
    
    steps:
      - uses: actions/checkout@v3
      
      - name: Login to Docker Hub
        uses: docker/login-action@v2
        with:
          username: ${{ secrets.DOCKERHUB_USERNAME }}
          password: ${{ secrets.DOCKERHUB_TOKEN }}
      
      - name: Build and push
        uses: docker/build-push-action@v4
        with:
          context: .
          push: true
          tags: |
            username/myapp:latest
            username/myapp:${{ github.sha }}
      
      - name: Deploy to production
        uses: appleboy/ssh-action@master
        with:
          host: ${{ secrets.PROD_HOST }}
          username: ${{ secrets.PROD_USER }}
          key: ${{ secrets.SSH_KEY }}
          script: |
            cd /app
            docker compose pull
            docker compose up -d
            docker system prune -f
```

**3. Blue-Green Deployment:**

```bash
# Current production (blue)
docker compose -f docker-compose.blue.yml up -d

# Deploy new version (green)
docker compose -f docker-compose.green.yml up -d

# Test green environment
curl http://green.example.com/health

# Switch traffic to green
# Update load balancer or DNS

# Remove blue environment
docker compose -f docker-compose.blue.yml down
```

**4. Monitoring and Logging:**

```yaml
version: '3.8'

services:
  # Application
  app:
    image: myapp:latest
    deploy:
      replicas: 3
    logging:
      driver: json-file
      options:
        max-size: "10m"
        max-file: "3"

  # Prometheus monitoring
  prometheus:
    image: prom/prometheus
    volumes:
      - ./prometheus.yml:/etc/prometheus/prometheus.yml
      - prometheus-data:/prometheus
    ports:
      - "9090:9090"

  # Grafana dashboards
  grafana:
    image: grafana/grafana
    ports:
      - "3000:3000"
    volumes:
      - grafana-data:/var/lib/grafana
    environment:
      - GF_SECURITY_ADMIN_PASSWORD=admin

  # Log aggregation
  loki:
    image: grafana/loki
    ports:
      - "3100:3100"
    volumes:
      - loki-data:/loki

volumes:
  prometheus-data:
  grafana-data:
  loki-data:
```

**5. Backup Strategy:**

```bash
#!/bin/bash
# production-backup.sh

BACKUP_DIR="/backups/$(date +%Y%m%d)"
mkdir -p $BACKUP_DIR

echo "🗄️  Backing up databases..."
docker exec postgres pg_dump -U postgres myapp > $BACKUP_DIR/database.sql

echo "📦 Backing up volumes..."
docker run --rm \
  -v pgdata:/data \
  -v $BACKUP_DIR:/backup \
  alpine \
  tar czf /backup/pgdata.tar.gz -C /data .

echo "💾 Backing up configs..."
cp -r /app/config $BACKUP_DIR/

echo "☁️  Uploading to S3..."
aws s3 sync $BACKUP_DIR s3://myapp-backups/$(date +%Y%m%d)/

echo "✅ Backup completed!"
```

**6. Health Monitoring Script:**

```bash
#!/bin/bash
# monitor-production.sh

SERVICES="web api database redis"
WEBHOOK_URL="https://hooks.slack.com/services/YOUR/WEBHOOK/URL"

for SERVICE in $SERVICES; do
    HEALTH=$(docker inspect --format='{{.State.Health.Status}}' $SERVICE 2>/dev/null)
    
    if [ "$HEALTH" != "healthy" ]; then
        MESSAGE="🚨 Alert: Service $SERVICE is $HEALTH"
        curl -X POST -H 'Content-type: application/json' \
            --data "{\"text\":\"$MESSAGE\"}" \
            $WEBHOOK_URL
    fi
done
```

**7. Production Checklist:**

```bash
# ✅ Production deployment checklist

[ ] Use specific image tags (not :latest)
[ ] Configure health checks
[ ] Set resource limits
[ ] Enable auto-restart policies
[ ] Use secrets for sensitive data
[ ] Configure logging
[ ] Set up monitoring
[ ] Configure backups
[ ] Use HTTPS/SSL
[ ] Configure firewall rules
[ ] Set up alerting
[ ] Document rollback procedure
[ ] Test disaster recovery
[ ] Performance testing completed
[ ] Security scan passed
```
