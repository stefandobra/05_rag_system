# CLAUDE.md

## Project

Fintech Document Assistant — a RAG service answering questions about bank terms, fees, and policies with cited, document-grounded answers. Part of an 8-project portfolio; this is project 5.

## Working Rules

- Stefan writes all code. Assist, suggest, review — never write whole files unprompted.
- Type hints on all functions.
- Comments explain WHY (decisions), not WHAT (restating code).
- Service-layer pattern: each module has one job and clean input/output contracts.

## Stack

- Python 3.12, venv
- LangChain (orchestration), sentence-transformers (local embeddings), Chroma (persistent vector store)
- FastAPI with async endpoints, Pydantic v2 schemas
- Anthropic API, claude-sonnet-4-6, for generation

## Git Conventions

- Conventional commits: feat:/fix:/docs:/chore:, lowercase, present tense, under ~50 chars
- One logical change per commit
- Branch prefixes: feature/, fix/, docs/, chore/. Always branch off latest main. Nothing lands on main directly — PR only.
- git status first, then git add -A. Never blind git add .

## Dependencies

- requirements.txt: pinned core dependencies
- requirements-dev.txt: full pip freeze
- Both updated in the same commit as the install that changed them

## Architecture

*Added as modules are built.*