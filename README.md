# 🚀 AgenticIntel

> An AI-powered multi-agent research automation platform built with LangChain, GPT-4o-mini, and Streamlit that autonomously researches topics, extracts insights, generates structured reports, and evaluates output quality using intelligent agent orchestration.

---

# 📌 Overview

AgenticIntel is a powerful multi-agent research system designed to automate the end-to-end research workflow using AI agents. The platform autonomously searches the web, extracts content, synthesizes information into professional reports, and critiques the final output for quality assurance.

The system demonstrates advanced agentic AI patterns with modular orchestration, intelligent tool usage, and scalable research automation pipelines.

---

# 🌟 Core Features

- 🤖 Multi-Agent Architecture
- 🔎 Automated Web Research
- 📚 Intelligent Content Extraction
- 📝 AI-Powered Report Generation
- 📊 Report Evaluation & Scoring
- 🌐 Streamlit Interactive UI
- ⚡ LangChain Agent Orchestration
- 🧠 GPT-4o-mini Powered Reasoning

---

# 🏗️ System Architecture

```text
Streamlit UI
      ↓
Research Pipeline
      ↓
 ┌───────────────┐
 │ Search Agent  │
 └──────┬────────┘
        ↓
 ┌───────────────┐
 │ Reader Agent  │
 └──────┬────────┘
        ↓
 ┌───────────────┐
 │ Writer Chain  │
 └──────┬────────┘
        ↓
 ┌───────────────┐
 │ Critic Chain  │
 └───────────────┘
```

---

# 🧠 Agent Responsibilities

## 🔎 Search Agent

- Discovers relevant information from the web using Tavily API
- Performs autonomous topic exploration

---

## 📚 Reader Agent

- Extracts readable content from websites
- Uses multiple fallback scraping strategies

---

## 📝 Writer Chain

- Generates structured research reports
- Synthesizes findings into coherent sections

---

## 📊 Critic Chain

- Evaluates report quality
- Provides scoring and improvement suggestions

---

# ⚙️ Tech Stack

## Backend & AI

- LangChain
- Gemni 
- Python

---

## Web & UI

- Streamlit

---

## Research & Extraction

- Tavily API
- BeautifulSoup4
- Trafilatura
- Readability-lxml

---

## Utilities

- Python-dotenv
- Rich

---

# 📂 Project Structure

```text
.
├── app.py
├── main.py
├── requirements.txt
├── README.md
├── LICENSE
│
└── src/
    ├── agents/
    │   └── agents.py
    ├── tools/
    │   └── tools.py
    └── pipelines/
        └── pipeline.py
```

---

# 🔄 Workflow

1. User enters a research topic
2. Search Agent gathers relevant sources
3. Reader Agent extracts website content
4. Writer Chain generates structured report
5. Critic Chain evaluates output quality
6. Final report is displayed with scores

---

# 🚀 Installation

## Clone Repository

```bash
git clone <repository-url>
cd AgenticIntel
```

---

## Create Environment

```bash
conda create -n agenticintel python=3.11 -y
conda activate agenticintel
```

---

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Configure Environment Variables

Create `.env` file:

```env
OPENAI_API_KEY=your_openai_api_key
TAVILY_API_KEY=your_tavily_api_key
```

---

# 💡 Usage

## Run Streamlit App

```bash
streamlit run app.py
```

Open:

```text
http://localhost:8501
```

---

## Run via Script

```bash
python main.py
```

---
