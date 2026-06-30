# 🤖 AI-RAG-Project

> Xây dựng hệ thống hỏi đáp thông minh về Trí tuệ nhân tạo sử dụng Retrieval-Augmented Generation (RAG)

## Giới thiệu

Đây là dự án đồ án môn học Trí tuệ nhân tạo nhằm xây dựng một hệ thống hỏi đáp sử dụng kỹ thuật **Retrieval-Augmented Generation (RAG)**. Hệ thống có khả năng thu thập dữ liệu từ Internet, xử lý dữ liệu, lưu trữ vào cơ sở dữ liệu vector và sử dụng mô hình ngôn ngữ lớn (LLM) để tạo ra câu trả lời chính xác dựa trên nguồn tài liệu.

Dự án được phát triển theo từng giai đoạn. Mỗi phần đều có mã nguồn, tài liệu và lịch sử commit rõ ràng.

---

# Lộ trình phát triển

- [x] Phần 1: Chuẩn bị môi trường và cấu trúc dự án
- [ ] Phần 2: Thu thập dữ liệu từ Internet
- [ ] Phần 3: Tiền xử lý dữ liệu
- [ ] Phần 4: Chunking
- [ ] Phần 5: Sinh Embedding
- [ ] Phần 6: Xây dựng Vector Database
- [ ] Phần 7: Semantic Search
- [ ] Phần 8: Xây dựng Pipeline RAG
- [ ] Phần 9: Tích hợp LLM
- [ ] Phần 10: Giao diện người dùng
- [ ] Phần 11: Đánh giá hệ thống

---

# PHẦN 1 - Chuẩn bị môi trường

## Mục tiêu

Chuẩn bị đầy đủ môi trường phát triển trước khi xây dựng hệ thống RAG.

Sau khi hoàn thành phần này, dự án sẽ có:

- Môi trường Python riêng (Virtual Environment)
- Các thư viện cần thiết
- Cấu trúc thư mục chuẩn
- Chương trình đầu tiên chạy thành công

---

## Bước 1. Cài đặt Python

Khuyến nghị sử dụng:

- Python 3.11

Kiểm tra phiên bản:

```bash
python --version
```

Nếu chưa có Python, hãy cài đặt trước rồi tiếp tục.

---

## Bước 2. Tạo thư mục dự án

```
AI_RAG_Project/
```

Sau đó tạo cấu trúc:

```
AI_RAG_Project/
│
├── app.py
├── requirements.txt
├── README.md
│
├── data/
│   ├── raw/
│   ├── clean/
│   └── chunks/
│
├── crawler/
├── preprocess/
├── embedding/
├── vectordb/
├── rag/
├── evaluation/
├── models/
└── ui/
```

### Ý nghĩa từng thư mục

### data/

Lưu toàn bộ dữ liệu của hệ thống.

- raw/: dữ liệu vừa thu thập.
- clean/: dữ liệu đã làm sạch.
- chunks/: dữ liệu sau khi chia đoạn.

---

### crawler/

Chứa chương trình crawl dữ liệu từ Internet.

Ví dụ:

- crawl.py
- download.py

---

### preprocess/

Các bước tiền xử lý dữ liệu.

Ví dụ:

- clean_text.py
- normalize.py
- chunk.py

---

### embedding/

Sinh vector embedding.

Ví dụ:

- embedding.py

---

### vectordb/

Quản lý ChromaDB.

Ví dụ:

- database.py

---

### rag/

Pipeline của hệ thống.

Ví dụ:

- retriever.py
- generator.py
- prompt.py

---

### evaluation/

Lưu bộ dữ liệu đánh giá và các chương trình tính toán Accuracy, Precision, Recall,...

---

### models/

Lưu mô hình AI nếu sử dụng cục bộ.

---

### ui/

Giao diện Streamlit.

---

## Bước 3. Tạo Virtual Environment

Windows

```bash
python -m venv venv
```

Linux/macOS

```bash
python3 -m venv venv
```

---

## Bước 4. Kích hoạt Virtual Environment

Windows

```bash
venv\Scripts\activate
```

Linux/macOS

```bash
source venv/bin/activate
```

Nếu thành công sẽ xuất hiện:

```
(venv)
```

---

## Bước 5. Cài đặt thư viện

Tạo file requirements.txt

```
langchain
langchain-community
langchain-text-splitters

chromadb

sentence-transformers

beautifulsoup4

requests

streamlit

ollama

pandas

numpy

tqdm

lxml
```

Cài đặt:

```bash
pip install -r requirements.txt
```

---

## Bước 6. Kiểm tra môi trường

Tạo file

```
test_import.py
```

Import toàn bộ thư viện.

Nếu chương trình chạy không báo lỗi thì môi trường đã sẵn sàng.

---

## Bước 7. Tạo chương trình đầu tiên

Tạo file

```
app.py
```

Viết chương trình Python đầu tiên để kiểm tra cấu trúc dự án.

---

# Kết quả đạt được

Sau phần này dự án đã có:

- Cấu trúc thư mục hoàn chỉnh
- Python Environment
- Các thư viện AI
- Mã nguồn ban đầu

Đây là nền tảng để bước sang giai đoạn thu thập dữ liệu.

---

# Commit đề xuất

```
feat: initialize AI RAG project structure

- Create project structure
- Add virtual environment guide
- Add requirements.txt
- Initialize README
```

---

# Công nghệ sử dụng

- Python
- LangChain
- ChromaDB
- Sentence Transformers
- Ollama
- Streamlit
- Git
- GitHub

---

# Tác giả

Sinh viên: ...

Môn học: Trí tuệ nhân tạo

Năm học: ...
