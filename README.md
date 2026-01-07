# AI Career Mentor
**An AI-powered career guidance platform for students**

## 🎬 Demo Video

▶️ **Imagine Cup MVP Demo – AI Career Mentor**  
A short walkthrough showcasing the frontend experience, structured career guidance flow, and roadmap interaction.

👉 Watch Demo (Unlisted YouTube):  
https://youtu.be/cPMfCEg9O58

## 📌 Problem Statement

Many students struggle to make informed career decisions due to:
- Lack of personalized career guidance
- Limited access to mentors
- Rapidly evolving skill requirements in AI and cloud technologies

This often leads to confusion, skill mismatches, and missed opportunities for internships and employment.

## 💡 Solution

AI Career Mentor is an AI-powered web platform that provides:
- Personalized career guidance based on a student’s interests and education level
- Structured, multi-year learning roadmaps
- Clear recommendations for skills, projects, and certifications

The platform makes career planning accessible, structured, and actionable for students globally.

## 🧠 How It Works

1. A user submits a career-related question or interest  
2. The backend processes the input and generates:
   - A concise professional summary
   - A detailed career roadmap (available on demand)
3. The frontend:
   - Displays the summary first to avoid information overload
   - Allows users to expand and view the full roadmap when needed

This approach balances clarity with depth.

## 🏗️ System Architecture

AI Career Mentor follows a modular, cloud-ready architecture that separates the frontend, backend, and intelligence layers to ensure scalability and maintainability.

### High-Level Architecture Flow

User (Browser)
↓
Frontend (Azure Static Web Apps)
↓ HTTPS REST API
Backend (FastAPI)
↓
Career Logic / AI Layer
↓
Structured Career Guidance Response

### Frontend Layer
- Lightweight, responsive web interface
- Hosted on Azure Static Web Apps
- Responsible for:
- Capturing user career queries
- Displaying concise summaries
- Toggling detailed roadmaps on demand

### Backend Layer
- Built using FastAPI
- Exposes a REST endpoint: `/api/career-advice`
- Handles:
- Input validation and cleanup
- Career logic processing
- Structured response generation (summary + roadmap)

FastAPI was selected for its performance and cloud deployment friendliness.

### AI & Intelligence Layer
- Uses structured, rule-based logic for roadmap generation
- Includes input normalization to handle spelling variations
- Designed to be AI-ready for seamless Azure OpenAI integration

Planned enhancements include:
- Context-aware AI responses
- Dynamic roadmap generation
- Personalized mentoring based on user profiles

## ☁️ Cloud & Deployment Strategy
- **Azure Static Web Apps** – Frontend hosting
- **FastAPI (Render / Azure-ready)** – Backend API hosting
- **GitHub** – Source control and CI/CD
- **Azure OpenAI (planned)** – Intelligent response generation

## 🤖 Azure OpenAI Integration Plan

AI Career Mentor is built with an AI-first design, enabling future integration with Azure OpenAI when regional access is available.

### Why Azure OpenAI
- Enterprise-grade security and compliance
- Built-in Responsible AI tooling
- Native Azure ecosystem integration
- Scalable, production-ready language models

### Planned Flow

User Query
↓
Frontend
↓
Backend (Prompt Construction)
↓
Azure OpenAI (GPT Model)
↓
Structured Career Guidance Response

### Fallback & Reliability

Due to current regional limitations:
- A rule-based logic layer is active
- The AI interface is abstracted to allow:
- Easy replacement with Azure OpenAI
- No frontend or architectural changes

## ⚖️ Responsible AI Considerations

The platform follows responsible AI principles by:
- Providing guidance rather than deterministic decisions
- Avoiding biased or harmful recommendations
- Encouraging continuous learning
- Maintaining transparency in AI-generated outputs

Future versions will include explainability and user feedback loops.

## 🌍 Impact

- Helps students make better-informed career decisions
- Reduces reliance on costly private mentoring
- Scales globally through cloud deployment
- Supports employability in high-demand technology fields

## 🚀 Future Enhancements

- Full Azure OpenAI-powered conversational mentoring
- Resume analysis and skill-gap detection
- Internship and project recommendations
- User profiles and progress tracking
- Multi-language support

## 🎯 Imagine Cup Alignment

AI Career Mentor aligns with Imagine Cup goals by:
- Addressing a real-world education and employability challenge
- Using AI and cloud technologies responsibly
- Demonstrating scalability and social impact
- Applying AI for meaningful, real-life outcomes

## 🎬 Demo Walkthrough (For Judges)

**Demo Duration:** 30–45 seconds

### Demo Steps
1. Open the live frontend URL  
2. Observe the clean, chat-style interface  
3. Enter a career-related question or interest  

No login. No setup. Instant access.

### Key Feature Highlight — Toggle-Based Roadmap
- Summary shown by default
- Full roadmap revealed only on request
- Same message container expands and collapses content

This design avoids cognitive overload while preserving depth.

## 📂 Repository Structure

ai-career-mentor/
├── frontend/ # Azure Static Web App
├── backend/ # FastAPI backend
├── .gitignore
└── README.md

## 👤 Author

**Sai Surya Hemanth Sanapathi**  
Imagine Cup Participant | AI & Cloud Enthusiast
