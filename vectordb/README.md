# Vector Database Module

## Mục đích

Lưu trữ các vector Embedding và hỗ trợ truy vấn tìm kiếm ngữ nghĩa.

## Chức năng

- Khởi tạo ChromaDB.
- Thêm dữ liệu.
- Xóa dữ liệu.
- Truy vấn Top-k.

## Dự kiến các tệp

```
vectordb/
│
├── database.py
└── README.md
```

## Pipeline

```
Embedding
    │
    ▼
ChromaDB
    │
    ▼
Similarity Search
```
