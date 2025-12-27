AI Career Mentor

An AI-powered career guidance platform for students

📌 Problem Statement

Many students struggle to make informed career decisions due to:

Lack of personalized career guidance

Limited access to mentors

Rapidly evolving skill requirements in AI and cloud technologies

This often leads to confusion, skill mismatches, and missed opportunities for internships and employment.

💡 Solution

AI Career Mentor is an AI-powered web platform that provides:

Personalized career guidance based on a student’s interests and education level

Structured, multi-year learning roadmaps

Clear recommendations for skills, projects, and certifications

The platform makes career planning accessible, structured, and actionable for students globally.

🧠 How It Works

A user submits a career-related question or interest

The backend processes the input and generates:

A concise professional summary

A detailed career roadmap (available on demand)

The frontend:

Displays the summary first to avoid information overload

Allows users to expand and view the full roadmap when needed

This approach balances clarity with depth.

🏗️ System Architecture

AI Career Mentor follows a modular, cloud-ready architecture that separates the frontend, backend, and AI logic layers to ensure scalability and maintainability.

High-Level Architecture Flow
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

Frontend Layer

Lightweight, responsive web interface

Hosted on Azure Static Web Apps

Responsible for:

Capturing user career queries

Displaying concise summaries

Allowing users to toggle and view detailed roadmaps

Backend Layer

Built using FastAPI

Exposes a REST endpoint: /api/career-advice

Handles:

Input validation

Career logic processing

Structured response generation (summary + roadmap)

FastAPI was selected for its performance and cloud deployment friendliness.

AI & Intelligence Layer

Currently uses structured, rule-based logic for roadmap generation

Designed to be AI-ready for seamless Azure OpenAI integration

Planned enhancements include:

Context-aware AI responses

Dynamic roadmap generation

Personalized mentoring based on user profiles

Cloud & Deployment Strategy

Azure Static Web Apps – Frontend hosting

FastAPI (Azure / Render) – Backend API hosting

GitHub – Source control and CI/CD

Azure OpenAI (planned) – Intelligent response generation

🤖 Azure OpenAI Integration Plan

AI Career Mentor is built with an AI-first design, enabling future integration with Azure OpenAI when regional access is available.

Why Azure OpenAI

Enterprise-grade security and compliance

Built-in Responsible AI tooling

Native Azure ecosystem integration

Scalable, production-ready language models

Planned Azure OpenAI Flow
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

Prompt Design Strategy

Prompts will include:

Education level

Career interests

Structured output requirements (summary + roadmap)

This ensures:

Consistent output quality

Reduced hallucinations

Guidance-focused responses

Fallback & Reliability

Due to current regional limitations:

A rule-based logic layer is active

The AI interface is abstracted to allow:

Easy replacement with Azure OpenAI

No frontend or architectural changes

⚖️ Responsible AI Considerations

The platform follows responsible AI principles by:

Providing guidance rather than deterministic decisions

Avoiding biased or harmful recommendations

Encouraging continuous learning

Maintaining transparency in AI-generated outputs

Future versions will include explainability and user feedback loops.

🌍 Impact

Helps students make better-informed career decisions

Reduces reliance on costly private mentoring

Scales globally through cloud deployment

Supports employability in high-demand technology fields

🚀 Future Enhancements

Full Azure OpenAI-powered conversational mentoring

Resume analysis and skill-gap detection

Internship and project recommendations

User profiles and progress tracking

Multi-language support

🎯 Imagine Cup Alignment

AI Career Mentor aligns with Imagine Cup goals by:

Addressing a real-world education and employability challenge

Using AI and cloud technologies responsibly

Demonstrating scalability and social impact

Applying AI for meaningful, real-life outcomes

📂 Repository Structure
ai-career-mentor/
├── ai-career-mentor-ui/   # Frontend
├── backend/               # FastAPI backend
├── .gitignore
└── README.md

👤 Author

Sai Surya Hemanth Sanapathi
Imagine Cup Participant | AI & Cloud Enthusiast