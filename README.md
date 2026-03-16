<div align="center">

# 🎓 MentorX

### AI-Powered Personal Learning Assistant

*Chat with your documents · Generate quizzes · Build your study path · Test your knowledge*

*Runs 100% locally — no internet, no API keys, no data sharing*

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=flat-square&logo=python)
![Gradio](https://img.shields.io/badge/UI-Gradio-orange?style=flat-square)
![Ollama](https://img.shields.io/badge/AI-Ollama%20Mistral%207B-green?style=flat-square)
![LangChain](https://img.shields.io/badge/RAG-LangChain-purple?style=flat-square)
![ChromaDB](https://img.shields.io/badge/VectorDB-ChromaDB-red?style=flat-square)

</div>

---

## 🧠 What is MentorX?

MentorX is an AI-powered learning assistant that turns any document into an interactive study session. Upload a PDF, Word file, PowerPoint, or paste a YouTube link — then ask questions, get explanations, generate quizzes, and build a personalized study plan, all powered by a local AI model running entirely on your machine.

---

## ✨ Features

### 📄 Document Understanding
Upload your study material and have a conversation with it. MentorX reads your document, understands it, and answers your questions based on the actual content.

- Supports **PDF, DOCX, DOC, PPTX, PPT, TXT, MD, CSV**
- Paste a **YouTube URL** to analyze video content
- Automatically extracts and indexes content using RAG

### 💬 Ask Questions
Get precise answers pulled directly from your uploaded document. No hallucinations — the AI only answers based on what's in your material.

### 🔍 Explain Concepts
Struggling with a concept? Get it explained at your level:
- **Beginner** — simple everyday language
- **Intermediate** — clear terms with some technical vocabulary
- **Advanced** — full technical depth

### 📝 Generate MCQs
Auto-generate multiple-choice questions from your document to test yourself. Choose how many questions (1–10) and get explanations for every answer.

### 📋 Summarize Documents
Get a summary of your material in the length you need:
- **Short** — 100–150 words
- **Medium** — 200–300 words
- **Long** — 400–600 words

### 🗺️ Student Learning Path
Enter a topic and get a **personalized learning roadmap** with a structured curriculum tailored to your level and goals — whether it's a 1-day crash course, a 1-week sprint, or a 1-month deep dive.

### 🧪 Test Your Knowledge
Interactive quiz mode with configurable difficulty:
- **Easy / Medium / Hard / Mixed**
- Question-by-question interface with instant feedback
- Final score + performance analysis + learning recommendations

### 💻 Code Explanation
Paste any code snippet and get a clear line-by-line breakdown of what it does.

### ❓ Ask Your Doubts
Have a specific confusion? Describe it and get a targeted, detailed explanation.

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| UI | Gradio |
| Backend | Python |
| AI Model | Ollama · Mistral 7B (local) |
| RAG Framework | LangChain |
| Vector Database | ChromaDB |
| PDF Processing | PyMuPDF · pypdf |
| Video Support | PyTube |

---

## 🚀 Getting Started

### Prerequisites

- Python 3.10+
- [Ollama](https://ollama.com/download) installed on your machine

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/Aalezz/MentorX.git
cd MentorX

# 2. Create and activate a virtual environment
python -m venv .venv

# Windows
.venv\Scripts\activate

# macOS / Linux
source .venv/bin/activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Install Ollama and pull Mistral 7B automatically
python modelinstall.py

# 5. Run the app
python app.py
```

Gradio will launch and open automatically in your browser. 🎉

### Manual Model Setup (alternative to step 4)

```bash
ollama pull mistral:7b
```

---

## 📖 How to Use

1. **Upload** a document or paste a YouTube URL
2. Click **"Process Document"** and wait for indexing
3. Navigate the tabs to interact with your content:

| Tab | What it does |
|---|---|
| 💬 Ask Questions | Q&A based on your document |
| 🔍 Explain Concepts | Multi-level concept breakdowns |
| 📝 Generate MCQs | Auto-generated quiz questions |
| 📋 Summarize | Short, medium, or long summaries |
| 🗺️ Study Plan | Personalized learning roadmap |
| 💻 Explain Code | Line-by-line code analysis |
| ❓ Ask Your Doubts | Targeted doubt resolution |
| 🧪 Test Your Knowledge | Interactive quiz with scoring |

---

## ⚠️ Limitations

- Large PDFs are processed up to the first 10 pages
- YouTube processing captures video metadata, not full transcripts
- Response speed depends on your hardware
- Complex PDFs with heavy formatting may not parse perfectly

---

## 📄 License

This project is licensed under the MIT License.

---

<div align="center">
  Built with ❤️ using <a href="https://ollama.com">Ollama</a> · <a href="https://gradio.app">Gradio</a> · <a href="https://python.langchain.com">LangChain</a>
  <br><br>
  <i>Your data never leaves your machine.</i>
</div>
