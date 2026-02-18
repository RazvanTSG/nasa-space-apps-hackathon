# System Architecture

## Core Concept
[cite_start]An AI Search Engine for NASA Biology that simplifies complex research papers into digestible insights. [cite: 7, 8]

## The Tech Stack
* [cite_start]**Frontend**: React.js 
* [cite_start]**Backend**: Python (Flask) 
* [cite_start]**AI Model**: Google Gemini 
* [cite_start]**Data Source**: NASA Open Science Database [cite: 9]

## Operational Flow
1. [cite_start]**User Input**: Asks a question about space biology. 
2. [cite_start]**Retrieval**: System finds the relevant NASA study from the local database. [cite: 9]
3. [cite_start]**NLP Processing**: Google Gemini removes technical jargon and summarizes. [cite: 8, 9]
4. [cite_start]**Output**: User receives a simplified, accurate answer. 

## Safety
* [cite_start]**Grounded AI**: The chatbot is restricted to NASA data to prevent false info (hallucinations). [cite: 8, 9]
