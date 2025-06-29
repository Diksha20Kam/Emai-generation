# Email Generation Tool

## 📧 Cold Mail Generator using LLM (Groq LLaMA 3.1 70B)

This is an AI-powered Cold Email Generator built using `LangChain`, `Streamlit`, and `Groq's LLaMA 3.1 70B` model. The app scrapes job data from a company’s careers page and generates personalized cold emails to pitch AtliQ's software solutions based on the job description and portfolio match.

---

## 🚀 Features

- ✅ **Web scraping** job descriptions from any career URL
- 🤖 **LLM-based job info extraction**: role, experience, skills, and description
- ✍️ **Cold email generation** tailored to AtliQ's services
- 🔗 **Dynamic portfolio linking** based on required skills
- 🧼 **Text cleaning pipeline** for noisy webpage content
- 🌐 **Streamlit UI** for easy use

---

## 🧱 Tech Stack

- Python 3.10+
- LangChain
- Groq LLaMA 3.1 70B (`ChatGroq`)
- Streamlit
- dotenv
- HTML/Website Scraping (`WebBaseLoader`)
- Custom Prompt Templates
- JSON Output Parsing

---


---

## ⚙️ How It Works

1. **User inputs a job posting URL**
2. The app scrapes and cleans the webpage
3. The `Chain` class:
   - Extracts job roles using `PromptTemplate` + `LLaMA 3.1`
   - Matches relevant skills to AtliQ's portfolio links
   - Generates a personalized cold email
4. The cold email is shown in the Streamlit interface

---


## **Requirements**
- Python 3.10+

- Groq API access (get it from https://console.groq.com)

- Streamlit

- LangChain

## 💡 Portfolio Matching Logic

The app uses the skills extracted from job descriptions to match with AtliQ’s internal portfolio using a similarity search logic (likely vector or keyword-based).

