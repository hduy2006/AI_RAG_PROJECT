# Crawler Module

## Mục đích

Module `crawler` chịu trách nhiệm thu thập dữ liệu từ các website trên Internet để xây dựng kho tri thức cho hệ thống RAG.

## Chức năng

- Đọc danh sách URL từ `urls.txt`.
- Gửi yêu cầu HTTP đến từng website.
- Tải nội dung HTML.
- Trích xuất nội dung văn bản.
- Lưu dữ liệu vào thư mục `data/raw/`.

## Cấu trúc

```
crawler/
│
├── crawl.py      # Chương trình chính
├── parser.py     # Phân tích HTML
├── save.py       # Lưu dữ liệu
├── urls.txt      # Danh sách website
└── README.md
```

## Luồng xử lý

```
URL
 │
 ▼
Download HTML
 │
 ▼
BeautifulSoup
 │
 ▼
Extract Text
 │
 ▼
Save TXT
```

## Kết quả

Sau khi chạy module này, dữ liệu sẽ được lưu trong:

```
data/raw/
```
