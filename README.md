# 🤖 AiAgent – Autonomous Research Assistant

AiAgent is a Streamlit-based AI-powered research assistant that leverages OpenAI, Groq, and AutoGen to automate literature search, summarization, and idea generation using tools like `scholarly`.

---

## 🚀 Features

- Query Google Scholar for research papers using `scholarly`
- Auto-summarize articles using OpenAI or Groq LLMs
- Streamlit UI to interact with agents
- Modular code using AutoGen's `AssistantAgent`
- Environment config with `.env` for API keys

---

## 📦 Requirements

- Python 3.10+
- Conda (recommended)
- Internet connection (for API calls)

---

## 🛠️ Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/codeypas/AiAgent.git
cd AiAgent
```

---

### 2. Create and Activate a Virtual Environment

```bash
conda create -n Aiagent python=3.10 -y
conda activate Aiagent
```

_Or use `venv` if not using Conda:_

```bash
python3 -m venv Aiagent
source Aiagent/bin/activate  # On Windows: Aiagent\Scripts\activate
```

---

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

_If `requirements.txt` is missing, install packages manually:_

```bash
pip install streamlit python-dotenv scholarly groq autogen
```

---

### 4. Create `.env` File

In the project root, create a file named `.env` and add your API key:

```ini
GROQ_API_KEY=your_groq_api_key_here
OPENAI_API_KEY=your_openai_api_key_here  # if needed
```

---

### 5. Run the App

```bash
streamlit run app.py
```

---

## 🧠 Project Structure

```
AiAgent/
│
├── app.py                # Streamlit frontend
├── agents.py             # Agent definitions using AutoGen
├── data_loader.py        # Fetch scholarly articles
├── requirements.txt      # Python dependencies
└── .env                  # API keys (not tracked in Git)
```

---

## 🧪 Sample Queries

You can type in queries like:

- `Latest research on diffusion models`
- `What are the applications of quantum computing in cybersecurity?`

---

## ❗ Troubleshooting

- **groq not installed**:  
  ```bash
  pip install groq
  ```

- **No module named 'autogen'**:  
  ```bash
  pip install autogen
  ```

- **No module named 'scholarly'**:  
  ```bash
  pip install scholarly
  ```

- **No module named 'dotenv'**:  
  ```bash
  pip install python-dotenv
  ```

---

## 🌐 TODO (optional)

- [ ] Add citation export feature
- [ ] Add PDF parser for full papers
- [ ] Save query history

---

## License
This project is for educational purposes.

---

## Contributing
Feel free to fork the repo, submit issues, or create pull requests for improvements!

---

## 👨‍💻 Author  

**Bijay Adhikari**  
📌 [GitHub Profile](https://github.com/codeypas)  
📧 Contact: bjbestintheworld@gmail.com  

---
Made with ❤️ by Codeypas


