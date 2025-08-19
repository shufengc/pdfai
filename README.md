# 📄 Conversational PDF Q&A System

An AI-powered assistant that allows users to **upload PDFs** and ask natural language questions about their content.  
Built with **LangChain**, **OpenAI GPT API**, and a **full-stack React + Express.js** architecture.  

## 🚀 Features
- **PDF Upload & Processing**  
  Upload a PDF file and interact with its content through natural language queries.
- **LangChain + GPT**  
  Modular backend with document loading, chunk splitting, vector embeddings, and memory-based retrieval.
- **Conversational UI**  
  Built in **React**, supporting both **typed queries** and **voice-based interaction**.
- **Voice Interface**  
  Real-time **speech input** and **speech output** via `react-speech-recognition` and `speak-tts`.
- **Performance Optimizations**  
  Vectorized chunks cached in **Memory Vector Store**, with custom prompt templates to reduce hallucinations.

## 🛠️ Tech Stack
- **Frontend:** React, Ant Design, Axios, React-Speech-Recognition, Speak-TTS  
- **Backend:** Node.js, Express.js, Multer, LangChain, OpenAI API  
- **Other:** REST APIs, Memory Vector Store, CORS, dotenv

## 📂 Project Structure
```
pdfai/
├── server/           # Express.js backend (file upload + chat endpoints)
│   ├── server.js
│   ├── chat.js
│   └── uploads/
├── src/              # React frontend
│   ├── components/
│   │   ├── PdfUploader.js
│   │   ├── ChatComponent.js
│   │   └── RenderQA.js
│   └── App.js
└── package.json
```

## ⚡ Usage

### 1. Install Dependencies
```bash
cd pdfai
npm install
```

### 2. Run Backend
```bash
cd server
node server.js
```
Server runs at: `http://localhost:5001`

### 3. Run Frontend
```bash
cd pdfai
npm start
```
Frontend runs at: `http://localhost:3000`

### 4. How to Use
1. Open `http://localhost:3000` in your browser.  
2. Upload a PDF via the uploader.  
3. Ask questions in the input box **or** switch to **Chat Mode** and use your voice.  
4. The system responds with answers, and in voice mode it will also **speak** the answer aloud.  

## 📖 Example
- Upload: *hbs.pdf*  
- Query: “Summarize the document in three sentences.”  
- Response: *AI returns a concise summary based on document embeddings.*

## 📌 Reference
This project is **originated from Laioffer Full Stack Development Course’s “Next AI” project**, extended into a **PDF conversational assistant**.
