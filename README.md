# LLM Chatbot with Persistent Memory

A production-ready conversational AI backend featuring stateful conversation history, session-based context memory, and structured schema validation. Built with FastAPI, SQLAlchemy, and LLM orchestration.

---

## 📌 Features

- **Contextual Conversation Memory:** Tracks multi-turn dialogue history per session for coherent long-term interactions.
- **Persistent Storage:** Backs conversation state and message threads in a relational database using SQLAlchemy models.
- **Strict Data Validation:** Enforces request/response contracts using Pydantic schemas.
- **Modular Architecture:** Clean separation of concerns between API routing, LLM reasoning logic, and database operations.
- **Async Execution:** Fast, non-blocking API endpoints designed to handle high concurrency.

---

## 🏗️ Architecture & Project Structure

```text
llm-chatbot-memory/
├── main.py          # FastAPI application initialization and API endpoints
├── llma.py          # LLM orchestration, prompt handling, and memory integration
├── db.py            # Database configuration, engine setup, and ORM models
├── schema.py        # Pydantic data schemas for request/response validation
├── requirements.txt # Python dependencies
└── README.md        # Project documentation
