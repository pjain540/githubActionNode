# 🚀 GitHub Actions CI/CD Pipeline with Docker & Node.js

This project demonstrates a complete **CI/CD pipeline** using GitHub Actions for a Node.js application. It includes automated linting, testing, Docker image building, and pushing the image to Docker Hub.

---

## 📌 Features

* ✅ Linting with ESLint
* ✅ Unit Testing with Jest
* ✅ Code Coverage Reporting
* ✅ Docker Image Build
* ✅ Push Image to Docker Hub
* ✅ Security Scan (npm audit)
* ✅ PostgreSQL Integration using Docker Compose

---

## 🛠️ Tech Stack

* Node.js
* Docker
* PostgreSQL
* GitHub Actions

---

## 📁 Project Structure

```
.
├── .github/
│   └── workflows/
│       └── ci.yml
├── docker-compose.yml
├── Dockerfile
├── .dockerignore
├── .eslintrc.json
├── package.json
├── package-lock.json
└── index.js
```

---

## ⚙️ Setup Instructions

### 1️⃣ Clone the Repository

```
git clone https://github.com/your-username/your-repo.git
cd your-repo
```

---

### 2️⃣ Run Locally (Without Docker)

```
npm install
npm start
```

---

### 3️⃣ Run with Docker

Build image:

```
docker build -t node-app .
```

Run container:

```
docker run -p 3000:3000 node-app
```

---

### 4️⃣ Run with Docker Compose (App + PostgreSQL)

```
docker-compose up
```

---

## 🔄 CI/CD Pipeline

The pipeline is implemented using GitHub Actions and includes:

1. **Install Dependencies**
2. **Run Linting**
3. **Run Tests**
4. **Generate Coverage**
5. **Build Docker Image**
6. **Push to Docker Hub**
7. **Security Scan**

---

## 🔑 GitHub Secrets Required

Add these secrets in your repository:

* `DOCKER_USERNAME`
* `DOCKER_PASSWORD` (Access Token)

---

## 🐳 Docker Image

The Docker image is available on Docker Hub:

```
docker pull your-dockerhub-username/node-app
```

Run the image:

```
docker run -p 3000:3000 your-dockerhub-username/node-app
```

---

## 🧪 Testing

Run tests locally:

```
npm test
```

---

## 🔍 Linting

```
npm run lint
```

---

## 🛡️ Security Check

```
npm audit
```

---

## 📈 Future Improvements

* 🔹 Deploy to AWS / Cloud
* 🔹 Add monitoring & logging
* 🔹 Auto deployment after build
* 🔹 Add caching for faster builds

---

## 📚 Conclusion

This project showcases how to build a complete CI/CD pipeline with Docker, ensuring consistent builds, automated testing, and seamless deployment.

---

## 👨‍💻 Author

Your Name

---
