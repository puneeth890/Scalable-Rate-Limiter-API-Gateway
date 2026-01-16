Scalable Rate Limiter & API Gateway

A high-performance, distributed API Gateway with built-in rate limiting, designed for low latency, high concurrency, and horizontal scalability.

📌 Features

Distributed rate limiting using Token Bucket and Sliding Window algorithms

Per-user, per-endpoint, and burst-aware throttling

Low-latency API gateway optimized for high request throughput

Strong concurrency guarantees using Redis atomic operations and Lua scripts

Real-time metrics streaming via Kafka

Built for fault tolerance, high availability, and horizontal scaling

🏗️ Architecture
Client → API Gateway → Rate Limiter (Redis + Lua)
                    → Backend Services
                    → Metrics Pipeline (Kafka → Consumers)

🧠 Rate Limiting Strategies

Token Bucket – Allows bursts while maintaining average rate

Sliding Window – Precise request counting over time windows

Atomic enforcement using Redis INCR, EXPIRE, and Lua scripts to prevent race conditions

🛠️ Tech Stack

Backend: Java / Node.js (adjust if needed)

Cache & Coordination: Redis

Messaging: Kafka

Concurrency Control: Redis Lua scripts

Deployment: Docker, Kubernetes (optional)

Monitoring: Prometheus / Grafana (optional)

⚙️ Scalability & Reliability

Stateless API Gateway instances

Redis-based centralized rate enforcement

Kafka-backed metrics pipeline

Supports horizontal scaling without single points of failure

🚦 Example Use Cases

Public API protection

Abuse prevention & DDoS mitigation

SaaS multi-tenant throttling

Traffic shaping and fairness enforcement

🤖 AI-Powered Document Classification & Semantic Search Platform

An end-to-end NLP system for document classification and semantic search, built using Transformer-based language models and vector similarity search.

📌 Features

Multi-class document classification using fine-tuned Transformers

Semantic search using dense vector embeddings

Approximate Nearest Neighbor (ANN) search for low-latency retrieval

Optimized inference for production deployment

Scales to large document corpora

🧠 Model Pipeline
Documents
   ↓
Text Preprocessing
   ↓
Transformer Encoder
   ↓
Vector Embeddings
   ↓
ANN Index
   ↓
Semantic Search Results

🔍 Semantic Search

Converts documents and queries into dense embeddings

Uses ANN indexing for fast similarity search

Retrieves semantically relevant documents beyond keyword matching

🛠️ Tech Stack

ML Frameworks: PyTorch / Hugging Face Transformers

Search: FAISS / Annoy / HNSW (choose one)

Backend: Python (FastAPI)

Data Storage: Vector Store / Object Storage

Deployment: Docker

⚡ Performance Optimizations

Fine-tuned pre-trained models for task-specific accuracy

Reduced inference latency through batching and model optimization

Efficient vector indexing for large-scale retrieval

📊 Use Cases

Enterprise document search

Knowledge base retrieval

Legal / research document classification

AI-powered content discovery

📈 Future Improvements

Add authentication & API keys

Implement adaptive rate limiting

Online learning for document classification

Distributed vector search across shards

👨‍💻 Author

Puni Chowdhary
Software Engineer | Distributed Systems | Machine Learning
