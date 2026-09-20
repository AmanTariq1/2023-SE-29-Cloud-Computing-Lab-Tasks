# ☁️ Cloud Computing Lab Tasks

[![Repo Size](https://img.shields.io/github/repo-size/AmanTariq1/2023-SE-29-Cloud-Computing-Lab-Tasks?style=flat-square)](https://github.com/AmanTariq1/2023-SE-29-Cloud-Computing-Lab-Tasks)
[![Last Commit](https://img.shields.io/github/last-commit/AmanTariq1/2023-SE-29-Cloud-Computing-Lab-Tasks?style=flat-square)](https://github.com/AmanTariq1/2023-SE-29-Cloud-Computing-Lab-Tasks/commits/main)
[![License](https://img.shields.io/github/license/AmanTariq1/2023-SE-29-Cloud-Computing-Lab-Tasks?style=flat-square)](https://github.com/AmanTariq1/2023-SE-29-Cloud-Computing-Lab-Tasks)

> **Cloud Computing (SE-3202)**
> **Department of Software Engineering**
> **The University of Azad Jammu and Kashmir**

---

## 📋 Course & Student Information

| Information         | Details                                     |
| ------------------- | ------------------------------------------- |
| **Student Name**    | Aman Tariq                                  |
| **Roll Number**     | 2023-SE-29                                  |
| **Course**          | Cloud Computing (SE-3202)                   |
| **Instructor**      | Engr. Fahad Nisar                           |
| **Semester**        | Spring 2026                                 |
| **Session**         | 2023–27                                     |
| **University**      | The University of Azad Jammu and Kashmir    |
| **Department**      | Software Engineering                        |
| **GitHub Username** | [AmanTariq1](https://github.com/AmanTariq1) |

---

## 📖 Overview

This repository contains all **8 Cloud Computing laboratory tasks** completed during the **Spring 2026 semester** as part of the **SE-3202 Cloud Computing** course.

The laboratory work covers Linux and WSL setup, SSH authentication and security hardening, cloud deployment, backend hosting, Docker fundamentals, custom Docker images, and multi-container application deployment using Docker Compose.

---

## 📁 Repository Structure

```text
2023-SE-29-Cloud-Computing-Lab-Tasks/
    ├── Lab Task 01 – WSL Ubuntu Installation
    ├── Lab Task 02 – SSH Key-Based Authentication
    ├── Lab Task 03 – SSH Security Hardening
    ├── Lab Task 04 – Static Website Deployment
    ├── Lab Task 05 – Backend Web App Deployment
    ├── Lab Task 06 – Docker Fundamentals
    ├── Lab Task 07 – Dockerfile Custom Image
    └── Lab Task 08 – Docker Compose
    └── README.md
    └── docker-web-app -lab_07.zip
    └── docker-web-app.zip
    └── my-backend-app.zip
    └── my-website.zip
    
```

> **Note:** The `2023-SE-29.zip` archive contains the Word/PDF documentation for all eight laboratory tasks.

---

# 🧪 Lab Tasks Summary

| Task # | Title                        | Description                                                                                     | Technologies                                   |
| ------ | ---------------------------- | ----------------------------------------------------------------------------------------------- | ---------------------------------------------- |
| **01** | WSL Ubuntu Installation      | Installed WSL with Ubuntu, created a Linux user account, and verified the environment.          | WSL, Ubuntu, PowerShell, Linux                 |
| **02** | SSH Key-Based Authentication | Configured SSH key-based authentication between Windows and WSL Ubuntu for passwordless access. | SSH, RSA, OpenSSH, PowerShell, Linux           |
| **03** | Securing SSH                 | Hardened the SSH server by disabling password authentication and direct root login.             | SSH, Linux, Security Hardening                 |
| **04** | Static Website Deployment    | Created and deployed a static HTML/CSS/JS website to a public cloud hosting platform.           | HTML, CSS, JavaScript, Git, GitHub, Netlify    |
| **05** | Backend Web App Deployment   | Developed and deployed a Node.js/Express backend application to a PaaS platform.                | Node.js, Express, Git, GitHub, Vercel          |
| **06** | Docker Fundamentals          | Installed Docker, ran containers, pulled an LLM image, and explored common Docker commands.     | Docker, Docker Desktop, Docker Hub, Containers |
| **07** | Dockerfile Custom Image      | Created a Dockerfile, built a custom Node.js image, launched a container, and inspected it.     | Docker, Dockerfile, Node.js, Containers        |
| **08** | Docker Compose               | Configured and ran a multi-container Node.js and Redis application using Docker Compose.        | Docker, Docker Compose, Node.js, Redis, YAML   |

---

# 🚀 Detailed Lab Tasks

## 🧪 Task 01 — WSL Ubuntu Installation

### Objective

Install **Windows Subsystem for Linux (WSL)** with Ubuntu, create a Linux user account, and verify that the installation is working correctly.

### Key Steps / What Was Done

1. Opened PowerShell with administrative privileges.
2. Installed WSL using the appropriate PowerShell command.
3. Installed and initialized Ubuntu.
4. Created the Linux user:

```text
2023-se-29
```

5. Updated the Ubuntu package repositories and installed available updates.
6. Verified the WSL and Ubuntu environment.

### Technologies Used

* Windows Subsystem for Linux (WSL)
* Ubuntu
* PowerShell
* Linux

---

## 🧪 Task 02 — SSH Key-Based Authentication into WSL Ubuntu

### Objective

Generate an SSH key pair on Windows, configure the public key in WSL Ubuntu, and establish a passwordless SSH connection.

### Key Steps / What Was Done

1. Installed and configured the OpenSSH server inside WSL Ubuntu.
2. Generated an RSA SSH key pair using `ssh-keygen`.
3. Created/configured the SSH `authorized_keys` file.
4. Deployed the public key to the WSL Ubuntu environment.
5. Configured the required permissions.
6. Tested SSH connectivity.
7. Verified passwordless SSH authentication.

### Technologies Used

* SSH
* RSA
* OpenSSH
* PowerShell
* Ubuntu
* Linux

---

## 🧪 Task 03 — Securing SSH

### Objective

Harden the WSL Ubuntu SSH server by disabling password-based authentication and preventing direct root login.

### Key Steps / What Was Done

1. Opened the SSH server configuration file:

```bash
/etc/ssh/sshd_config
```

2. Configured SSH authentication settings.
3. Disabled password authentication:

```text
PasswordAuthentication no
```

4. Enabled public-key authentication:

```text
PubkeyAuthentication yes
```

5. Disabled direct root login:

```text
PermitRootLogin no
```

6. Restarted the SSH service.
7. Used verbose SSH output to verify the authentication configuration:

```bash
ssh -v
```

### Technologies Used

* SSH
* OpenSSH
* Ubuntu
* Linux
* Security Hardening

---

## 🧪 Task 04 — Deploying a Static Website to a Free Hosting Platform

### Objective

Create and deploy a static HTML/CSS/JavaScript website to a free hosting platform and make it publicly accessible through a live URL.

### Key Steps / What Was Done

1. Created the static website files:

```text
index.html
style.css
app.js
```

2. Developed the front-end website using HTML, CSS, and JavaScript.
3. Created a Git repository for the project.
4. Pushed the project to GitHub.
5. Connected the GitHub repository to Netlify.
6. Configured continuous deployment.
7. Deployed the website to a public URL.
8. Verified that the deployed website was accessible online.

### Live URL

🔗 **[View Live Website](https://2023-se-29-static-website.netlify.app)**

### Technologies Used

* HTML
* CSS
* JavaScript
* Git
* GitHub
* Netlify

---

## 🧪 Task 05 — Deploying a Web App with a Backend Server

### Objective

Develop and deploy a web application with a backend server to a free **Platform as a Service (PaaS)** environment.

### Key Steps / What Was Done

1. Created a Node.js backend application.
2. Used Express.js to implement the backend server.
3. Created API routes for the application.
4. Tested the backend locally.
5. Pushed the project source code to GitHub.
6. Configured deployment for Vercel.
7. Created a custom `vercel.json` configuration file.
8. Deployed the backend application.
9. Verified the application through its public URL.

### Live URL

🔗 **[View Live Backend Application](https://2023-se-29-backend-app.vercel.app)**

### Technologies Used

* Node.js
* Express.js
* Git
* GitHub
* Vercel
* REST API

---

## 🧪 Task 06 — Docker Fundamentals: Install, Run, and Explore Containers

### Objective

Install Docker and learn how to create, run, manage, and inspect containers using existing Docker images.

### Key Steps / What Was Done

1. Installed Docker Desktop on Windows.
2. Verified the Docker installation.
3. Ran the `hello-world` container.
4. Pulled the `ai/smollm2` LLM image/model.
5. Explored locally available Docker images.
6. Listed running containers.
7. Listed all containers.
8. Inspected container logs.

### Important Docker Commands

```bash
docker images
docker ps
docker ps -a
docker logs <container-id>
```

### Technologies Used

* Docker
* Docker Desktop
* Docker Hub
* Containers
* Windows

---

## 🧪 Task 07 — Dockerfile: Build, Run, and Inspect a Custom Image

### Objective

Create a custom Docker image for a Node.js application using a Dockerfile, run it as a container, and inspect the resulting image and container.

### Key Steps / What Was Done

1. Created a Node.js application.
2. Created a `Dockerfile`.
3. Configured the Dockerfile using instructions including:

```dockerfile
FROM
WORKDIR
COPY
RUN
EXPOSE
CMD
```

4. Built the custom Docker image with the name:

```text
2023-se-29app
```

5. Ran the container with port mapping:

```text
3000:3000
```

6. Verified the generated image.
7. Verified the running container.
8. Inspected Docker images and containers.

### Important Commands

```bash
docker build -t 2023-se-29app .
docker run -p 3000:3000 2023-se-29app
docker images
docker ps
```

### Technologies Used

* Docker
* Dockerfile
* Node.js
* Containers

---

## 🧪 Task 08 — Multi-Container Apps with Docker Compose

### Objective

Use Docker Compose to run a Node.js application together with a Redis database service using a single configuration and command.

### Key Steps / What Was Done

1. Created a Node.js application.
2. Configured Redis as a database/service.
3. Created a `docker-compose.yml` file.
4. Defined the application and Redis services.
5. Configured service dependency using:

```yaml
depends_on:
```

6. Started the complete application stack in detached mode:

```bash
docker compose up -d
```

7. Verified running services:

```bash
docker compose ps
```

8. Monitored application logs:

```bash
docker compose logs -f
```

9. Stopped and removed the services:

```bash
docker compose down
```

### Technologies Used

* Docker
* Docker Compose
* Node.js
* Redis
* YAML
* Containers

---

# 🛠️ Technologies Used Overall

The eight laboratory tasks provided practical experience with the following technologies and concepts:

| Category                         | Technologies / Concepts                           |
| -------------------------------- | ------------------------------------------------- |
| **Operating Systems**            | Windows, Ubuntu, Linux                            |
| **Linux Environment**            | WSL                                               |
| **Shell / Administration**       | PowerShell, Linux Commands                        |
| **Remote Access**                | SSH, OpenSSH, RSA                                 |
| **Security**                     | SSH Security Hardening, Public-Key Authentication |
| **Web Development**              | HTML, CSS, JavaScript                             |
| **Backend Development**          | Node.js, Express.js                               |
| **Version Control**              | Git, GitHub                                       |
| **Cloud Hosting**                | Netlify, Vercel                                   |
| **Containerization**             | Docker, Docker Desktop                            |
| **Container Images**             | Docker Hub, Custom Docker Images                  |
| **Container Configuration**      | Dockerfile                                        |
| **Multi-Container Applications** | Docker Compose                                    |
| **Database / Service**           | Redis                                             |
| **Configuration**                | YAML, `vercel.json`                               |

---

# 📂 How to Access the Lab Reports

Follow the steps below to access all eight laboratory reports.

### 1. Clone the Repository

Open a terminal or Git Bash and run:

```bash
git clone https://github.com/AmanTariq1/2023-SE-29-Cloud-Computing-Lab-Tasks.git
```

### 2. Navigate to the Repository

```bash
cd 2023-SE-29-Cloud-Computing-Lab-Tasks
```

### 3. View the Repository Contents

```bash
ls
```

On Windows Command Prompt, you can use:

```cmd
dir
```

You should see:

```text
2023-SE-29.zip
README.md
```

### 4. Extract the ZIP File

Extract:

```text
2023-SE-29.zip
```

using Windows File Explorer or any ZIP extraction utility.

### 5. Access the Lab Reports

After extraction, the folder will contain the documentation for all **8 Cloud Computing lab tasks**, including the relevant Word/PDF files and supporting material.

---

# 🌐 Live Deployments

Two laboratory tasks include publicly accessible deployments.

| Task        | Deployment              | Platform | Link                                                          |
| ----------- | ----------------------- | -------- | ------------------------------------------------------------- |
| **Task 04** | Static Website          | Netlify  | [Open Website](https://2023-se-29-static-website.netlify.app) |
| **Task 05** | Backend Web Application | Vercel   | [Open Application](https://2023-se-29-backend-app.vercel.app) |

> **Note:** Availability of externally hosted projects may depend on the hosting platforms and deployment configuration.

---

# 📊 Learning Outcomes

Through these laboratory tasks, the following practical areas of Cloud Computing were explored:

* Setting up a Linux environment using WSL.
* Working with Ubuntu and Linux command-line tools.
* Configuring SSH-based remote access.
* Implementing SSH public-key authentication.
* Applying basic SSH security hardening.
* Deploying static websites to cloud hosting platforms.
* Deploying backend applications using PaaS.
* Using Git and GitHub for source-code management.
* Understanding Docker images and containers.
* Building custom Docker images with Dockerfiles.
* Running and inspecting containers.
* Creating multi-container applications.
* Using Docker Compose to manage application services.
* Integrating Redis into a containerized application environment.

---

# 👨‍💻 Author

### Aman Tariq

**Roll Number:** 2023-SE-29
**Department:** Software Engineering
**University:** The University of Azad Jammu and Kashmir
**Session:** 2023–27
**Course:** Cloud Computing (SE-3202)

---

# 📧 Contact

* **Email:** [amantariq344@gmail.com](mailto:amantariq344@gmail.com)
* **GitHub:** [github.com/AmanTariq1](https://github.com/AmanTariq1)
* **Repository:** [2023-SE-29-Cloud-Computing-Lab-Tasks](https://github.com/AmanTariq1/2023-SE-29-Cloud-Computing-Lab-Tasks)

---

# 📜 License & Academic Disclaimer

This repository contains **academic work completed as part of the Cloud Computing (SE-3202) course** at **The University of Azad Jammu and Kashmir, Department of Software Engineering**.

The contents are intended primarily for **educational and academic purposes**. The laboratory tasks demonstrate practical implementation of cloud computing, Linux, SSH, web deployment, containerization, and related technologies.

This repository is **not intended to represent a commercial production system**. External services, hosting platforms, APIs, and third-party technologies remain subject to their respective terms and conditions.

---

## 📌 Academic Information

| Field           | Information                              |
| --------------- | ---------------------------------------- |
| **Course Code** | SE-3202                                  |
| **Course Name** | Cloud Computing                          |
| **Instructor**  | Engr. Fahad Nisar                        |
| **Semester**    | Spring 2026                              |
| **Student**     | Aman Tariq                               |
| **Roll No.**    | 2023-SE-29                               |
| **Session**     | 2023–27                                  |
| **Department**  | Software Engineering                     |
| **University**  | The University of Azad Jammu and Kashmir |

---

## ⭐ Repository

If you find this repository useful for learning or reference, you can explore the complete project on GitHub:

**[AmanTariq1/2023-SE-29-Cloud-Computing-Lab-Tasks](https://github.com/AmanTariq1/2023-SE-29-Cloud-Computing-Lab-Tasks)**

---

### 📅 Last Updated

**September 2026**

---

> **Cloud Computing (SE-3202) — Spring 2026**
> *Practical Learning • Cloud Deployment • Containerization • DevOps Foundations*
