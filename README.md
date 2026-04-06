# DevOps CI Setup using AWS EC2, GitHub, and Jenkins

This project demonstrates a **hands-on Continuous Integration (CI) workflow** built as part of my **4-day DevOps training journey (Day 1)**.

The goal of this setup is to automate the build process whenever code changes are pushed to GitHub.

---

## Project Workflow

```text
Code change in EC2 shell
        ↓
Push to GitHub
        ↓
GitHub Webhook Trigger
        ↓
Jenkins Build Starts Automatically
        ↓
Java Build Success
```

This setup shows how **CI works in a real DevOps workflow**.

---

##  Tech Stack

* **AWS EC2 (Ubuntu)** – Cloud server setup
* **PuTTY / Linux Shell** – Secure server access
* **Git & GitHub** – Version control and source repository
* **Jenkins** – Continuous Integration automation server
* **Java** – Sample build validation
* **GitHub Webhooks** – Automatic Jenkins trigger

---

## What I Implemented

* Launched an Ubuntu EC2 instance on AWS
* Connected securely using SSH
* Managed project files in Linux shell
* Created and modified Java source files
* Initialized Git repository inside project workspace
* Pushed code to GitHub
* Installed Jenkins on EC2
* Configured Jenkins freestyle job
* Added shell build steps
* Enabled GitHub hook trigger
* Verified automatic build success

---

## ⚙️ Jenkins Build Step

```bash
cd /home/ubuntu/dir1
javac HelloWorld.java
java HelloWorld
```

---

## 🔗 Webhook Integration

GitHub webhook payload URL used:

```text
http://<EC2-PUBLIC-IP>:8080/github-webhook/
```

This automatically triggers Jenkins whenever a new commit is pushed.

---

## Output Proof

This repository includes screenshots showing:

1. Code changes made in EC2 shell
2. GitHub updated commit
3. Jenkins auto-triggered successful build

---

##  Learning Outcome

Through this project, I learned:

* Linux file and permission handling
* Git troubleshooting and remote setup
* Jenkins installation and service management
* Freestyle job configuration
* Webhook-based CI automation
* Debugging build failures using console output

---


## Author

**Mowshika**
DevOps Learner | AWS | Jenkins | CI/CD | Cloud Automation
