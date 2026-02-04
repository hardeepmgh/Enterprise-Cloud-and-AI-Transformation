## Day 13: Local AI Integration & Vector Search

### ✅ Accomplishments:
- **Local LLM Setup:** Integrated **Ollama** as a local inference engine to handle x86_64 architecture constraints on Intel Mac.
- **Embedding Pipeline:** Successfully pulled and deployed `nomic-embed-text` to convert raw text into 768-dimensional vectors.
- **Database Schema Evolution:** Enabled `pgvector` extension in AWS RDS and provisioned a specialized schema to store high-dimensional embeddings.
- **Semantic Retrieval:** Developed a Python search script using the `<=>` (Cosine Distance) operator to perform meaning-based queries rather than simple keyword matches.
- **Cross-Platform Bridge:** Established a functional "Local Brain / Cloud Memory" architecture.

### 🛠️ Tech Stack:
- **Ollama** (Local Model Hosting)
- **Llama3 / Nomic-Embed-Text** (Models)
- **AWS RDS PostgreSQL** (Vector Store)
- **psycopg2** (Database Adapter)

### 📈 Current Status:
Successfully retrieved contextually relevant IT manual data from AWS using local embeddings. The "Retrieval" part of RAG is now 100% operational.
