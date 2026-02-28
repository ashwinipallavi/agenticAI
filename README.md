# agenticAI
# 🏛️ Karnataka Entrepreneur Scheme Finder

An AI-powered RAG-based Government Scheme Discovery System that helps Karnataka entrepreneurs find relevant government schemes based on their profile.

This application simplifies complex government documents and converts them into clear, structured, and easy-to-understand scheme recommendations.

---

## 🚀 Features

- 📂 Upload Government Scheme PDFs
- 🧠 Retrieval-Augmented Generation (RAG)
- 🔎 Semantic Search using Embeddings
- 📊 Profile-Based Scheme Matching
- 📄 OCR Support for Scanned PDFs
- 💾 Persistent Vector Database (ChromaDB)
- 🎯 Clean and Professional Output Format
- 🔐 Fully Offline (Runs using Ollama)

---

## 🛠️ Tech Stack

- **Frontend:** Streamlit  
- **Vector Database:** ChromaDB  
- **LLM:** phi3:mini (via Ollama)  
- **Embedding Model:** nomic-embed-text  
- **PDF Processing:** PyPDF  
- **OCR:** Tesseract  
- **Image Conversion:** pdf2image  

---

## 🧠 System Architecture

1. User uploads government scheme PDFs.
2. Text is extracted (normal extraction or OCR for scanned PDFs).
3. Text is split into overlapping chunks.
4. Chunks are converted into embeddings.
5. Stored in ChromaDB (vector database).
6. User fills entrepreneur profile form.
7. System retrieves top relevant chunks.
8. LLM generates structured scheme recommendation.

---
## 🎯 Scheme Recommendation Output
### 🏠 Home Screen
![Home Screen](C:\Users\User\Downloads\s1.jpeg)

### 📂 Upload Section
![Upload Section](C:\Users\User\Downloads\s2.jpeg)

### 🎯 Output Screen
![Output Screen](C:\Users\User\OneDrive\画像\Screenshots\Screenshot 2026-02-28 211803.png)


## 📦 Installation

### Step 1: Install Python Dependencies

```bash
pip install streamlit chromadb ollama pypdf pdf2image pytesseract
2️⃣ Install Dependencies
pip install -r requirements.txt
3️⃣ Run Ollama Models
ollama pull nomic-embed-text
ollama pull phi3:mini
4️⃣ Run the App
streamlit run filename
