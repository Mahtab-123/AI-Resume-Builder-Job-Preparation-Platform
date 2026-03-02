# 🚀 AI-Powered Interview & ATS Resume Builder

A full-stack web application that allows users to upload resumes, analyze job descriptions, detect skill gaps, and generate AI-powered interview questions along with ATS-optimized resumes.

This project simulates a real-world SaaS product and demonstrates Full Stack Development + Generative AI integration.

---

## 📌 Features

- 🔐 Secure Authentication using JWT
- 🚫 Token Blacklisting for Secure Logout
- 📄 Resume Upload & Parsing
- 🧠 AI-Based Skill Extraction
- 📊 Skill Gap Detection (Resume vs Job Description)
- 🎯 AI-Generated Interview Questions
- 📝 ATS-Optimized Resume Generation
- 📑 Dynamic Resume PDF Creation using Puppeteer
- 🔒 Protected Routes
- 🏗 Clean & Scalable Architecture

---

## 🛠 Tech Stack

### Frontend
- React.js
- Vite
- React Router
- Axios
- Context API

### Backend
- Node.js
- Express.js
- MongoDB Atlas
- Mongoose

### Authentication
- JWT (JSON Web Tokens)
- Token Blacklisting
- HTTP-only Cookies

### AI Integration
- Gemini API

### File Handling & PDF
- Multer (File Uploads)
- Puppeteer (Dynamic PDF Generation)

---

## 📂 Folder Structure

- 📁 [Backend](./Backend) – Contains the Node.js backend server  
- 📁 [Frontend](./Frontend) – Contains the React frontend application  
- 📄 [README.md](./README.md) – Detailed project documentation  

---

## ⚙️ Installation & Setup

### 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

---

### 2️⃣ Backend Setup

```bash
cd backend
npm install
```

Create a `.env` file inside the backend folder:

```
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
GEMINI_API_KEY=your_gemini_api_key
```

Start the backend server:

```bash
npm run dev
```

Server will run on:

```
http://localhost:5000
```

---

### 3️⃣ Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

Frontend will run on:

```
http://localhost:5173
```

---

## 🔐 Authentication Flow

1. User registers or logs in  
2. JWT token is generated  
3. Protected routes validate token  
4. On logout, token is blacklisted  
5. Blacklisted tokens cannot access protected APIs  

---

## 🤖 AI Workflow

1. User uploads resume  
2. Resume is parsed and skills are extracted  
3. User provides job description  
4. AI compares resume skills with job requirements  
5. Skill gaps are identified  
6. AI generates:
   - Interview questions  
   - Interview report  
   - ATS-optimized resume  
7. Resume PDF is generated dynamically using Puppeteer  

---

## 🧪 API Endpoints

### Auth APIs
- POST `/api/auth/register`
- POST `/api/auth/login`
- POST `/api/auth/logout`
- GET `/api/auth/me`

### Interview APIs
- POST `/api/interview/generate`
- GET `/api/interview/:id`
- GET `/api/interview`

### Resume APIs
- POST `/api/resume/generate-pdf`

---

## 🎯 Learning Outcomes

- Real-world Full Stack architecture  
- Secure authentication implementation  
- Token blacklisting mechanism  
- AI integration in production apps  
- Resume parsing and skill gap detection  
- Backend-to-PDF generation pipeline  

---

## 📄 License

This project is built for educational purposes.  
Feel free to fork and improve.
