# 🎓 MentorX

> **MentorX** is an AI-powered personal learning assistant that lets you chat with your documents, generate quizzes, build personalized study paths, and track your progress — all running 100% locally on your machine.

---

## ✨ Features

- 🤖 **AI Chat** — Ask questions and get intelligent answers powered by Mistral 7B running locally
- 📄 **Document Understanding** — Upload your files and chat with them using RAG (Retrieval-Augmented Generation)
- 🎥 **YouTube Support** — Paste a YouTube link and ask questions about the video content
- 📝 **Quiz Generation** — Auto-generate quizzes from any topic or uploaded document to test your knowledge
- 🗺️ **Student Learning Path** — Get a personalized learning roadmap and structured curriculum tailored to your goals and current level
- 📊 **Progress Tracking** — Monitor your learning milestones over time
- 🌐 **Interactive UI** — Clean, easy-to-use interface built with Gradio

---

## 📂 Supported File Types

| Type | Formats |
|---|---|
| Documents | PDF, DOCX, DOC |
| Presentations | PPTX, PPT |
| Text | TXT, MD, CSV |
| Video | YouTube URLs |

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

---

## 🚀 Getting Started

### Prerequisites

- Python 3.10+
- [Ollama](https://ollama.com) installed and running locally

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

# 4. Install Ollama and pull the model automatically
python modelinstall.py

# 5. Run the app
python app.py
```

Gradio will open automatically in your browser. 🎉

---

## 🤝 Contributing

Contributions are welcome! Please open an issue first to discuss what you'd like to change.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License.

---

<div align="center">
  Built with ❤️ using <a href="https://ollama.com">Ollama</a> · <a href="https://gradio.app">Gradio</a> · <a href="https://python.langchain.com">LangChain</a> · Runs 100% locally
</div>
