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

![s1](https://github.com/user-attachments/assets/0e97d2c0-2863-4df4-bd2c-c33137811d07)

### 📂 Upload Section
![s2](https://github.com/user-attachments/assets/d51933b0-ef26-41ed-a847-00da970f8226)


### 🎯 Output Screen

<img width="1357" height="859" alt="Screenshot 2026-02-28 211803" src="https://github.com/user-attachments/assets/3a91c8ea-41ee-485b-b4b1-e203cee04727" />


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
