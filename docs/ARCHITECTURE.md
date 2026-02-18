# System Architecture

## Core Concept
An AI Search Engine for NASA Biology that simplifies complex research papers into digestible insights.

## The Tech Stack
* **Frontend**: React.js 
* **Backend**: Python (Flask) 
* **AI Model**: Google Gemini 
* **Data Source**: NASA Open Science Database

## Operational Flow
1. **User Input**: Asks a question about space biology. 
2. **Retrieval**: System finds the relevant NASA study from the local database.
3. **NLP Processing**: Google Gemini removes technical jargon and summarizes.
4. **Output**: User receives a simplified, accurate answer. 

## Safety
**Grounded AI**: The chatbot is restricted to NASA data to prevent false info (hallucinations).
