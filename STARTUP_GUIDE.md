# DocuSight: Companion AI — Startup Guide

**Author**: Rishi Sheladiya | **College ID**: 23CE132 | **GitHub**: rishi-sheladiya-26

This guide explains how to start the FastAPI backend and React frontend.

## Prerequisites

Before starting, ensure you have:

1. **MongoDB Atlas**: Already configured in `.env` (cloud-hosted, no local install needed)
2. **ChromaDB**: The vector database for document embeddings.
   - Run via Docker: `docker run -d -p 8001:8000 chromadb/chroma:latest`
   - Or install via pip: `pip install chromadb` and run locally
3. **Google Gemini API Key**: Already configured in `.env`

---

## Step 1: Backend Setup

1. Navigate to the backend directory:
   ```powershell
   cd backend
   ```

2. Create a virtual environment (recommended):
   ```powershell
   python -m venv venv
   .\venv\Scripts\activate
   ```

3. Install dependencies:
   ```powershell
   pip install -r requirements.txt
   ```

4. The `.env` file is already configured with:
   - ✅ MongoDB Atlas connection string
   - ✅ Google Gemini API key
   - ✅ ChromaDB settings

---

## Step 2: Run the Backend

```powershell
uvicorn app.main:app --reload --host 0.0.0.0 --port 8000
```

- **--reload**: Enables auto-reload on code changes
- **--host 0.0.0.0**: Makes the server accessible from other devices
- **--port 8000**: Runs on port 8000

---

## Step 3: Frontend Setup

Open a new terminal:

```powershell
cd frontend
npm install
npm start
```

---

## Step 4: Access the Application

- **Frontend**: http://localhost:3000
- **API Documentation**: http://localhost:8000/docs
- **Health Check**: http://localhost:8000/api/v1/health

---

## Troubleshooting

- **MongoDB Connection Error**: Check that your Atlas cluster is running and the IP is whitelisted in Atlas Network Access.
- **ChromaDB Connection Error**: Ensure ChromaDB is running on port 8001.
- **Gemini API Error**: Verify the `GOOGLE_API_KEY` in `backend/.env` is correct.
- **Frontend can't connect**: Verify backend is on port 8000 and CORS is configured.
