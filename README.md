# 🔬 ResearchMind – Multi-Agent AI Research System

> Four specialized AI agents collaborate to deliver a polished research report on any topic — automatically.

**🚀 Live Demo → [multi-agents-system.streamlit.app](https://multi-agents-system.streamlit.app/)**

---

## What it does

ResearchMind runs a 4-step autonomous pipeline:

1. **Search Agent** — Searches the web in real-time using Tavily API
2. **Reader Agent** — Scrapes and extracts deep content from the most relevant URLs
3. **Writer Chain** — Drafts a structured, professional research report
4. **Critic Chain** — Reviews and scores the report with actionable feedback

---

## Demo

![Pipeline](https://img.shields.io/badge/Status-Live-success) ![Streamlit](https://img.shields.io/badge/Streamlit-Cloud-FF4B4B?logo=streamlit) ![Gemini](https://img.shields.io/badge/Gemini-2.0--flash-4285F4?logo=google) ![LangChain](https://img.shields.io/badge/LangChain-0.2-1C3C3C)

---

## Tech Stack

| Layer | Technology |
|---|---|
| LLM | Google Gemini 2.0 Flash |
| Agent Framework | LangGraph + LangChain |
| Search Tool | Tavily Search API |
| Web Scraping | BeautifulSoup + Requests |
| Frontend | Streamlit |
| Deployment | Streamlit Cloud |

---

## Project Structure

```
Multi-Agent-System/
├── app.py          # Streamlit frontend UI
├── agents.py       # Agent & chain definitions
├── tools.py        # web_search and scrape_url tools
├── requirements.txt
└── .env            # API keys (never commit this)
```

---

## Run Locally

**1. Clone the repo**
```bash
git clone https://github.com/akshat407/Multi-Agent-System.git
cd Multi-Agent-System
```

**2. Install dependencies**
```bash
pip install -r requirements.txt
```

**3. Add your API keys — create a `.env` file:**
```
GOOGLE_API_KEY=your_google_api_key
TAVILY_API_KEY=your_tavily_api_key
```

**4. Run the app**
```bash
streamlit run app.py
```

---

## Get API Keys

- **Google Gemini** → [aistudio.google.com](https://aistudio.google.com) (free)
- **Tavily Search** → [app.tavily.com](https://app.tavily.com) (free tier available)

---

## How the Pipeline Works

```
User Input (Topic)
       │
       ▼
 [Search Agent] ──► Tavily API ──► Real-time web results
       │
       ▼
 [Reader Agent] ──► BeautifulSoup ──► Scraped deep content
       │
       ▼
 [Writer Chain] ──► Gemini LLM ──► Structured research report
       │
       ▼
 [Critic Chain] ──► Gemini LLM ──► Score + feedback
       │
       ▼
  Final Report (downloadable .md)
```

---

## Author

**Akshat Srivastava**
- 📧 srivastava.akshat407@gmail.com
- 💼 [LinkedIn](https://www.linkedin.com/in/akshat-srivastava-a50285202/)
- 🐙 [GitHub](https://github.com/akshat407)

---

⭐ Star this repo if you found it useful!
