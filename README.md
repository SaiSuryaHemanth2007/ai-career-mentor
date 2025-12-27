AI Career Mentor

An AI-powered career guidance platform for students

📌 Problem Statement

Millions of students struggle to make informed career decisions due to:

Lack of personalized guidance

Limited access to mentors

Rapidly changing skill requirements in AI and cloud technologies

This often leads to confusion, skill mismatch, and missed opportunities for internships and jobs.

💡 Solution

AI Career Mentor is an AI-powered web application that provides:

Personalized career guidance based on a student’s interests and education level

Structured, multi-year learning roadmaps

Clear guidance on skills, projects, and certifications

The platform makes career planning accessible, structured, and actionable for students anywhere.

🧠 How It Works

The user enters a career-related question or interest

The backend processes the input and generates:

A short professional summary

A detailed career roadmap (on demand)

The frontend displays:

A concise overview first

An option to expand and view the full roadmap

This ensures clarity without overwhelming the user.

🏗️ Architecture Overview
Frontend (Azure Static Web Apps)
        |
        |  HTTPS (REST API)
        v
Backend (FastAPI on Azure / Render)
        |
        |  AI Logic (Rule-based → Azure OpenAI ready)
        v
Career Roadmap Generation

☁️ Azure & Cloud Services Used

Azure Static Web Apps – Frontend hosting

FastAPI – Backend REST API

Azure AI / Azure OpenAI (planned integration) – Intelligent response generation

GitHub – Source control and CI/CD

The architecture is designed to seamlessly integrate Azure OpenAI when regional access is enabled.

⚖️ Responsible AI Considerations

The project follows responsible AI principles by:

Providing guidance, not deterministic decisions

Avoiding biased or harmful content

Encouraging continuous learning rather than fixed career paths

Ensuring transparency in how recommendations are generated

Future versions will include explainable AI outputs and user feedback loops.

🌍 Impact

Helps students make better-informed career decisions

Reduces dependency on costly private mentoring

Scales globally through cloud-based deployment

Supports employability in high-demand fields like AI and cloud computing

🚀 Future Enhancements

Azure OpenAI integration for dynamic, conversational mentoring

Resume analysis and skill-gap detection

Internship and project recommendations

User profiles and progress tracking

Multi-language support

🎯 Why This Matters (Imagine Cup Alignment)

AI Career Mentor aligns strongly with Imagine Cup goals by:

Solving a real-world educational problem

Using cloud and AI technologies responsibly

Being scalable, impactful, and accessible

Demonstrating practical application of AI for social good

📂 Repository Structure
ai-career-mentor/
├── ai-career-mentor-ui/   # Frontend (Static Web App)
├── backend/               # FastAPI backend
├── .gitignore
└── README.md

👤 Author

Sai Surya Hemanth Sanapathi
Imagine Cup Participant | AI & Cloud Enthusiast