# 🚀 RAG Model Simulator: Personalized Data Augmentation

This is a **single-file, client-side web application (`rag_simulator.html`)** that demonstrates the **Retrieval-Augmented Generation (RAG)** pattern.

RAG is essential for ensuring Large Language Models (LLMs) provide **factually accurate answers grounded strictly in your own private, domain-specific data**—such as internal documents, manuals, policy files, or PDFs.

The application allows users to upload their own document files (`.pdf`, `.md`, `.txt`) and query the content, simulating how an LLM retrieves and uses private data as a knowledge source.

---

## ✨ Features

### **Client-Side Document Parsing**
Uploads and extracts text from:
- **PDF files** (via PDF.js)
- **Markdown files**
- **Plain text files**

### **Two-Step RAG Process Visualization**
The UI clearly shows:
1. **Retrieval** – the exact context chunks pulled from the uploaded document  
2. **Generation** – the LLM’s final grounded answer based only on retrieved content

### **Gemini API Integration**
Uses **Gemini 2.5 Flash** for fast, contextual responses.

### **Reliability**
Implements **exponential backoff** for stable API communication.

### **Single-File HTML**
Everything lives in one HTML file—easy to deploy and runs entirely in your browser.

---

## 🛠️ Prerequisites

### **1. Gemini API Key**
Obtain a key from **Google AI Studio**.

Then open `rag_simulator.html` and update this line:

```js
const apiKey = "YOUR_ACTUAL_API_KEY_HERE";
