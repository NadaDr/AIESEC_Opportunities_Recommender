#  AIESEC Opportunities Recommender (Based On CV)

### Turning candidate profiles into relevant opportunities.

A Python project exploring how **API-driven data collection and intelligent matching** can help candidates discover international opportunities aligned with their skills, academic background, and interests.

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/GraphQL-E10098?style=for-the-badge&logo=graphql&logoColor=white" alt="GraphQL" />
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas" />
  <img src="https://img.shields.io/badge/Google_Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=black" alt="Google Colab" />
</p>

---

## ◈ Overview

Finding opportunities that match a candidate's qualifications can be time-consuming. This project explores the foundations of a **CV-based opportunity recommendation system** by collecting structured opportunity data from the AIESEC GraphQL API.

The notebook retrieves information about international opportunities, including required skills, languages, study levels, locations, programmes, and start dates.

The collected data provides a foundation for building a system that can connect candidate profiles with relevant opportunities.

## ✦ Key Learning Outcomes

<table>
  <tr>
    <td width="50%">
      <h3>⌘ API Integration</h3>
      Working with GraphQL queries, variables, fragments, nested fields, and HTTP POST requests.
    </td>
    <td width="50%">
      <h3>▤ Data Extraction</h3>
      Retrieving and inspecting structured JSON data from an external API using Python.
    </td>
  </tr>
  <tr>
    <td width="50%">
      <h3>⚙ Data Filtering</h3>
      Applying programme, date, and partner-type filters to retrieve relevant opportunities.
    </td>
    <td width="50%">
      <h3>✧ Recommendation Foundations</h3>
      Identifying candidate and opportunity attributes that can support profile matching and relevance ranking.
    </td>
  </tr>
</table>

## ⌘ Project Workflow

```text
AIESEC GraphQL API
        │
        ▼
  Query Construction
        │
        ▼
 HTTP Request (Python)
        │
        ▼
   JSON Response
        │
        ▼
 Data Inspection & Filtering
        │
        ▼
  Opportunity Dataset
        │
        ▼
 Future: CV-Based Matching
```

## ◈ Data Collected

| Attribute | Description |
|---|---|
| Opportunity details | Title, description, project information |
| Location | Country and host location |
| Skills & languages | Opportunity requirements |
| Academic background | Study levels and programme details |
| Organization | Company and partner information |
| Availability | Start dates, duration, available openings |
| Additional details | Compensation and logistics, when provided |

## ⚙ Tech Stack

- **Language:** Python
- **API:** GraphQL over HTTP
- **Libraries:** Requests, JSON
- **Environment:** Google Colab / Jupyter Notebook
- **Next steps:** Pandas, data cleaning, content-based recommendation algorithms

## ▶ Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/CV-Opportunity-Recommender.git
cd CV-Opportunity-Recommender
```

### 2. Install dependencies

```bash
pip install requests pandas
```

Pandas is needed only if you use it in the notebook.

### 3. Open the notebook

Open `CV_Opportunity_Recommender.ipynb` in Google Colab or Jupyter Notebook.

### 4. Configure API credentials

Store the required API credential in Google Colab Secrets or an environment variable. Never commit access tokens or other secrets to GitHub.

### 5. Run the notebook

Execute the cells to retrieve and inspect opportunity data. API access, credentials, and current endpoint availability may affect execution.

## 🚀 Future Improvements

- [ ] Transform nested JSON responses into structured Pandas DataFrames.
- [ ] Clean missing values and remove duplicate opportunities.
- [ ] Extract skills, qualifications, and experience from CVs.
- [ ] Develop a content-based recommendation algorithm.
- [ ] Rank opportunities according to candidate-profile similarity.
- [ ] Explain why each opportunity matches a candidate.
- [ ] Evaluate recommendation quality using sample candidate profiles.

## 🎯 Project Goal

Explore the intersection of **data engineering and artificial intelligence** by developing a workflow that starts with external data ingestion and progresses toward personalized opportunity recommendations.

## 👩‍💻 Author

**Nada Dridi & Med Helmi Essouied**

Computer Engineering Student | Interested in Data Engineering, Data Science & AI

[LinkedIn](https://linkedin.com/in/nadadridi) · [GitHub](https://github.com/NadaDr)

