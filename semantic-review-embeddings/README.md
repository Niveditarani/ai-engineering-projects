## Semantic Review Analysis & Similarity Search

### Problem
E-commerce reviews contain rich feedback but are hard to 
analyze at scale using traditional keyword methods.

### Solution
Built a semantic search engine using text embeddings and a 
vector database to surface similar reviews and categorize 
feedback by topic — without any labeled training data.

### Approach
- Embedded reviews using OpenAI text-embedding-3-small
- Stored embeddings in ChromaDB for fast vector retrieval
- Applied t-SNE to visualize hidden clusters in 2D
- Cosine similarity for zero-shot topic categorization
- Similarity search returns 3 closest reviews to any input

### Tech Stack
Python · OpenAI Embeddings · ChromaDB · scikit-learn · 
t-SNE · cosine similarity · pandas · matplotlib

### Output
Categorized feedback + personalized similarity search 
ready for customer service applications
