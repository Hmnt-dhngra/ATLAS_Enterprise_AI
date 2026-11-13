# ATLAS Enterprise AI

A full-stack enterprise AI project focused on building a Retrieval-Augmented Generation (RAG) application with infrastructure, AI orchestration, application layers, and end-to-end integration.

## Overview

This repository is organized into four core phases:

1. Infrastructure setup for environment configuration, PostgreSQL, AWS, and Pinecone
2. AI engineering for RAG, memory, guardrails, observability, human-in-the-loop workflows, and LangGraph orchestration
3. Full-stack application development using API, HTML, CSS, and JavaScript
4. Integration and testing, including S3 CORS, automated tests, documentation, and demo validation

## Tech Stack

- Python 3.12
- FastAPI
- PostgreSQL
- AWS services
- Pinecone vector database
- LangGraph
- Jinja2 + JavaScript frontend
- Pydantic settings and environment-based configuration

## Quick Start

### 1) Initialize the environment

```bash
uv init --python 3.12
uv python pin
uv venv .venv
.venv\Scripts\activate
uv add -r requirements.txt
```

### 2) Create the project structure

```bash
python create_structure.py
```

### 3) Run the app

```bash
uvicorn app.main:app --reload
```

## Project Structure

```text
ATLAS_Enterprise_AI/
├── app/
│   ├── __init__.py
│   ├── aws.py
│   ├── config.py
│   ├── db.py
│   ├── graph.py
│   ├── guardrails.py
│   ├── main.py
│   ├── memory.py
│   ├── observability.py
│   ├── rag.py
│   ├── vector.py
│   ├── static/
│   └── templates/
├── docs/
│   └── SETUP.md
├── infra/
│   └── schema.sql
├── scripts/
│   └── init_db.py
├── worker/
│   └── ingest.py
├── README.md
├── create_structure.py
├── main.py
├── pyproject.toml
├── requirements.txt
├── uv.lock
├── LICENSE
└── .venv/
```

## Roadmap

### Phase 1 — Infrastructure
- Set up development environment
- Configure PostgreSQL and cloud services
- Connect AWS and Pinecone resources

### Phase 2 — AI Engineering
- Build retrieval and document processing pipelines
- Add memory and guardrails
- Integrate observability and human oversight
- Orchestrate multi-step workflows with LangGraph

### Phase 3 — Full-Stack Application
- Expose APIs with FastAPI
- Build frontend interface with HTML, CSS, and JavaScript
- Connect UI to AI workflows and document retrieval

### Phase 4 — Integration & Testing
- Validate service interactions
- Configure S3 CORS and secure integrations
- Add tests and documentation
- Demonstrate the end-to-end system

## Notes

This README is intended as a project entry point and roadmap. As the project evolves, you can expand it with:

- architecture diagrams
- environment variable examples
- API usage examples
- deployment instructions
- testing commands and screenshots

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
