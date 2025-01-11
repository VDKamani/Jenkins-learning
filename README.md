# jenkins-learning

---

# Jenkins Pipeline Tasks

This repository contains Jenkins pipeline scripts to demonstrate various use cases, including cloning repositories, building Docker images, conditional logic based on branches, and deploying applications to EC2 instances. Below is the list of tasks with their respective descriptions.

---

### **Filename:** `Jenkinsfile-back`
**Description:**
This task involves creating a pipeline to clone a GitHub repository, build a Docker image, push the image to AWS ECR, and deploy it on an EC2 instance using SSH commands.

---

### **Filename:** `Jenkinsfile-bak-if-else`
**Description:**
This task demonstrates the use of conditional logic in a pipeline to perform specific actions based on the current branch name (e.g., `main`, `dev`, `preprod`).

---

### **Filename:** `Jenkinsfile-cred`
**Description:**
This task creates a multistage pipeline (`Dev`, `Stage`, `Prod`) using parameters such as name, city, and password. It showcases storing credentials in Jenkins' credential manager and dynamically accessing them during builds.

---

### **Filename:** `Jenkinsfile-cred-print`
**Description:**
This task focuses on accessing and printing credentials stored in the Jenkins credential manager within a multistage pipeline. It includes stages to demonstrate parameterized builds.

---

### **Filename:** `Jenkinsfile-docker-task`
**Description:**
This task defines a multistage pipeline (`Dev`, `Stage`, `Prod`) with global and stage-specific parameters. It highlights parameterized builds, including the use of Docker for deployments.

---

### **Filename:** `Jenkinsfile-multi-main`
**Description:**
This pipeline listens to pushes on specific GitHub branches (`master`, `pre-prod`, `stage`, `dev`) and triggers corresponding build stages (e.g., `Prod`, `Pre-prod`, `Stage`, `Dev`).

---

### **Filename:** `jenkinsfile-ref-full-multisame`
**Description:**
A refined multistage pipeline for multiple branches. It includes branch identification and specific steps based on the branch being built (e.g., `master`, `pre-prod`, etc.).

---

## How to Use
1. Clone this repository to your local machine.
2. Upload the desired Jenkinsfile to your Jenkins pipeline.
3. Configure the pipeline settings, including required parameters and credentials.
4. Trigger the pipeline to test the functionality of the Jenkinsfile.

## Prerequisites
- Jenkins installed and configured.
- Docker and AWS CLI installed (for Docker-based pipelines).
- Credentials stored in the Jenkins credential manager.
- GitHub repository access for cloning and pushing code.

## License
This repository is open source and available for educational purposes. Use at your own discretion.

