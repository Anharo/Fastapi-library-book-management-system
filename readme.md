# 📚 Library Management API (FastAPI)

A simple yet powerful Library Management System built using **FastAPI**.
This project demonstrates core backend concepts like CRUD operations, filtering, searching, sorting, pagination, queue handling, and borrow/return workflows.

---

## 🚀 Features

* 📖 Manage Books (Create, Read, Update, Delete)
* 🔍 Search books by title or author
* 🎯 Filter books by genre, author, availability
* 🔽 Sort books (title, author, genre)
* 📄 Pagination support
* 📦 Borrow & Return system
* ⏳ Queue system for unavailable books
* 🔁 Auto re-assign book to next user in queue
* 📊 Summary & analytics endpoints
* 👤 Borrow records with search & pagination

---

## 🛠️ Tech Stack

* **Python**
* **FastAPI**
* **Uvicorn**

---

## 📂 Project Setup

### 1. Clone the repository

```bash
git clone https://github.com/Anharo/fastapi-library-system.git
```

---

### 2. Create virtual environment

```bash
python -m venv venv
```

Activate:

* Windows:

```bash
venv\Scripts\activate
```

* Mac/Linux:

```bash
source venv/bin/activate
```

---

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

---

### 4. Run the server

```bash
uvicorn main:app --reload
```

---

## 🌐 API Docs

* Swagger UI: http://127.0.0.1:8000/docs
* ReDoc: http://127.0.0.1:8000/redoc

---

## 📌 Main Endpoints

### 📚 Books

* `GET /books` → Get all books
* `POST /books` → Add new book
* `PUT /books/{book_id}` → Update book
* `DELETE /books/{book_id}` → Delete book

### 🔍 Search & Filter

* `GET /books/search?keyword=...`
* `GET /books/filter?...`
* `GET /books/sort?...`
* `GET /books/page?...`
* `GET /books/browse?...`

### 📦 Borrow System

* `POST /borrow` → Borrow a book
* `POST /return/{book_id}` → Return a book

### ⏳ Queue System

* `POST /queue/add` → Join waitlist
* `GET /queue` → View queue

### 📊 Borrow Records

* `GET /borrow-records/search?...`
* `GET /borrow-records/page?...`

---

## 🧠 Concepts Covered

* REST API Design
* Data validation (Pydantic)
* Query parameters & filtering
* Pagination & sorting
* Business logic implementation
* Error handling
* In-memory data structures

---

## 🚀 Future Improvements

* Database integration (SQLite/PostgreSQL)
* Authentication (JWT)
* User roles (Admin/User)
* Fine calculation system
* Notifications for queue users

---

## 👨‍💻 Author

**Anish Sharma**

---

## ⭐ Show your support

If you like this project, give it a ⭐ on GitHub!
