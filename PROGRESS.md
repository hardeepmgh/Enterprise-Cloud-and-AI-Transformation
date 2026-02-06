# 🤖 Cloud-Native IT Support RAG Assistant
**A Full-Stack AI Application leveraging AWS RDS (pgvector) and Local LLMs.**

## 🌟 Overview
This project is a Retrieval-Augmented Generation (RAG) system designed to serve as an automated IT Support Desk. It combines high-performance cloud infrastructure with local AI inference to provide secure, context-aware answers from a corporate knowledge base.

## 🏗️ Architecture
The system follows a modern RAG pattern:
1.  **Frontend:** Streamlit web interface for real-time user interaction.
2.  **Orchestration:** Python (Psycopg2, Ollama SDK).
3.  **Vector Database:** Amazon RDS PostgreSQL with the `pgvector` extension.
4.  **Local LLM:** - **Embeddings:** `nomic-embed-text` via Ollama.
    - **Generation:** `Llama 2` (or `Phi-3`) via Ollama.
5.  **Infrastructure:** Managed via Terraform (IaC).



## 🛠️ Tech Stack
- **Cloud:** AWS (RDS, VPC, Security Groups)
- **IaC:** Terraform
- **AI/ML:** Ollama, pgvector
- **Language:** Python 3.9+
- **UI:** Streamlit

## 🚀 Key Features
- **Contextual Accuracy:** Uses vector similarity search (`<=>` cosine distance) to retrieve exact manual snippets.
- **Local Inference:** Keeps processing costs low by running the LLM locally while offloading data storage to the cloud.
- **Traceability:** Includes a "View Source Knowledge" feature to show the raw data used for every AI response.
- **Security:** Infrastructure locked down via VPC Security Groups and SSL-encrypted database connections.

## 📈 Milestone Progress
- [x] **Week 1:** Cloud Infrastructure setup via Terraform.
- [x] **Week 2:** Vector Database configuration and data ingestion.
- [x] **Week 3:** RAG Pipeline integration and Streamlit UI deployment.

## 🛠️ Installation & Usage
1. **Provision Infrastructure:** `terraform apply`
2. **Ingest Data:** `python3 init_db.py && python3 smart_ingest.py`
3. **Run App:** `python3 -m streamlit run app.py`
