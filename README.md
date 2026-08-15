# 🔬 Multi-Agent AI Research System

> An AI-powered multi-agent research system that searches the web, reads relevant sources, generates a research report, and critiques the final output.

## 🚀 Live Demo

[**Try the Research System →**](https://multi-agent-ai-research-system-hck9zcshqbvcgnelqo7k46.streamlit.app/)

## ✨ Features

* 🔍 **Search Agent** — finds recent and relevant web information using Tavily
* 📄 **Reader Agent** — selects and scrapes relevant sources
* ✍️ **Writer Chain** — generates a structured research report
* 🧐 **Critic Chain** — evaluates the report and provides feedback
* 🎨 **Streamlit UI** — interactive research interface
* 📥 **Report Download** — download generated reports as Markdown

## 🧠 Architecture

```text
Research Topic
      │
      ▼
🔍 Search Agent
      │
      ▼
📄 Reader Agent
      │
      ▼
✍️ Writer Chain
      │
      ▼
🧐 Critic Chain
      │
      ▼
Final Research Report
```

## 🛠️ Tech Stack

* **Python**
* **LangChain**
* **Mistral AI — mistral-small-2506**
* **Tavily**
* **Streamlit**
* **BeautifulSoup**
* **Requests**

## 📁 Project Structure

```text
multi-agent-ai-research-system/
│
├── app.py              # Streamlit UI
├── agents.py           # Agents and LLM chains
├── pipeline.py         # Research pipeline
├── tools.py            # Search and scraping tools
├── requirements.txt    # Dependencies
├── .gitignore
├── LICENSE
└── README.md
```

## ⚙️ Setup

### 1. Clone the repository

```bash
git clone https://github.com/SanjanaShetty/multi-agent-ai-research-system.git
cd multi-agent-ai-research-system
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

**Windows:**

```bash
.venv\Scripts\activate
```

**Linux/macOS:**

```bash
source .venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure API keys

Create a `.env` file in the project root:

```env
MISTRAL_API_KEY=your_mistral_api_key
TAVILY_API_KEY=your_tavily_api_key
```

### 5. Run the application

```bash
streamlit run app.py
```

## 🔄 Workflow

Given a research topic, the system:

1. Searches the web for relevant information.
2. Selects and scrapes a useful source.
3. Generates a structured research report.
4. Critically evaluates the report.

## 🔐 Security

API keys are stored using environment variables and are **not committed to GitHub**.

## 📜 License

This project is licensed under the [MIT License](LICENSE).

---

### 👩‍💻 Built by Sanjana Shetty

Built with **LangChain, Mistral AI, Tavily, and Streamlit**.
