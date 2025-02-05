# AI-Powered Chatbot for Supplier and Product Information

## Project Overview
This project is an AI-powered chatbot that allows users to query a product and supplier database using natural language. It integrates an open-source LLM for data summarization and uses the **LangGraph** framework to handle workflows.

## Tech Stack
- **Backend**: FastAPI, LangGraph, PostgreSQL, SQLAlchemy  
- **Frontend**: React, Material UI  
- **Database**: PostgreSQL  
- **LLM**: Open-source LLM (e.g., Hugging Face models)  

## Installation & Setup

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/yourusername/AI-Chatbot-Assignment.git
cd AI-Chatbot-Assignment

Set Up Backend
Install Dependencies
cd backend
pip install -r requirements.txt
uvicorn main:app --reload
Backend runs at: http://localhost:8000

Frontend Setup
cd frontend
npm install
npm start
Frontend runs at: http://localhost:3000

Database Setup
Install PostgreSQL and create the database:
CREATE DATABASE chatbot_db;
Run database migrations:
python migrate.py


API Endpoints
Chatbot Query
POST /chat/
Request Body:
{
  "query": "Show me all products under brand X"
}
Response:
{
  "response": "Here are the products under brand X..."
}

Folder Structure
AI-Chatbot-Assignment/
│── backend/
│   ├── main.py
│   ├── database.py
│   ├── requirements.txt
│── frontend/
│   ├── src/
│   ├── package.json
│── database/
│   ├── schema.sql
│── README.md

Notes
Make sure PostgreSQL is installed and running.
You can use Hugging Face transformers for LLM-based summarization.
License
This project is open-source and free to use.
