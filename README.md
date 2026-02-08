# 📘 Endee Academic AI Assistant

An **extraction‑first Academic Question Answering system** built on top of **Endee (Vector Database)**.

This project allows a user to **upload any academic PDF (including scanned PDFs)** and ask questions. The system **extracts answers directly from the document** — preserving structure, order, numbering, and exam‑ready formatting.

No hallucinations. No raw vectors shown to the user. Just clean answers.

---

## 🚀 Why This Project Stands Out

Most PDF‑QA projects *generate* answers loosely. This project is different:

✔ Uses **OCR for scanned PDFs**
✔ Uses **semantic retrieval (vectors)** for relevance
✔ **Restores original document order** before answering
✔ Fixes broken numbering, spacing, and formatting
✔ Produces **exam‑ready, readable answers**

This is ideal for:

* Engineering notes
* University exam preparation
* Research PDFs
* Technical documentation

---

## 🧠 Architecture Overview

```
PDF (Scanned / Digital)
        ↓
OCR (Tesseract + PyMuPDF)
        ↓
Text Chunking (structure‑aware)
        ↓
Embeddings (Sentence Transformers)
        ↓
Endee / FAISS Vector Index
        ↓
Semantic Retrieval (TOP‑K)
        ↓
Document Order Restoration
        ↓
Clean, Structured Answer
```

---

## 🛠 Tech Stack

| Layer      | Technology                     |
| ---------- | ------------------------------ |
| UI         | Streamlit                      |
| OCR        | PyMuPDF + Tesseract            |
| Embeddings | Sentence‑Transformers (MiniLM) |
| Vector DB  | Endee / FAISS                  |
| Language   | Python                         |

---

## ✨ Key Features

* 📄 Upload **any PDF** (scanned or digital)
* 🔍 OCR‑based text extraction
* 🧠 Semantic question answering
* 📑 Restores **original ordering** of content
* 🧾 Handles bullet points, numbered lists, paragraphs
* 🎓 Exam‑oriented output formatting
* 🌙 Clean dark‑mode UI

---

## 🖥️ User Interface Flow

1. Upload academic PDF
2. Wait for indexing confirmation
3. Type a question (example: *Explain non traditional machining*)
4. Get a **clean extracted answer**, not vectors

---

## 📦 Installation

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/<your-username>/Endee-Academic-AI-Assistant.git
cd Endee-Academic-AI-Assistant
```

### 2️⃣ Create Virtual Environment

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Install Tesseract (Required for OCR)

**macOS**

```bash
brew install tesseract
```

**Ubuntu**

```bash
sudo apt install tesseract-ocr
```

---

## ▶️ Run the App

```bash
streamlit run app.py
```

Open browser at:

```
http://localhost:8501
```

---

## 📁 Project Structure

```
Endee-Academic-AI-Assistant/
│
├── app.py                # Main application
├── requirements.txt      # Python dependencies
├── README.md             # Project documentation
├── data/                 # Sample PDFs
└── venv/                 # Virtual environment
```

---

## 🧪 Example Questions

* What is non traditional machining?
* Explain ultrasonic machining
* List advantages of AJM
* What is the function of power supply in USM?

---

## 🏆 Suitable For

* Academic competitions
* Vector database demonstrations
* AI + NLP coursework
* Resume & portfolio projects

---

## 🔮 Future Enhancements

* Diagram image display alongside text
* Table reconstruction from PDFs
* Multi‑PDF knowledge base
* Export answers as notes

---

## 👩‍💻 Author

**Venna Satya Varsha Sri**
Academic AI Project using Endee Vector Database

---

## ⭐ If You Like This Project

Give it a star ⭐ and use it to ace your exams 📚

---

> *This project demonstrates practical, real‑world use of vector databases for structured knowledge extraction
