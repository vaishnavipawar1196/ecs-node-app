# 🚀 AWS ECS Node.js CI/CD Deployment

A production-style Node.js application deployed on **Amazon ECS Fargate** using **Docker**, **Amazon ECR**, and **GitHub Actions** for automated CI/CD.

This project demonstrates containerization, cloud deployment, and continuous delivery on AWS.

---

# 📌 Architecture

```text
                Developer
                    │
                    ▼
            GitHub Repository
                    │
           (Push to main branch)
                    │
                    ▼
            GitHub Actions CI/CD
                    │
         Build Docker Image
                    │
                    ▼
           Push Image to Amazon ECR
                    │
                    ▼
        Amazon ECS Fargate Service
                    │
                    ▼
           Running Node.js Container
```

---

# 🛠 Technologies Used

- Node.js
- Express.js
- Docker
- Amazon ECS (Fargate)
- Amazon ECR
- GitHub Actions
- AWS IAM
- AWS CloudWatch

---

# 📂 Project Structure

```
aws-ecs-nodejs-project/
│
├── .github/
│   └── workflows/
│       └── deploy.yml
│
├── app.js
├── Dockerfile
├── package.json
├── package-lock.json
├── .dockerignore
└── README.md
```

---

# 🚀 Features

- Dockerized Node.js application
- Amazon ECR image repository
- Amazon ECS Fargate deployment
- GitHub Actions CI/CD
- Automatic deployment on every push
- Cloud-native container deployment

---

# ⚙️ Local Setup

Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/aws-ecs-nodejs-project.git
```

Go to project

```bash
cd aws-ecs-nodejs-project
```

Install dependencies

```bash
npm install
```

Run application

```bash
npm start
```

Open

```
http://localhost:3000
```

---

# 🐳 Docker

Build image

```bash
docker build -t ecs-node-app .
```

Run container

```bash
docker run -p 3000:3000 ecs-node-app
```

Application

```
http://localhost:3000
```

---

# ☁️ AWS Deployment

The application is deployed using:

- Amazon ECR
- Amazon ECS Fargate
- ECS Service
- ECS Task Definition
- IAM Roles
- CloudWatch Logs

Deployment flow:

```
GitHub Push
      │
      ▼
GitHub Actions
      │
      ▼
Docker Build
      │
      ▼
Amazon ECR
      │
      ▼
Amazon ECS
      │
      ▼
Updated Running Container
```

---

# 🔄 CI/CD Pipeline

Every push to the **main** branch automatically:

- Checks out source code
- Configures AWS credentials
- Builds Docker image
- Pushes image to Amazon ECR
- Updates ECS Task Definition
- Deploys new version to ECS Service
- Waits for deployment completion

---

# 🔐 GitHub Secrets

Configure the following repository secrets:

| Secret | Description |
|----------|-------------|
| AWS_ACCESS_KEY_ID | AWS Access Key |
| AWS_SECRET_ACCESS_KEY | AWS Secret Key |
| AWS_REGION | AWS Region (e.g. ap-south-1) |

---

# 📷 Screenshots

Add screenshots of:

- Amazon ECR Repository
- ECS Cluster
- ECS Service
- Running Task
- GitHub Actions Workflow
- Application Running

---

# 📚 Learning Outcomes

This project demonstrates:

- Docker containerization
- Amazon ECS Fargate deployment
- Amazon ECR image management
- GitHub Actions automation
- IAM permissions
- Continuous Integration
- Continuous Deployment
- Cloud-native application deployment

---

# 🎯 Future Improvements

- HTTPS using ACM
- Application Load Balancer
- Route 53 Domain
- Blue/Green Deployment
- Auto Scaling
- Terraform Infrastructure as Code
- AWS CodeDeploy integration

---

# 👩‍💻 Author

**Vaishnavi Pawar**

GitHub:
https://github.com/vaishnavipawar1196

LinkedIn:
https://www.linkedin.com/in/vaishnavi-pawar-315804169/

---

# ⭐ If you found this project helpful, consider giving it a star!
