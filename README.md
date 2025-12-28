# AI Career Mentor
**An AI-powered career guidance platform for students**

## 🎬 Demo Video

▶️ **Imagine Cup MVP Demo – AI Career Mentor**  
A short walkthrough showcasing the frontend experience, structured career guidance flow, and roadmap interaction.

👉 Watch Demo (Unlisted YouTube):  
https://youtu.be/oRIkbHDLQgg

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

AI Career Mentor follows a modular, cloud-ready architecture that separates the frontend, backend, and AI logic layers to ensure scalability and maintainability.

### High-Level Architecture Flow

User (Browser)
|
v
Frontend (Azure Static Web Apps)
|
| HTTPS REST API
v
Backend (FastAPI)
|
| Career Logic / AI Layer
v
Structured Career Guidance Response

### Frontend Layer
- Lightweight, responsive web interface
- Hosted on Azure Static Web Apps
- Responsible for:
  - Capturing user career queries
  - Displaying concise summaries
  - Allowing users to toggle and view detailed roadmaps

### Backend Layer
- Built using FastAPI
- Exposes a REST endpoint: `/api/career-advice`
- Handles:
  - Input validation
  - Career logic processing
  - Structured response generation (summary + roadmap)

FastAPI was selected for its performance and cloud deployment friendliness.

### AI & Intelligence Layer
- Uses structured, rule-based logic for roadmap generation
- Designed to be AI-ready for seamless Azure OpenAI integration

Planned enhancements include:
- Context-aware AI responses
- Dynamic roadmap generation
- Personalized mentoring based on user profiles

### Cloud & Deployment Strategy
- Azure Static Web Apps – Frontend hosting
- FastAPI (Azure / Render) – Backend API hosting
- GitHub – Source control and CI/CD
- Azure OpenAI (planned) – Intelligent response generation

## 🤖 Azure OpenAI Integration Plan

AI Career Mentor is built with an AI-first design, enabling future integration with Azure OpenAI when regional access is available.

### Why Azure OpenAI
- Enterprise-grade security and compliance
- Built-in Responsible AI tooling
- Native Azure ecosystem integration
- Scalable, production-ready language models

### Planned Azure OpenAI Flow

User Query
|
v
Frontend (Azure Static Web Apps)
|
v
Backend (FastAPI)
|
| Prompt Construction
v
Azure OpenAI (GPT Model)
|
v
Structured Career Guidance Response

### Prompt Design Strategy

Prompts include:
- Education level
- Career interests
- Structured output requirements (summary + roadmap)

This ensures:
- Consistent output quality
- Reduced hallucinations
- Guidance-focused responses

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

This walkthrough demonstrates how AI Career Mentor delivers structured, responsible, and actionable career guidance.

### Demo Setup
1. Open the live frontend URL  
2. See a clean chat-style interface  
3. Input a career-related question or interest  

No login, no setup — instant access.

### Demo Question 1 (Primary)
**Question:**  
“I am a second-year student interested in AI and cloud computing. What should I do next?”

**What the System Shows:**
- A short professional summary
- A “Show Full Roadmap” button below the summary

**Why This Matters:**
- Clarity-first design
- Avoids overwhelming users
- Demonstrates structured guidance

### Demo Question 2 (Skill Transition)
**Question:**  
“I know basic programming but want to move into AI roles. What skills should I focus on?”

### Demo Question 3 (Career Confusion)
**Question:**  
“I am confused about my career path. How can I prepare for future jobs?”

### Key Feature Highlight
**Toggle-Based Roadmap**
- Summary shown by default
- Full roadmap revealed only on request
- Same message box expands and collapses content

### Demo Duration
30–45 seconds total, designed to respect judges’ limited time.

## 🚀 Innovation Angle

AI Career Mentor is not a generic AI chatbot.  
Its innovation lies in how AI guidance is structured, controlled, and delivered for real-world student needs.

### Structured Guidance Over Open-Ended Chat
- Separates summaries from detailed roadmaps
- Allows progressive disclosure of information
- Reduces cognitive overload

### Career-Specific Intelligence
- Purpose-built for mentoring, not casual chat
- Roadmap-oriented outputs
- Guidance, not guarantees

### Responsible AI by Design
- Avoids deterministic career decisions
- Encourages adaptability and transparency

### AI-Ready, Not AI-Dependent
- Works reliably without generative AI
- Seamlessly integrates Azure OpenAI when available

### Scalable Social Impact
- Democratizes access to mentorship
- Supports employability in fast-growing tech fields

## 📂 Repository Structure

ai-career-mentor/
├── ai-career-mentor-ui/ # Frontend
├── backend/ # FastAPI backend
├── .gitignore
└── README.md

## 👤 Author

**Sai Surya Hemanth Sanapathi**  
Imagine Cup Participant | AI & Cloud Enthusiast