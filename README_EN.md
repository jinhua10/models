# Please download the model compressed package from the Release page and store it in the release/models directory.

**Language**: [English](README_EN.md) | [中文](README.md)

---

## 📦 Directory Structure

```
release/
├── ai-reviewer-base-file-rag-2.0-jar-with-dependencies.jar  # Main Application
├── config/                                                   # Configuration
│   └── application.yml                                      # Main Config File
├── data/                                                    # Data Directory
│   ├── documents/                                          # Document Storage (User Uploads)
│   ├── knowledge-base/                                     # Knowledge Base Data
│   │   ├── cache/                                         # Cache Directory
│   │   ├── documents/                                     # Documents (Date-based)
│   │   ├── index/                                         # Lucene Index
│   │   │   └── lucene-index/                             # Index Files
│   │   └── metadata/                                      # Metadata
│   │       └── metadata.db                               # Metadata Database
│   ├── rag/                                               # RAG Retrieval Data
│   │   ├── cache/                                        # RAG Cache
│   │   ├── documents/                                    # RAG Documents
│   │   ├── index/                                        # RAG Index
│   │   │   └── lucene-index/                            # Lucene Index
│   │   └── metadata/                                     # RAG Metadata
│   │       └── metadata.db                              # Metadata DB
│   ├── vector-index/                                      # Vector Index
│   │   └── vector-index/                                 # Vector Data
│   │       └── vectors.dat                              # Vector File
│   ├── feedback/                                          # User Feedback (Runtime)
│   ├── llm-results/                                       # LLM Analysis Results (Runtime)
│   ├── qa-records/                                        # QA Records (Runtime)
│   └── hope/                                              # HOPE 3-Layer Memory (Runtime)
│       ├── permanent/                                     # Low-freq Layer - Permanent
│       ├── ordinary/                                      # Mid-freq Layer - Recent
│       └── high-frequency/                                # High-freq Layer - Real-time (Memory)
├── models/                                                  # AI Model Files
│   ├── bge-base-zh/                                        # Vector Model (Built-in)
│   └── qwen2.5-0.5b-instruct/                             # PPL Model (Optional)
├── logs/                                                    # Log Directory
├── temp/                                                    # Temporary Files
├── scripts/                                                 # Utility Scripts
│   ├── download_embedding_model.py                         # Download Vector Model
│   ├── download_qwen_onnx.py                              # Download PPL Model
│   └── convert_bge_to_onnx.py                             # Convert BGE to ONNX
├── start.bat                                                # Windows Startup Script
├── stop.bat                                                 # Windows Stop Script
├── fix-lock.bat                                            # Fix Port Occupation
├── PROMPT_QUICK_START.md                                   # Prompt Config Guide (CN)
├── PROMPT_TEMPLATE_CONFIG_EN.md                            # Prompt Config Guide (EN)
└── jdk download.txt                                        # JDK Download Links
```

