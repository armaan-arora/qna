# 🧠 LLM Question-Answering Application

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.9+-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
  <img src="https://img.shields.io/badge/OpenAI-GPT--3.5--Turbo-412991?style=for-the-badge&logo=openai&logoColor=white" alt="OpenAI"/>
  <img src="https://img.shields.io/badge/LangChain-🦜-121212?style=for-the-badge" alt="LangChain"/>
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white" alt="Streamlit"/>
  <img src="https://img.shields.io/badge/License-MIT-blue?style=for-the-badge" alt="License"/>
</p>

<p align="center">
  <b>A powerful LLM-powered application that extracts insights from your documents using natural language queries 🚀</b>
</p>

<p align="center">
  <img src="screenshots/demo.gif" alt="Demo" width="700"/>
</p>

<p align="center">
  <a href="https://jacobj215-llm-qna-chat-bot-app-yzhsmu.streamlit.app/">🌐 Live Demo</a> •
  <a href="#-installation">📦 Installation</a> •
  <a href="#-how-it-works">⚙️ How It Works</a> •
  <a href="#-usage">🚀 Usage</a>
</p>

---

## 📋 Table of Contents

- [Problem Statement](#-problem-statement)
- [Solution](#-solution)
- [How It Works](#-how-it-works)
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Tools Used](#-tools-used)
- [Installation](#-installation)
- [Usage](#-usage)
- [Future Scope](#-future-scope)
- [Contributing](#-contributing)
- [License](#-license)

---

## ❓ Problem Statement

Extracting specific information from documents is a tedious and time-consuming process:

- 📚 **Manual Reading** — Skimming through lengthy PDFs and documents to find specific answers is inefficient
- 🔍 **Keyword Limitations** — Traditional Ctrl+F search only finds exact matches, missing contextual information
- ⏱️ **Time Drain** — Professionals waste hours searching through reports, contracts, and research papers
- 🧩 **Context Loss** — Important nuances and relationships between concepts get missed
- 💰 **Costly Solutions** — Many enterprise Q&A tools require expensive subscriptions
- 🔒 **Privacy Concerns** — Uploading sensitive documents to unknown services raises security issues

---

## 💡 Solution

**LLM Q&A Application** is a user-friendly, cost-effective solution that lets you chat with your documents using natural language — powered by OpenAI's GPT-3.5 Turbo and free HuggingFace embeddings.

### ✨ Why This App?

| Benefit | Description |
|---------|-------------|
| 💸 **Free Embeddings** | Uses HuggingFace's `all-MiniLM-L6-v2` — no embedding costs! |
| 🔐 **Bring Your Own Key** | Use your own OpenAI API key for full control |
| ⚡ **Fast Processing** | Documents processed in 1-2 minutes |
| 🎯 **Accurate Answers** | Semantic search finds contextually relevant information |
| 🌐 **No Installation** | Use the live demo instantly |

---

## ⚙️ How It Works

```
┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐
│  📄 Upload      │────▶│  🔪 Chunk       │────▶│  🧮 Embed with  │
│  PDF/DOCX/TXT   │     │  Document       │     │  MiniLM-L6-v2   │
└─────────────────┘     └─────────────────┘     └────────┬────────┘
                                                         │
                                                         ▼
┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐
│  💬 Get Answer  │◀────│  🤖 GPT-3.5     │◀────│  🔍 FAISS       │
│  from GPT       │     │  Turbo          │     │  Vector Search  │
└─────────────────┘     └─────────────────┘     └─────────────────┘
        ▲                                               ▲
        │              ┌─────────────────┐              │
        └──────────────│  ❓ Your        │──────────────┘
                       │   Question      │
                       └─────────────────┘
```

### Pipeline Breakdown

1. **📤 Document Upload** — Upload your PDF, DOCX, or TXT file
2. **🔪 Chunking** — Document is split into manageable text chunks
3. **🧮 Embedding** — Chunks are converted to vectors using HuggingFace's `all-MiniLM-L6-v2` (FREE!)
4. **🗄️ Vector Storage** — Embeddings are stored in FAISS for efficient similarity search
5. **❓ Query** — You ask a question in natural language
6. **🔍 Retrieval** — FAISS finds the most relevant chunks
7. **🤖 Generation** — GPT-3.5-Turbo generates an answer based on retrieved context

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 📤 **Multi-Format Upload** | Support for PDF, DOCX, and TXT files |
| 🧠 **Free Embeddings** | HuggingFace `all-MiniLM-L6-v2` — zero embedding costs |
| ⚡ **FAISS Vector Search** | Lightning-fast similarity search |
| 🤖 **GPT-3.5-Turbo** | Powered by OpenAI's capable language model |
| 🔐 **BYOK (Bring Your Own Key)** | Use your personal OpenAI API key |
| 🌐 **Live Demo** | Try instantly without local setup |
| 📱 **Responsive UI** | Clean Streamlit interface |

---

## 🛠️ Tech Stack

### Core Components

| Technology | Purpose |
|------------|---------|
| ![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white) | Primary Language |
| ![LangChain](https://img.shields.io/badge/🦜_LangChain-121212?style=flat) | LLM Orchestration & Chains |
| ![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat&logo=openai&logoColor=white) | GPT-3.5-Turbo LLM |
| ![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat&logo=huggingface&logoColor=black) | all-MiniLM-L6-v2 Embeddings |

### Infrastructure

| Technology | Purpose |
|------------|---------|
| ![FAISS](https://img.shields.io/badge/FAISS-0467DF?style=flat&logo=meta&logoColor=white) | Vector Storage & Similarity Search |
| ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat&logo=streamlit&logoColor=white) | Web Interface |

---

## 🔧 Tools Used

| Tool | Purpose |
|------|---------|
| ![LangChain](https://img.shields.io/badge/🦜_LangChain-121212?style=flat) | Document loading, chunking, and QA chains |
| ![FAISS](https://img.shields.io/badge/FAISS-0467DF?style=flat&logo=meta&logoColor=white) | Efficient similarity search & clustering |
| ![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat&logo=openai&logoColor=white) | GPT-3.5-Turbo for answer generation |
| ![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat&logo=huggingface&logoColor=black) | Free embedding generation |
| ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat&logo=streamlit&logoColor=white) | Interactive web application |
| ![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white) | Version Control |

---

## 📦 Installation

###  Run Locally 💻

#### Prerequisites

- Python 3.9+
- OpenAI API Key ([Get one here](https://platform.openai.com/api-keys))

#### Steps

```bash
# 1. Clone the repository
git clone https://github.com/armaan-arora/qna.git

# 2. Navigate to project directory
cd qna

# 3. Create virtual environment (recommended)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# 4. Install dependencies
pip install -r requirements.txt

# 5. Run the Streamlit app
streamlit run app.py
```

The app will open in your browser at `http://localhost:8501`

---

## 🚀 Usage

### Step-by-Step Guide

#### 1️⃣ Enter Your OpenAI API Key

<p align="center">
  <img src="screenshots/api_auth1.png" alt="API Key Step 1" width="400"/>
  <img src="screenshots/api_auth2.png" alt="API Key Step 2" width="400"/>
</p>

#### 2️⃣ Upload Your Document

Upload a file in one of the supported formats:
- 📕 **PDF** — Research papers, reports, contracts
- 📘 **DOCX** — Word documents
- 📄 **TXT** — Plain text files

*Drag & drop or browse to select your file*

#### 3️⃣ Wait for Processing

⏳ The app will chunk and embed your document (typically 1-2 minutes depending on file size)

#### 4️⃣ Ask Your Questions

Type your question and click **Send**. Get accurate, context-aware answers in ~1 minute!

### 💡 Example Questions

```
📌 "What are the key findings in this research paper?"
📌 "Summarize the main arguments in section 3"
📌 "What are the contractual obligations mentioned?"
📌 "Explain the methodology used in this study"
📌 "What recommendations does the author make?"
```

---

## ⚡ Performance

| Metric | Value |
|--------|-------|
| **Document Processing** | 1-2 minutes |
| **Query Response Time** | ~1 minute |
| **Embedding Model** | all-MiniLM-L6-v2 |
| **LLM** | GPT-3.5-Turbo |
| **Embedding Cost** | 💸 FREE |
| **Supported Formats** | PDF, DOCX, TXT |

---

## 🔮 Future Scope

The application has exciting potential for growth:

| Feature | Description | Priority |
|---------|-------------|----------|
| 🔄 **Multi-Model Support** | Add GPT-4, Claude, and local LLMs | High |
| 💬 **Chat History** | Maintain conversation context | High |
| 📎 **Source Citations** | Show exact document sections used | High |
| 📊 **Multiple Documents** | Query across multiple files | Medium |
| 🌐 **URL Support** | Q&A over web pages | Medium |
| 🔐 **User Authentication** | Save sessions and documents | Medium |
| 📈 **Analytics** | Track popular queries and usage | Low |
| 🗣️ **Voice Input** | Ask questions via speech | Low |
| 📱 **Mobile App** | Native iOS/Android apps | Future |

---

## 📁 Project Structure

```
qna/
├── 📄 app.py                 # Main Streamlit application
├── 📂 screenshots/
│   ├── demo.gif              # Application demo
│   ├── api_auth1.png         # API key screenshot 1
│   └── api_auth2.png         # API key screenshot 2
├── 📄 requirements.txt       # Python dependencies
├── 📄 .gitignore
└── 📄 README.md
```

---

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. 🍴 Fork the repository
2. 🌿 Create a feature branch (`git checkout -b feature/amazing-feature`)
3. 💾 Commit your changes (`git commit -m 'Add amazing feature'`)
4. 📤 Push to the branch (`git push origin feature/amazing-feature`)
5. 🔃 Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgements

- [LangChain](https://langchain.com/) — LLM application framework
- [OpenAI](https://openai.com/) — GPT-3.5-Turbo
- [HuggingFace](https://huggingface.co/) — Free embeddings with all-MiniLM-L6-v2
- [FAISS](https://faiss.ai/) — Efficient similarity search
- [Streamlit](https://streamlit.io/) — Web app framework
- Original inspiration: [JacobJ215/LLM-QnA-CHAT-BOT](https://github.com/JacobJ215/LLM-QnA-CHAT-BOT)

---

## 👤 Author

**Armaan Arora**

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/armaan-arora)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/armaan-arora)

---

<p align="center">
  ⭐ Star this repo if you found it helpful! ⭐
</p>

<p align="center">
  Made with ❤️ and 🤖 by Armaan Arora
</p>
