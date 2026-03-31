## CUxITMO (OKKO video-rag) solution.

* HyDE
* Hypothetical Document Embedding - generates transcript-like responses to bridge semantic gap
Topic Filtering
BERT-based classifier narrows search space to relevant topics
LoRA Fine-tuned Embeddings
Qwen3-Embedding-0.6B with custom fine-tuning for video domain
Multi-scale Chunking
60s transcript chunks with 10s overlap
Synthetic Chunks
QA pairs from training data as additional retrieval corpus
Cross-Encoder Reranking
BGE-Reranker-v2-m3 for final relevance scoring
IoU Deduplication
Removes overlapping video segments from results
