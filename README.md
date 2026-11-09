# 🚀 AIESEC Opportunities Recommender

**Intelligent Opportunity Matching Using NLP, LLMs, and Similarity-Based Recommendation**

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Processing-150458.svg)
![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-013243.svg)
![Ollama](https://img.shields.io/badge/Ollama-Local%20LLM-black.svg)
![GraphQL](https://img.shields.io/badge/GraphQL-API-E10098.svg)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626.svg)

This project explores how **Artificial Intelligence**, **Natural Language Processing (NLP)**, and **Recommendation Systems** can automate the process of matching candidates with relevant international opportunities.

Using a candidate's CV, the system extracts key skills, qualifications, and interests through a **local Ollama LLM**, then compares the profile against opportunity data collected from the **AIESEC EXPA GraphQL API**. Opportunities are ranked using **cosine similarity**, providing personalized recommendations based on profile relevance.

---

## 📌 Table of Contents

- [Project Objective](#-project-objective)
- [System Architecture](#️-system-architecture)
- [Key Features](#-key-features)
- [Tech Stack](#-tech-stack)
- [Skills Demonstrated](#-skills-demonstrated)
- [Dataset](#-dataset)
- [Getting Started](#-getting-started)
- [Future Improvements](#-future-improvements)
- [Business Impact](#-business-impact)
- [Authors](#-authors)

---

## 🎯 Project Objective

Finding suitable internships can be overwhelming when candidates must manually search through hundreds of opportunities.

This project addresses that challenge by building an AI-powered workflow that:

- Extracts information from candidate CVs
- Processes and cleans opportunity data
- Generates semantic candidate profiles
- Computes similarity scores between candidates and opportunities
- Recommends the most relevant opportunities

The goal is to demonstrate practical applications of **Data Science**, **Artificial Intelligence**, **NLP**, **Recommendation Systems**, and **Data Engineering**.

---

## ⚙️ System Architecture

```text
Candidate CV
      │
      ▼
Local Ollama LLM
(Skill & Keyword Extraction)
      │
      ▼
Candidate Profile Vector
      │
      ├─────────────────────┐
      │                     │
      ▼                     ▼
EXPA GraphQL API      Opportunity Dataset
      │                     │
      ▼                     ▼
Data Cleaning & Feature Engineering
      │
      ▼
Vector Representation
      │
      ▼
Cosine Similarity
      │
      ▼
Ranked Opportunities
```

---

## 🔍 Key Features

### 📄 CV Parsing with LLM
- Uses a local **Ollama** Large Language Model
- Extracts:
  - Technical skills
  - Soft skills
  - Academic background
  - Keywords
  - Areas of interest

### 🌐 API-Driven Data Collection
- Retrieves live opportunities from the **AIESEC EXPA GraphQL API**
- Collects:
  - Job titles
  - Opportunity descriptions
  - Skills requirements
  - Languages
  - Locations
  - Start dates
  - Organization information

### 🧹 Data Preparation
- Cleans and transforms nested API responses
- Handles missing values
- Standardizes textual information
- Prepares data for recommendation tasks

### 🤖 Similarity-Based Recommendation
- Converts candidate and opportunity profiles into comparable feature representations
- Computes similarity using **cosine similarity**
- Returns ranked recommendations

### 📊 Explainable Results
- Highlights matching skills and keywords
- Provides transparent recommendation logic
- Helps users understand *why* opportunities are suggested

---

## 🛠 Tech Stack

| Category | Technologies |
|---|---|
| **Programming** | Python |
| **Data Processing** | Pandas, NumPy |
| **AI & NLP** | Ollama, LLM-Based Information Extraction |
| **Recommendation System** | Cosine Similarity, Content-Based Filtering |
| **Data Acquisition** | GraphQL, Requests |
| **Development Environment** | Jupyter Notebook, Google Colab |

---

## 📈 Skills Demonstrated

- Data Collection
- API Integration
- Data Cleaning
- Feature Engineering
- Natural Language Processing
- Recommendation Systems
- Prompt Engineering
- Similarity Search
- Data Analysis
- AI Application Development

---

## 📂 Dataset

Opportunity data is collected directly from the **AIESEC EXPA GraphQL API** and includes:

| Category | Features |
|---|---|
| **Opportunities** | Title, Description |
| **Requirements** | Skills, Languages |
| **Academic Information** | Study Levels |
| **Location** | Country, City |
| **Programs** | Internship Types |
| **Organization** | Partner Information |
| **Availability** | Start Dates, Openings |

---

## 🚀 Getting Started

### Prerequisites

- Python 3.10+
- [Ollama](https://ollama.com/) installed and running locally
- A pulled Ollama model (e.g. `ollama pull llama3`)
- An AIESEC EXPA API access token

### Installation

```bash
# Clone the repository
git clone https://github.com/NadaDr/aiesec-opportunities-recommender.git
cd aiesec-opportunities-recommender

# Install dependencies
pip install pandas numpy requests scikit-learn ollama jupyter
```

### Usage

1. Start Ollama and make sure your model is available:
   ```bash
   ollama serve
   ```
2. Open the notebook:
   ```bash
   jupyter notebook
   ```
3. Add your EXPA API token and the path to your CV.
4. Run all cells to extract your profile, fetch opportunities, and get ranked recommendations.

---

## 🔮 Future Improvements

- [ ] Implement semantic embeddings using **Sentence Transformers**
- [ ] Improve recommendation accuracy with **hybrid recommender** approaches
- [ ] Add candidate–opportunity **explanation generation** with LLMs
- [ ] Deploy as a **Streamlit** web application
- [ ] Integrate **vector databases** for scalable matching
- [ ] Evaluate recommendation performance using **ranking metrics**

---

## 💼 Business Impact

This solution demonstrates how AI can support:

- International recruitment
- Talent matching
- Career recommendation platforms
- Internship discovery systems
- Educational and professional mobility programs

---

## 👩‍💻 Authors

**Nada Dridi**
Computer Engineering Student | Former Local Head of Marketing AIESEC in Tunisia, Sousse
🔗 [LinkedIn](https://linkedin.com/in/nadadridi) · [GitHub](https://github.com/NadaDr)

