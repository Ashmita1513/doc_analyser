# Doc_Analyser

Autonomous Document Processing & Compliance Agent
🚀 Overview

An AI-powered decision intelligence system that automates the processing, validation, and verification of business documents such as invoices, purchase orders, and delivery receipts.

Unlike traditional OCR systems that only extract text, this solution understands, verifies, detects anomalies, and makes intelligent decisions using risk-based analysis.

🎯 Problem Statement

Businesses face several challenges in handling documents:

Manual verification is time-consuming and error-prone
Fraudulent or duplicate invoices go undetected
Lack of cross-document validation (Invoice vs PO vs Receipt)
No real-time risk assessment Existing OCR systems only extract data — they don’t analyze or decide

💡 Solution

This project introduces an AI-powered autonomous agent that transforms document processing into an intelligent workflow system.

Key capabilities:
📄 Extracts structured data using OCR + NLP
🔗 Links related documents (Invoice ↔ PO ↔ Delivery Receipt)
✅ Performs validation checks (field, arithmetic, cross-document)
🚨 Detects fraud and anomalies
📊 Assigns risk scores (0–100)
⚡ Recommends actions:
Approve
Reject
Manual Review
Request Correction

This system not only assists but actively supports decision-making in real-world business operations.

 Core Features
Document ingestion (PDFs, images, scanned files)
Intelligent data extraction (fields + tables)
Cross-document linking
Validation engine
Fraud detection system
Risk scoring mechanism
Explanation engine (reasoning for decisions)
Action recommendation system
⚙️ Tech Stack
🔹 Backend
Python
FastAPI
🔹 AI / ML
Tesseract OCR
HuggingFace Transformers
LayoutLM (optional for document understanding)
🔹 Data Processing
Pandas
Regex
🔹 Frontend
React / Next.js / Streamlit
🔹 Database
SQLite / MongoDB
🔹 DevOps
Docker
▶️ How to Run
1. Clone the Repository
git clone <your-repo-link>
cd doc_analyzer
2. Backend Setup
cd backend
pip install -r requirements.txt

Run the backend server:

uvicorn app.main:app --reload

Server will start at:

http://localhost:8000
3. Frontend Setup
cd frontend
npm install
npm run dev

Frontend will run at:

http://localhost:3000
4. Using Docker (Optional)

Build the container:

docker build -t doc-ai .

Run the container:

docker run -p 8000:8000 doc-ai
🌐 API Overview

Base URL:

/api/v1

Sample endpoints:

POST /upload → Upload document
GET /documents → Fetch all documents
POST /validate → Validate document
GET /risk/{id} → Get risk score
⚠️ Error Logging
Centralized logging system implemented
Logs stored for:
API errors
Validation failures
System exceptions
🔐 Security
JWT-based authentication
Secure API handling
Sensitive data protection
📊 Sample Output
Risk Level: HIGH (82/100)

Issues:
- Quantity mismatch
- Missing GST number
- Duplicate invoice

Recommended Action:
- Manual verification
- Request correction
🔥 Unique Selling Points
Beyond OCR → Full decision intelligence system
Multi-document understanding
Risk-based automation
Explainable AI
Real-world business application
🔮 Future Enhancements
Real-time API integrations
Advanced ML anomaly detection
Conversational AI interface
Self-learning rule engine
🏁 Conclusion

This project is not just a document processing tool —
it is an AI-powered compliance and decision engine designed to make business workflows faster, smarter, and more reliable.
