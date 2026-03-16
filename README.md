# 🎓 MentorX

> **MentorX** is an AI-powered learning assistant with chat, quiz generation, and student progress tracking.

---

## ✨ Features

- 🤖 **AI Chat** — Conversational learning assistant powered by Ollama (local LLM)
- 📝 **Quiz Generation** — Automatically generate quizzes on any topic
- 📊 **Progress Tracking** — Monitor student learning progress over time
- 🗄️ **MongoDB Integration** — Persistent data storage (optional)
- 🌐 **Web Interface** — Clean, responsive Flask-based UI

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Backend | Python · Flask |
| AI Engine | Ollama · Llama 7B (local) |
| Database | MongoDB (optional) |
| Environment | python-dotenv |

---

## 🚀 Getting Started

### Prerequisites

- Python 3.10+
- [Ollama](https://ollama.com) installed and running locally
- MongoDB URI *(optional — the app works without it)*

### 1. Install Ollama & Pull the Model

```bash
# Install Ollama from https://ollama.com/download
# Then pull the Llama 7B model
ollama pull llama2
```

> Make sure Ollama is running before starting the app. By default it listens on `http://localhost:11434`.

### 2. Clone & Install

```bash
# Clone the repository
git clone https://github.com/Aalezz/MentorX.git
cd MentorX

# Create and activate a virtual environment
python -m venv .venv

# Windows
.venv\Scripts\activate

# macOS / Linux
source .venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Set up environment variables
cp .env.example .env
```

### 3. Configure Environment

Open `.env` and fill in your values:

```env
# Flask secret key (change this to a random string)
SECRET_KEY=your-random-secret-key

# Ollama settings
OLLAMA_HOST=http://localhost:11434
OLLAMA_MODEL=llama2

# Optional
MONGODB_URI=mongodb+srv://...
PORT=5000
```

> ⚠️ **Never commit your `.env` file.** It is already listed in `.gitignore`.

### 4. Run the App

```bash
python app.py
```

Then open your browser at [http://localhost:5000](http://localhost:5000)

---

## 📁 Project Structure

```
MentorX/
├── app.py                 # Main Flask application
├── requirements.txt       # Python dependencies
├── .env.example           # Environment variable template
├── .gitignore
├── static/                # CSS, JS, images
└── templates/             # HTML templates (Jinja2)
```

---

## 🔑 Environment Variables

| Variable | Required | Description |
|---|---|---|
| `SECRET_KEY` | ✅ Yes | Flask session secret — use a long random string |
| `OLLAMA_HOST` | ✅ Yes | Ollama server URL (default: `http://localhost:11434`) |
| `OLLAMA_MODEL` | ✅ Yes | Model to use (default: `llama2`) |
| `MONGODB_URI` | ❌ No | MongoDB connection string for persistent storage |
| `PORT` | ❌ No | Port to run the server on (default: `5000`) |

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
  Built with ❤️ using <a href="https://ollama.com">Ollama</a> · Runs 100% locally
</div>
