# ☁️ CloudArchitect AI – AI-Powered AWS Infrastructure Advisor

CloudArchitect AI is an AI-powered web application that helps developers and businesses design scalable, secure, and cost-effective AWS cloud infrastructure based on their project requirements.

Users can describe their application requirements, and the system uses Google Gemini AI to generate AWS architecture recommendations, estimated monthly costs, security best practices, architecture reasoning, and Terraform infrastructure-as-code suggestions.

The goal is to simplify cloud architecture planning and make AWS infrastructure design easier, faster, and more accessible.

## 🚀 Live Demo & Project Links

| Resource | Link |
|---|---|
| 🌐 Live Demo – AWS S3 | [Open CloudArchitect AI](http://cloudarchitect-ai-frontend-2026.s3-website.ap-south-1.amazonaws.com/) |
| ☁️ EC2 Deployment | [Open EC2 Application](http://3.110.204.184/) |
| 💻 GitHub Repository | [View Source Code](https://github.com/kar98star/Infrastructure-advisor) |

**Deployment Information:**
- Frontend Hosting: Amazon S3 Static Website Hosting
- Backend Hosting: Amazon EC2
- Web Server: Nginx
- Process Management: PM2
- AWS Region: Asia Pacific (Mumbai) – `ap-south-1`

> **Note:** The current deployment uses HTTP. HTTPS support through Amazon CloudFront is planned as a future enhancement.

## ✨ Key Features

- **AI-Powered Architecture Generation:** Generates AWS architecture recommendations from natural-language project requirements.
- **AWS Service Recommendations:** Suggests suitable AWS services based on application needs.
- **Cost Estimation:** Provides estimated monthly infrastructure costs and service-wise cost breakdowns.
- **Security Recommendations:** Suggests security best practices for the proposed architecture.
- **Architecture Reasoning:** Explains why particular AWS services are recommended.
- **Terraform Suggestions:** Generates Terraform infrastructure-as-code configuration.
- **Interactive Interface:** Provides a simple and user-friendly React-based interface.

## 🛠️ Technology Stack

| Category | Technologies |
|---|---|
| Frontend | React.js, Vite, CSS |
| Backend | Node.js, Express.js |
| AI Integration | Google Gemini API |
| Cloud Platform | Amazon Web Services (AWS) |
| Compute | Amazon EC2 |
| Storage & Hosting | Amazon S3 |
| Web Server & Reverse Proxy | Nginx |
| Process Management | PM2 |
| Infrastructure as Code | Terraform |
| Version Control | Git, GitHub |

## 🏗️ How It Works

1. The user enters application requirements through the React frontend.
2. The frontend sends the requirements to the Node.js and Express backend.
3. The backend processes the request using the Google Gemini API.
4. Gemini generates AWS architecture recommendations, security practices, cost estimates, and Terraform suggestions.
5. The backend returns structured JSON data.
6. The frontend displays the generated architecture and recommendations.

## ☁️ AWS Deployment Architecture

The application uses AWS services for hosting and deployment.

- **Amazon EC2:** Hosts the Node.js backend and an Nginx-served frontend.
- **Amazon S3:** Hosts the static React frontend.
- **Nginx:** Serves frontend files and acts as a reverse proxy for backend API requests.
- **PM2:** Keeps the Node.js backend process running.

## ⚙️ Run Locally

### Prerequisites

- Node.js and npm
- Git
- Google Gemini API key

### 1. Clone the Repository

```bash
git clone https://github.com/kar98star/Infrastructure-advisor.git

cd Infrastructure-advisor
```

### 2. Backend Setup

```bash
cd backend

npm install
```

Create a `.env` file inside the backend directory:

```env
PORT=5000
GEMINI_API_KEY=your_gemini_api_key
```

Start the backend:

```bash
npm start
```

The backend will run on:

```text
http://localhost:5000
```

### 3. Frontend Setup

Open another terminal:

```bash
cd frontend

npm install

npm run dev
```

Open the local URL displayed by Vite in your browser.

## 🔐 Environment Variables

| Variable | Description |
|---|---|
| `PORT` | Backend server port |
| `GEMINI_API_KEY` | Google Gemini API key |

**Security Reminder:** Never upload your `.env` file, API keys, or other sensitive credentials to GitHub.

## 📁 Project Structure

```text
Infrastructure-advisor/
│
├── backend/
│   ├── services/
│   │   ├── geminiAI.js
│   │   └── geminiService.js
│   ├── server.js
│   ├── package.json
│   └── .env
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── services/
│   │   └── App.jsx
│   ├── public/
│   ├── package.json
│   └── vite.config.js
│
└── README.md
```

*Note: This is a representative project structure. Adjust it to match the actual files and folders in the repository.*

## 🎯 Project Objectives

- Simplify AWS infrastructure planning.
- Help developers select appropriate AWS services.
- Provide early-stage cloud cost estimates.
- Encourage secure and scalable cloud architecture.
- Automate infrastructure planning using AI.

## 🔮 Future Enhancements

- Interactive AWS architecture diagrams.
- More accurate cost estimation using AWS Pricing APIs.
- Direct Terraform file export.
- Support for Microsoft Azure and Google Cloud Platform.
- AWS Well-Architected Framework recommendations.
- User authentication and saved architecture history.
- HTTPS deployment using Amazon CloudFront.

## 👨‍💻 Author

**Kartikeya Verma**

- GitHub: [kar98star](https://github.com/kar98star)
- Project Repository: [CloudArchitect AI](https://github.com/kar98star/Infrastructure-advisor)

---

⭐ If you find this project interesting, consider giving the repository a star!

**CloudArchitect AI – Simplifying AWS Architecture Design with AI.**ider giving it a ⭐ on GitHub.
