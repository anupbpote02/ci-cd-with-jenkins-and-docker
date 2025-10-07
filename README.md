# Jenkins + Docker CI/CD Pipeline

This repository demonstrates a simple **CI/CD pipeline** that builds and pushes a Docker image using **Jenkins**.

---

## 🧩 Project Overview
The setup includes:
- A `Dockerfile` to build a basic Ubuntu-based image.
- A `Jenkinsfile` that automates:
  1. Git checkout
  2. Docker image build
  3. Docker image push to Docker Hub

---

## ⚙️ Jenkins Pipeline Stages

### **1. Git Checkout**
Pulls the latest version of the code from the repository.

### **2. Docker Build**
Builds a Docker image using the `Dockerfile` and tags it:
```bash
docker build -t anupbpote/myimage6 .
```

### **3. Docker Push**
Pushes the image to Docker Hub:
```bash
docker push anupbpote/myimage6:latest
```

---

## 🚀 How to Run Locally
1. Clone the repository:
   ```bash
   git clone https://github.com/anupbpote02/ci-cd-with-jenkins-and-docker.git
   cd jenkins-docker-pipeline
   ```

2. Build the Docker image:
   ```bash
   docker build -t myimage6 .
   ```

3. Run the container:
   ```bash
   docker run myimage6
   ```

You’ll see:
```
Hello world!!! this is my first docker image
```

---

## 🧠 Key Learnings
- Integrating **Jenkins** with **Docker** for continuous integration and delivery  
- Automating image build and push processes  
- Understanding declarative pipelines (`Jenkinsfile`)  

---

## 🧰 Tools & Technologies
- **Jenkins**
- **Docker**
- **Ubuntu**
- **Groovy (Jenkinsfile DSL)**
- **CI/CD Automation**

---

## 📘 Reference
- [Jenkins Pipeline Syntax](https://www.jenkins.io/doc/book/pipeline/syntax/)
- [Docker Official Docs](https://docs.docker.com/)

---

⭐ *A simple but powerful demonstration of automating Docker image builds and pushes using Jenkins CI/CD pipelines.*
