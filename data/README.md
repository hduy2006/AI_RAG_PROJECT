# Data Directory

## Mục đích

Thư mục `data` lưu toàn bộ dữ liệu của dự án trong các giai đoạn xử lý khác nhau.

## Cấu trúc

```
data/
│
├── raw/
├── clean/
└── chunks/
```

## Mô tả

### raw/

Lưu dữ liệu gốc sau khi thu thập từ Internet.

### clean/

Lưu dữ liệu sau khi loại bỏ HTML, ký tự thừa và chuẩn hóa văn bản.

### chunks/

Lưu dữ liệu sau khi chia thành các đoạn nhỏ (Chunking) để phục vụ bước tạo Embedding.

## Luồng xử lý

```
Internet
    │
    ▼
raw
    │
    ▼
clean
    │
    ▼
chunks
```
