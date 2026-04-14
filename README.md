
# Underwriting Docs RAG

![Demo Screenshot](demo/screenshot.png)

## Overview
Search underwriting manuals, exceptions, and policy notes with grounded answers for reviewers.

This project is part of a 50-project portfolio covering data science, AI, LLM, RAG, and product analytics use cases across finance, health, retail, cybersecurity, developer tools, and enterprise workflows.

## Project Profile
- Domain: Insurtech
- Project type: `rag`
- Tags: insurance, rag, docs

## Quick Start
```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python scripts/bootstrap_data.py
uvicorn src.app.main:app --host 0.0.0.0 --port 8000 --reload
```

Open `http://localhost:8000/` to use the interactive application.

## Key Endpoints
- `GET /`
- `GET /health`
- `GET /bootstrap`
- `GET /project`
- `POST /score`
- `POST /analyze`
- `POST /query`
- `POST /recommend`

## Structure
```text
underwriting-docs-rag/
|- configs/
|- data/
|- demo/
|- docs/
|- scripts/
|- src/app/
|- src/app/web/
|- tests/
|- .github/workflows/
|- Dockerfile
|- docker-compose.yml
|- Makefile
```
