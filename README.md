# ☁️ CloudArchitect AI

> **AI-Powered AWS Infrastructure Advisor**

CloudArchitect AI is a full-stack AI-powered application that analyzes natural-language project requirements and generates an optimized AWS cloud architecture.

The application uses **Google Gemini AI** to recommend AWS services, estimate infrastructure costs, suggest security best practices, generate Terraform code, and provide a deployment guide.

---

## 🚀 Live Demo

👉 **[CloudArchitect AI – Live Demo](http://cloudarchitect-ai-kartikeya.s3-website.ap-south-1.amazonaws.com/)**

---

## ✨ Features

* 🤖 AI-powered AWS architecture generation
* ☁️ Intelligent AWS service recommendations
* 🔐 Security best-practice recommendations
* 💰 Monthly infrastructure cost estimation
* 🏗️ Interactive AWS architecture visualization
* 📄 Terraform code generation
* 📥 Terraform file download
* 📋 Deployment guide
* 📄 PDF architecture report export
* 🕒 Architecture history using Local Storage

---

## 🛠️ Tech Stack

### Frontend

* React.js
* Vite
* Axios
* JavaScript
* HTML5
* CSS3
* jsPDF

### Backend

* Node.js
* Express.js
* Google Gemini API
* REST API

### Cloud & DevOps

* AWS EC2
* Amazon S3 Static Website Hosting
* PM2
* Git
* GitHub

---

## 🏗️ System Architecture

```text
                    User
                      │
                      ▼
          ┌─────────────────────┐
          │   Amazon S3         │
          │ Static Website      │
          └──────────┬──────────┘
                     │
                     ▼
          ┌─────────────────────┐
          │   React + Vite      │
          │     Frontend        │
          └──────────┬──────────┘
                     │
                 REST API
                     │
                     ▼
          ┌─────────────────────┐
          │      AWS EC2        │
          │ Node.js + Express   │
          │       + PM2         │
          └──────────┬──────────┘
                     │
                     ▼
          ┌─────────────────────┐
          │   Google Gemini     │
          │      AI API         │
          └──────────┬──────────┘
                     │
                     ▼
          ┌─────────────────────┐
          │ AI Generated AWS    │
          │    Architecture     │
          └─────────────────────┘
```

---

## 🔄 Application Workflow

```text
User enters project requirement
            ↓
React Frontend
            ↓
REST API Request
            ↓
Node.js + Express Backend
            ↓
Google Gemini AI
            ↓
Requirement Analysis
            ↓
AWS Architecture Generation
            ↓
┌──────────────────────────────┐
│ AWS Service Recommendations  │
│ Security Recommendations     │
│ Cost Estimation              │
│ Terraform Code               │
│ Deployment Guide             │
└──────────────────────────────┘
            ↓
React Dashboard
```

---

## 📊 Generated Architecture

Based on the user's requirements, CloudArchitect AI can generate:

### ☁️ AWS Services

The AI can recommend services such as:

* Amazon EC2
* AWS Lambda
* Amazon API Gateway
* Amazon S3
* Amazon RDS
* Amazon DynamoDB
* Amazon CloudFront
* AWS WAF
* Amazon CloudWatch
* Amazon SNS
* Elastic Load Balancing
* Amazon ElastiCache

### 🔐 Security

The application provides recommendations such as:

* IAM roles and least-privilege permissions
* MFA
* Encryption
* Secure S3 bucket configuration
* Network security
* Monitoring and logging

### 💰 Cost Estimation

The application provides an estimated monthly infrastructure cost along with a service-level cost breakdown.

### 🏗️ Terraform

The application generates Terraform Infrastructure-as-Code that can be used as a starting point for AWS deployment.

---

## 📂 Project Structure

```text
CloudArchitect-AI
│
├── frontend
│   ├── src
│   ├── public
│   ├── package.json
│   └── vite.config.js
│
├── backend
│   ├── services
│   ├── server.js
│   ├── package.json
│   └── .env
│
├── package.json
└── README.md
```

---

# ⚙️ Local Installation

## 1. Clone Repository

```bash
git clone https://github.com/kar98star/Infrastructure-advisor.git
```

```bash
cd Infrastructure-advisor
```

---

## 2. Backend Setup

```bash
cd backend
npm install
```

Create a `.env` file:

```env
PORT=5000
GEMINI_API_KEY=YOUR_GEMINI_API_KEY
```

Start the backend:

```bash
node server.js
```

Or run it using PM2:

```bash
pm2 start server.js --name cloudarchitect-backend
```

---

## 3. Frontend Setup

Open another terminal:

```bash
cd frontend
npm install
```

Start the development server:

```bash
npm run dev
```

For a production build:

```bash
npm run build
```

---

# 🚀 Deployment

## Frontend – Amazon S3

The React frontend is deployed using:

**Amazon S3 Static Website Hosting**

Live application:

👉 **[CloudArchitect AI](http://cloudarchitect-ai-kartikeya.s3-website.ap-south-1.amazonaws.com/)**

---

## Backend – AWS EC2

The backend is deployed on an **AWS EC2 instance** using:

* Node.js
* Express.js
* PM2

PM2 keeps the backend application running as a background process and automatically restarts it if required.

---

# 🧪 Example Requirement

The user can enter a natural-language requirement such as:

```text
Build a food delivery application for 50,000 users
with real-time order tracking.
```

CloudArchitect AI analyzes the requirement and generates:

```text
AWS Architecture
        ↓
Security Recommendations
        ↓
Cost Estimation
        ↓
Terraform Code
        ↓
Deployment Guide
```

---

# 🎯 Use Cases

CloudArchitect AI can help:

* Developers design AWS architectures
* Students learn AWS architecture
* Beginners understand AWS services
* Teams quickly create infrastructure proposals
* Developers generate Terraform starting points
* Estimate initial AWS infrastructure costs

---

# 🔮 Future Improvements

* 🔐 User authentication
* 🗄️ MongoDB integration
* 🌐 CloudFront + HTTPS
* 🔗 Custom domain
* 🐳 Docker containerization
* ⚙️ CI/CD using GitHub Actions
* 📊 CloudWatch monitoring
* ☸️ Kubernetes deployment
* ☁️ Multi-cloud recommendations for AWS, Azure, and GCP
* 📈 More accurate AWS cost estimation

---

# 👨‍💻 Author

### Kartikeya Verma

**GitHub:**
https://github.com/kar98star

**LinkedIn:**
https://www.linkedin.com/in/kartikeya-verma-12737328a/

---

## ⭐ Project Highlights

* Full-stack AI application
* React + Node.js architecture
* Google Gemini API integration
* AWS cloud deployment
* S3 static website hosting
* EC2 backend deployment
* PM2 process management
* REST API integration
* Infrastructure-as-Code generation
* AI-powered cloud architecture recommendations

---

## 📜 License

This project is created for educational and portfolio purposes.


---

## ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub.
