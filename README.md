# Fintech Document Assistant

A RAG (Retrieval-Augmented Generation) service that answers questions about bank terms, fees, and policies, with every answer grounded in the source documents and cited.

## Overview

Bank customers and support teams need accurate answers from dense policy documents: terms and conditions, fee schedules, account rules. Generic AI chatbots answer from memory and hallucinate, which is unacceptable in a regulated industry. This service retrieves the relevant passages from the indexed documents first, then generates an answer grounded only in those passages, with citations back to the source. Wrong answers about fees cost money. Cited answers build trust.

## Demo / Results

*Coming as the project is built: example queries with cited answers, screenshots, retrieval evaluation results.*

## Data Sources

Public documents from three UK fintechs: Revolut, Monzo, and Wise. Terms and conditions, fee schedules, and help-centre policy pages. All publicly available, indexed locally.

## Architecture

Pipeline: **ingest → chunk → embed → store → retrieve → generate with citations**

- Document ingestion and chunking: LangChain
- Embeddings: Hugging Face sentence-transformers, run locally
- Vector store: Chroma, persistent local storage
- Generation: Anthropic API (Claude)
- Service layer: FastAPI with async endpoints, Pydantic schemas

## Concepts Demonstrated

*Filled as built.*

## Project Structure

*Filled as the modules take shape.*

## How to Run

*Filled once the service runs.*