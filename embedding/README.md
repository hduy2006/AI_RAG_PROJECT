# Embedding Module

## Mục đích

Chuyển mỗi đoạn văn bản thành một vector số để phục vụ tìm kiếm ngữ nghĩa.

## Chức năng

- Tải mô hình Embedding.
- Sinh vector cho từng Chunk.
- Lưu vector để đưa vào Vector Database.

## Dự kiến các tệp

```
embedding/
│
├── embedding.py
└── README.md
```

## Pipeline

Chunk
│
▼
Embedding Model
│
▼
Vector

## Mô hình dự kiến

- BAAI/bge-m3
- sentence-transformers
