# Corrective RAG Agent

A sophisticated Retrieval-Augmented Generation (RAG) agent that implements an intelligent document analysis system with web search capabilities and self-correcting mechanisms.

## Features

- **Multi-Source Document Processing**
  - Support for PDF, TXT, and MD files
  - URL-based document loading
  - Web content retrieval

- **Advanced RAG Pipeline**
  - Document chunking with RecursiveCharacterTextSplitter
  - Vector storage using Qdrant
  - Relevance assessment and filtering
  - Automated web search for information augmentation
  - Query transformation for enhanced retrieval

- **LLM Integration**
  - Claude 3.5 Sonnet integration for high-quality responses
  - OpenAI embeddings for document vectorization
  - Intelligent response generation with context awareness

- **Reliability Features**
  - Retry mechanism for web searches
  - Error handling and graceful degradation
  - Progress tracking and user feedback
  - Session state management
 
## Architecture

The application follows a graph-based workflow:
1. Document Retrieval
2. Relevance Assessment
3. Query Transformation (if needed)
4. Web Search (if required)
5. Response Generation

## Prerequisites

- Python 3.8+
- Streamlit
- Required API Keys:
  - Anthropic API key (Claude)
  - OpenAI API key
  - Tavily API key (for web search)
  - Qdrant API key and URL

## Installation

```bash
pip install streamlit langchain langgraph qdrant-client openai anthropic tavily-python
```

## Environment Setup

Configure the following API keys in the application:
- `ANTHROPIC_API_KEY`
- `OPENAI_API_KEY`
- `TAVILY_API_KEY`
- `QDRANT_API_KEY`
- `QDRANT_URL`

## Usage

1. Start the application:
```bash
streamlit run app.py
```

2. Configure API keys in the sidebar
3. Choose input method (URL or File Upload)
4. Enter your question
5. View the step-by-step processing and final response



