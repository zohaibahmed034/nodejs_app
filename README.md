# simple-nodejs-app

A simple **Node.js web application** built as part of DevOps/Cloud Labs for demonstrating Continuous Integration and Docker deployment workflows on AWS.

This application serves as the backend *Node.js service* that can be containerized using Docker and deployed through AWS CodeBuild and AWS CodePipeline for CI/CD.

---

## 📌 Features

- Built with **Node.js**
- Runs a basic web server
- Ready to containerize with **Docker**
- Works with AWS CodeBuild/CodePipeline for CI/CD automation
- Configured to push Docker image to **ECR**

---

## 📁 Repository Structure

.
├── .gitignore
├── Dockerfile
├── buildspec.yaml
├── index.js
├── package-lock.json
└── package.json


- **Dockerfile** – defines how to build the Docker image  
- **buildspec.yaml** – AWS CodeBuild spec for CI pipeline  
- **index.js** – main application entrypoint  
- **package.json** – Node.js dependencies & scripts  
- **.gitignore** – ignored files

:contentReference[oaicite:1]{index=1}

---

## 💻 Prerequisites

Before running the app locally, make sure you have:

- **Node.js** (v14 or higher)
- **npm** (Node package manager)

---

## 🛠 Installation & Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/zohaibahmed034/nodejs_app.git


Navigate into the project:

cd nodejs_app


Install dependencies:

npm install

▶️ Run Locally

Start the application with:

npm start


It will start the server, and you can test it via your browser or Postman.

🐳 Run with Docker

To build the Docker image locally:

docker build -t nodejs_app .


To run the container locally:

docker run -p 3000:3000 nodejs_app

The application will be accessible at http://localhost:3000.

☁️ AWS Continuous Integration (CI)

This project includes a buildspec.yaml for AWS CodeBuild to:

Authenticate to Amazon ECR

Build the Docker image

Tag and push the image to your ECR repository

🚀 Once connected to a CodePipeline or GitHub webhook, this enables fully automated Docker image creation on every commit.

📦 Deployment with CodePipeline & ECS

You can extend this repository to a full CI/CD pipeline using AWS services:

GitHub as source

CodeBuild to build Docker image

Amazon ECR to store the image

Amazon ECS / Fargate to deploy the container

This is ideal for production workflows and automates pushes on code changes.

📚 Technologies Used

Node.js — JavaScript runtime

npm — Package management

Docker — Containerization

AWS CodeBuild / CodePipeline — CI/CD Automation

Amazon ECR — Docker registry

🤝 Contributing

Feel free to fork this repository and submit pull requests.
Please follow good commit practices and add meaningful documentation for any new features.

📄 License

This project is open source — feel free to use and modify as needed.

📫 Contact

If you have questions, suggestions, or feedback, you can reach out through my GitHub profile:

👉 https://github.com/zohaibahmed034
