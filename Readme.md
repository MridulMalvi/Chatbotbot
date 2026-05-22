# 🤖 Chatbot

A lightweight, conversational web application powered by **Google's Gemini 1.5 Flash** model, built with **Streamlit** and **LangChain**.

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?logo=streamlit&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?logo=langchain&logoColor=white)
![Google Gemini](https://img.shields.io/badge/Google%20Gemini-8E75B2?logo=google&logoColor=white)
![License](https://img.shields.io/badge/License-Apache%202.0-green)

---

## ✨ Features

- **Interactive UI** — Clean and intuitive chat interface built with Streamlit
- **Powered by Gemini** — Uses Google's `gemini-1.5-flash` model for fast, intelligent responses
- **Context Aware** — Maintains full chat history during your session so the AI remembers the conversation
- **Easy Controls** — One-click **"Clear Conversation"** button in the sidebar to reset context
- **Modular Design** — Clean separation between UI (`frontend.py`) and AI logic (`backend.py`)

---

## 🛠️ Prerequisites

Before you begin, make sure you have:

- Python **3.8 or higher** installed
- A **Google Gemini API Key** — get one free from [Google AI Studio](https://aistudio.google.com/)

---

## 🚀 Installation & Setup

### 1. Clone the Repository

```bash
git clone <your-repository-url>
cd <your-repository-folder>
```

### 2. Create a Virtual Environment *(Recommended)*

```bash
python -m venv myenv

# Activate on macOS/Linux
source myenv/bin/activate

# Activate on Windows
myenv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Set Up Environment Variables

Create a `.env` file in the root directory of the project and add your Google API key:

```env
GOOGLE_API_KEY=your_actual_api_key_here
```

> ⚠️ **Never commit your `.env` file to version control.** It is already listed in `.gitignore`.

---

## 💻 Usage

Start the chatbot by running:

```bash
streamlit run frontend.py
```

This will open a new tab in your default browser at **`http://localhost:8501`** where you can start chatting with the AI.

---

## 📁 Project Structure

```
├── frontend.py        # Streamlit UI — handles user input, chat display, and session state
├── backend.py         # LangChain integration — initializes Gemini and generates responses
├── requirements.txt   # Python package dependencies
├── .env               # (You create this) Stores your secret API key
└── .gitignore         # Excludes .env, virtual envs, and other untracked files
```

---

## 📦 Key Dependencies

| Package | Purpose |
|---|---|
| `streamlit` | Web UI framework |
| `langchain` | LLM orchestration |
| `langchain-google-genai` | Google Gemini integration |
| `python-dotenv` | Loads environment variables from `.env` |

---

## 📄 License

This project is licensed under the **Apache License 2.0**. See the [LICENSE](LICENSE) file for full details.

---

## 🙌 Acknowledgements

- [Google AI Studio](https://aistudio.google.com/) for the Gemini API
- [Streamlit](https://streamlit.io/) for the rapid UI framework
- [LangChain](https://www.langchain.com/) for LLM tooling
