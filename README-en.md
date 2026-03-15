# 🧠 Multimodal RAG CLI

README's language:
- [Portuguese](https://github.com/louuispy/multimodal-rag-cli-gt/blob/main/README.md)
- [English]()

---

> Chatbot with multimodal RAG in CLI - it processes PDF files, YouTube videos and images as a knowledge base to answer user questions with LLM.

---

This project was built and taught to my students during the Module 2 of Geração Tech GenAI course, focused on RAG (Retrieval-Augmented Generation) and LangChain.

---

## ✨ Features

- **PDF** — loads and indexes PDF files as a context
- **YouTube** — extracts the YouTube video transcription from a URL
- **Image** — process images
- **CLI Interface** — question-and-answer interface in terminal
- **RAG** — retrieve important parts from the material before generating the response

---

## 🛠️ Stack

| Technology | Role |
|---|---|
| Python | Main language |
| LangChain | Orquestrates RAG pipeline |
| InMemoryVectorStore | Local Vectorstore |
| Gemini | LLM to generate responses |
| uv | Package manager and virtual environment |

---

## 📁 Structure

```
multimodal-rag-cli-gt/
├── main.py           # The orquestrator 
├── utils/            # The functions separated in specific files
├── material/         # Project tutorial
├── pyproject.toml    # Dependencies
└── .python-version   # Python version
```

---

## 🚀 How to use

### Prerequisites

- Python 3.11+
- [uv](https://docs.astral.sh/uv/) 

### Installation

```bash
# Clone this repository
git clone https://github.com/louuispy/multimodal-rag-cli-gt.git
cd multimodal-rag-cli-gt

# Install the dependencies with uv
uv sync
```

### Settings

Create a `.env` file in the project root with your API key:

```env
GOOGLE_API_KEY=type_your_apikey_here
```

### Running the project

```bash
uv run main.py
```

Follow the instructions in the terminal to specify the source type (PDF, YouTube or Image) and ask your questions.

---

## 📄 License

MIT © [louuispy](https://github.com/louuispy)
