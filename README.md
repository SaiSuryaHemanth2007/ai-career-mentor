AI Career Mentor

An AI-powered career guidance platform for students

📌 Problem Statement

Millions of students struggle to make informed career decisions due to:

Lack of personalized guidance

Limited access to mentors

Rapidly changing skill requirements in AI and cloud technologies

This often leads to confusion, poor skill alignment, and missed internship or job opportunities.

💡 Solution

AI Career Mentor is an AI-powered web application that provides:

Personalized career guidance based on a student’s interests and education level

Clear, structured multi-year learning roadmaps

Actionable guidance on skills, projects, and certifications

The platform makes career planning accessible, structured, and scalable for students everywhere.

🧠 How It Works

A user asks a career-related question or provides an area of interest

The backend processes the input and generates:

A short professional summary

A detailed career roadmap (shown on demand)

The frontend:

Displays the summary first to avoid information overload

Allows users to expand and view the full roadmap when needed

This design balances clarity with depth.

🏗️ System Architecture

AI Career Mentor follows a modular, cloud-ready architecture that cleanly separates the user interface, backend logic, and AI intelligence layer. This ensures scalability, maintainability, and future AI integration.

🔹 High-Level Architecture Flow
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

🔹 Frontend Layer

Lightweight, responsive web interface

Hosted on Azure Static Web Apps

Responsible for:

Capturing user career queries

Displaying a concise summary

Allowing users to toggle and view a full roadmap

The UI is designed to look professional and easy to understand, similar to modern AI assistants.

🔹 Backend Layer

Implemented using FastAPI

Exposes a REST endpoint (/api/career-advice)

Handles:

Input validation

Career logic processing

Structured response generation (summary + detailed roadmap)

FastAPI was chosen for its performance, clarity, and ease of cloud deployment.

🔹 AI & Intelligence Layer

Currently, the backend uses structured, rule-based logic to generate career roadmaps.
The system is intentionally designed to be AI-ready, enabling seamless integration with Azure OpenAI.

Planned AI enhancements include:

Dynamic roadmap generation using Azure OpenAI

Context-aware conversational mentoring

Personalized guidance based on user profiles and progress

This approach ensures reliability today and intelligent adaptability in future versions.

🔹 Cloud & Deployment Strategy

Azure Static Web Apps – Frontend hosting

FastAPI (Azure / Render) – Backend API hosting

GitHub – Source control and CI/CD

Azure OpenAI (planned) – Intelligent response generation

The architecture supports independent scaling of frontend and backend services.

🔹 Security & Best Practices

CORS configuration for controlled frontend access

No hardcoded secrets in the repository

Environment-variable–based configuration for future API keys

Clear separation of responsibilities across layers

🔹 Why This Architecture Works

Simple and easy to understand

Cloud-native and scalable

AI-ready without overengineering

Suitable for real-world deployment

Aligned with Microsoft Imagine Cup evaluation standards

⚖️ Responsible AI Considerations

AI Career Mentor follows responsible AI principles by:

Providing guidance rather than deterministic decisions

Avoiding biased or harmful recommendations

Encouraging continuous learning instead of fixed career paths

Maintaining transparency in how guidance is generated

Future versions will include explainable AI responses and user feedback loops.

🌍 Impact

Helps students make better-informed career decisions

Reduces dependency on expensive private mentoring

Scales globally through cloud deployment

Supports employability in high-demand fields like AI and cloud computing

🚀 Future Enhancements

Azure OpenAI integration for conversational mentoring

Resume analysis and skill-gap detection

Internship and project recommendations

User profiles and progress tracking

Multi-language support

🎯 Imagine Cup Alignment

This project aligns strongly with Imagine Cup goals by:

Solving a real-world education and employability problem

Using AI and cloud technologies responsibly

Being scalable, impactful, and accessible

Demonstrating practical AI application for social good

📂 Repository Structure
ai-career-mentor/
├── ai-career-mentor-ui/   # Frontend (Azure Static Web App)
├── backend/               # FastAPI backend
├── .gitignore
└── README.md

👤 Author

Sai Surya Hemanth Sanapathi
Imagine Cup Participant | AI & Cloud Enthusiast