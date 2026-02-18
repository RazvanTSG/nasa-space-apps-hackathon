# 🏗️ System Architecture & Engineering

## High-Level Overview
The system is designed to bridge the gap between raw scientific data and accessible education. It acts as a middleware layer that ingests complex NASA Space Biology datasets and serves them through a simplified, gamified frontend.

## 🔄 Data Flow Diagram
```mermaid
graph TD
    User[User / Student] -->|Queries| FE[Frontend (React/Lovable)]
    FE -->|API Requests| BE[Backend API (Python/Flask)]
    
    subgraph "Data Processing Layer"
        BE -->|Fetch Data| NASA[NASA Bioscience API]
        BE -->|Vector Search| KG[Knowledge Graph]
    end
    
    subgraph "AI & NLP Engine"
        NASA -->|Raw Publications| NLP[NLP Processing]
        NLP -->|Summarization| GEM[Google Gemini]
        GEM -->|Simplified Content| BE
    end
    
    FE -->|Render| EXP[Explore Mode / Rocket UI]
    FE -->|Chat Interaction| BOT[AI Chatbot]
🛠️ Tech Stack & Integration
Frontend: React.js (via Lovable) for the interactive "Explore Mode" and responsive UI.

Backend: Python (Flask) acting as the orchestrator between the frontend and data services.

AI Engine: Google Gemini & Custom NLP scripts to process academic language into student-friendly summaries.

Data Source: 608 Full-text Open-Access Space Biology Publications (NASA).

🧩 Key Components
The Explore Mode: A gamified interface (Rocket Navigation) that visualizes the Knowledge Graph relationships.

Intelligent Search: A retrieval-augmented generation (RAG) system that restricts answers strictly to the verified NASA dataset to prevent hallucinations.

Bioscience Translation: Automated pipelines that convert "dense scientific jargon" into "digestible content".
