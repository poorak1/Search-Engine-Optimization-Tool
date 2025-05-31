# SEO Report Generation using Multi-Agent AI System

## Problem Statement
Small or new business owners often lack the budget, time, or technical expertise to invest in comprehensive SEO services. Hiring an SEO consultant or agency can be a substantial cost per audit. This creates a significant barrier to online visibility and growth. These businesses risk being overshadowed by larger competitors with dedicated SEO teams and marketing budgets, regardless of the quality of their actual offerings.

## Project Description
This Streamlit-based web application accepts a URL input and generates a brief SEO report. It employs CrewAI to orchestrate four intelligent agents working together to analyze the website's SEO profile and generate a strategic report.

### Agent Roles & Interactions
## 👥 Agent Roles and Responsibilities

### 🧠 Website Analyst
- **Role**: Senior SEO Analyst  
- **Task**: Analyze the target website’s current SEO performance and provide actionable insights to improve its search engine visibility.

---

### 🕵️‍♂️ Competitor Analyst
- **Role**: B2B Competitor Analyst  
- **Task**: Identify the top competitors operating in the same domain or industry as the target website.

---

### 🔍 Competitor Researcher
- **Role**: SEO Research Specialist  
- **Task**: Conduct in-depth SEO comparisons between the target website and its identified competitors. Highlight strengths, weaknesses, and keyword opportunities.

---

### 📝 Report Writer
- **Role**: Technical Report Writer  
- **Task**: Compile all findings and analyses from the other agents into a structured, professional SEO report that is clear, insightful, and actionable.

## 🛠️ Tools, Libraries, and Frameworks Used

### Agent Framework
- **CrewAI**: Used to create, manage, and orchestrate a team of intelligent agents that collaborate on tasks in a structured workflow.

### Information Retrieval Tools
- **SerperDevTool**: Interfaces with the Google Search API to retrieve real-time SERP (Search Engine Results Page) data.
- **ScrapeWebsiteTool**: Extracts content directly from the provided website URL for analysis by various agents.

### Web UI
- **Streamlit**: Provides a lightweight, interactive web interface allowing users to input a website URL, configure the model, and view the generated SEO report.

### Input Validation
- **validators**: Ensures that the user inputs a syntactically valid URL before proceeding with the analysis.

### Others
- **os**: Used for securely setting and accessing API keys and environment variables required by CrewAI and the tools.

## LLM Selection
GPT-4o and 4.1 is being used due to its complex reasoning abilities. An option to use GPT-4o mini and 4.1 mini is also given for higher inference speed with respect to heir subsequent heavy tier models. In free tier models, gemini as well as groq can be used for high inference speed.

