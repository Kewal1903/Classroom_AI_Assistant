# 🧠 AI Notes Generator + RAG Study Assistant

This project provides a full-stack pipeline to automatically generate smart, exam-ready notes from educational videos (e.g., lectures, tutorials) and enables students to interact with the generated content through a conversational AI assistant.  

Built using Whisper, LLaMA, GPT-4.1, and Gemini 1.5, the system supports automated note-taking and retrieval-augmented question-answering.

---

## 🚀 Features

### 1. 🎥 YouTube Video/Local File Input
- Accepts a **YouTube video link** or **uploaded `.mp4`/`.wav` file** as input.
- Accepts an OpenAI token (from GitHub Marketplace) for accessing models such as **GPT 4.1** and **Meta Llama 4**
- Uses Whisper small (OpenVINO Optimized) to transcribe audio into high-quality text.

### 2. ✂️ Smart Chunking & Topic Identification
- Segments the transcript into meaningful chunks using a smart chunking algorithm.
- Topics are identified using LLaMA-4 for contextual relevance.

### 3. 📝 Notes Generation (OpenAI GPT-4.1)
- Generates three types of notes:
  - **Main Notes (`individual_chunk_notes.md`)**
  - **Comprehensive Study Guide (`comprehensive_study_guide.md`)**
  - **Exam-Ready Notes (`detailed_exam_ready_notes.md`)**
- Notes are structured with LaTeX support and visual clarity.

### 4. 🤖 RAG Chatbot (Gemini 1.5)
- A Retrieval-Augmented Generation assistant is available to:
  - Answer questions about your notes.
  - Guide you with study tips.
  - Reference sources from the notes during responses.

---

## 💡 How to Use

### 🛠️ Backend Setup

1. Clone this repo on an EC2 or local machine.
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
