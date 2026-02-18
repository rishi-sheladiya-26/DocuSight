# DocuSight: Companion AI for Documents

An AI-powered chatbot system for intelligent document troubleshooting and assistance using RAG (Retrieval Augmented Generation) technology.

## 👨‍💻 Author

- **Name**: Rishi Sheladiya
- **College ID**: 23CE132
- **GitHub**: [rishi-sheladiya-26](https://github.com/rishi-sheladiya-26)
- **Project**: DocuSight — Companion AI for Documents

## 🎯 System Overview

This application helps users get answers from their documents by:
- Answering queries in plain language
- Searching through uploaded documents and manuals
- Providing step-by-step instructions with source citations
- Supporting multiple document types (PDF, HTML, Text)

## 🏗️ Architecture

### Technology Stack
- **Frontend**: React.js with custom CSS
- **Backend**: FastAPI (Python)
- **AI/ML**: LangChain + RAG
- **Vector Database**: ChromaDB
- **LLM**: Google Gemini
- **Database**: MongoDB Atlas

### Components
1. **User Interface Layer** - React-based chat interface
2. **API Gateway** - FastAPI REST endpoints
3. **Document Processing Pipeline** - PDF/HTML/Text ingestion
4. **Vector Database** - Embeddings storage with metadata
5. **RAG Retrieval System** - Semantic search and ranking
6. **LLM Integration** - Response generation with citations (Google Gemini)

## 📁 Project Structure

```
DocuSight/Companion-AI/
├── frontend/                 # React application
│   ├── src/
│   │   ├── components/      # UI components
│   │   ├── services/        # API integration
│   │   └── utils/           # Helper functions
│   └── package.json
├── backend/                  # FastAPI application
│   ├── app/
│   │   ├── api/             # API endpoints
│   │   ├── core/            # Configuration
│   │   ├── models/          # Data models
│   │   ├── services/        # Business logic
│   │   └── rag/             # RAG implementation
│   └── requirements.txt
├── docs/                     # Documentation
└── README.md
```

## 🚀 Quick Start

### Prerequisites
- Node.js 18+
- Python 3.10+
- Google Gemini API key
- MongoDB Atlas account

### Installation

1. Clone the repository
2. Set up environment variables (see `STARTUP_GUIDE.md`)
3. Install dependencies
4. Run the backend and frontend

See detailed instructions in `STARTUP_GUIDE.md`

## 📊 Performance Targets

- **Concurrent Users**: 1000+
- **Response Time**: < 3 seconds
- **Supported Formats**: PDF, HTML, Text
- **Uptime**: 99.9%

## 📖 Documentation

- [System Architecture](docs/architecture.md)
- [API Documentation](docs/api.md)
- [Frontend Guide](docs/frontend.md)
- [RAG Implementation](docs/rag.md)
- [Data Preparation](docs/data-preparation.md)

## 🔒 Security

- JWT authentication
- Rate limiting (100 req/min per user)
- CORS configuration
- Input validation
- API key encryption

## 📝 License

MIT License — Rishi Sheladiya, 2025