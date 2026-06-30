# RAG Module

## Mục đích

Đây là module trung tâm của dự án, chịu trách nhiệm xây dựng quy trình Retrieval-Augmented Generation (RAG).

## Chức năng

- Tiếp nhận câu hỏi.
- Truy vấn Vector Database.
- Lấy Top-k tài liệu liên quan.
- Tạo Prompt.
- Gửi đến LLM.
- Sinh câu trả lời.

## Dự kiến các tệp

```
rag/
│
├── retriever.py
├── prompt.py
├── generator.py
└── README.md
```

## Pipeline

```
Question
    │
    ▼
Retriever
    │
    ▼
Top-k Documents
    │
    ▼
Prompt
    │
    ▼
LLM
    │
    ▼
Answer
```
