# 🍽️ AI-Powered Zomato Analytics Platform

An end-to-end **AI-powered restaurant analytics platform** built using **PostgreSQL, n8n, Power BI, Gemini AI, and Lovable frontend**.

The project enables users to:
- Ask business questions in **natural language**
- Automatically generate optimized **PostgreSQL queries**
- Retrieve and analyze restaurant data
- Generate concise **business insights**
- Visualize trends through an interactive **Power BI dashboard**

This project combines:
- 📊 Data Analytics
- 🤖 AI Automation
- 🧠 Natural Language to SQL
- 📈 Business Intelligence
- ⚡ Workflow Automation

---

# 🚀 Key Features

## 🤖 AI SQL Query Generator

Users can ask questions like:

- “Top rated restaurants in Bangalore”
- “Best North Indian restaurants with online delivery”
- “Cheapest restaurants with rating above 4”
- “Most popular cuisines by city”

The AI agent:
- Converts natural language into PostgreSQL queries
- Handles fuzzy matching using `ILIKE '%keyword%'`
- Supports ranking, filtering, aggregation, and comparisons
- Prevents unsafe SQL operations

---

## 📊 AI-Generated Business Insights

After executing SQL queries, another AI agent:
- Analyzes query results
- Filters only relevant columns
- Generates:
  - 📌 Brief summary
  - 💡 Business insights
  - 🔍 Key observations

Responses are returned in structured JSON format for frontend rendering.

### Example Output

```json
{
  "summary": "Bangalore restaurants have consistently high ratings.",
  "business_insight": "Online delivery restaurants tend to receive more customer engagement.",
  "key_insights": [
    "North Indian cuisine dominates top-rated listings.",
    "Mid-range restaurants receive the highest votes."
  ]
}
```

---

# ⚡ n8n Workflow Automation

The entire AI pipeline is automated using **n8n workflows**.

<p align="center">
  <b>n8n Workflow</b>
</p>

<p align="center">
  <img src="https://ik.imagekit.io/vtwmik0pw/Screenshot%202025-08-24%20222404.png?updatedAt=175839145916" alt="n8n Workflow" width="850"/>
</p>

## Workflow Architecture

```text
User Query
   ↓
Frontend (Lovable)
   ↓
Webhook Trigger (n8n)
   ↓
AI SQL Agent
   ↓
PostgreSQL Database
   ↓
Insight Generation Agent
   ↓
Structured JSON Response
   ↓
Frontend Visualization
```

### Workflow Capabilities

- Natural language processing
- Dynamic SQL generation
- PostgreSQL execution
- AI insight generation
- JSON output parsing
- Error handling & validation

---

# 🖥️ Frontend Application

A modern frontend interface was developed using **Lovable** to provide a conversational analytics experience.

## Frontend Highlights

- 💬 Chat-style analytics interface
- 📊 AI-powered insight cards
- ⚡ Real-time query execution
- 📱 Responsive UI
- 🔍 Natural language querying
- 📈 Structured business analytics display

### Example UI Prompt

> “Ask business questions in plain English and get AI-powered SQL insights instantly.”

---

# 📊 SQL Analysis Performed

## 1️⃣ Rating Distribution & Trends

- Average rating by city and price range
- Best and worst-rated cuisines
- Top voted restaurants
- Rating distribution analysis

## 2️⃣ Comparative Analysis

- Delivery vs non-delivery ratings
- Table booking impact on ratings
- Cost vs rating relationship
- Price-range-based comparisons

## 3️⃣ Aggregation & Segmentation

- Cuisine-wise average ratings
- Locality-wise restaurant counts
- City leaderboards
- Rating segmentation:
  - 🥇 Gold: 4.5–5
  - 🥈 Silver: 4–4.4
  - 🥉 Bronze: 3–3.9

## 4️⃣ Outlier Detection

- High-rated low-vote restaurants
- Overrated restaurants
- Expensive but poorly rated restaurants

---

# 📈 Power BI Dashboard

An interactive **Power BI dashboard** was created for visual exploration of restaurant trends and KPIs.

## Dashboard Features

- City-wise filtering
- Cuisine-based exploration
- Rating distribution charts
- Cost analysis
- Restaurant leaderboards
- Interactive drill-throughs

<p align="center">
  <b>Zomato Power BI Dashboard</b>
</p>

<p align="center">
  <img src="https://ik.imagekit.io/vtwmik0pw/Screenshot%202025-08-24%20222404.png?updatedAt=1758391459169" alt="Zomato Dashboard" width="850"/>
</p>

---

# 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| 🧠 PostgreSQL | Database & SQL Analysis |
| ⚡ n8n | Workflow Automation |
| 🤖 Gemini AI / LLM | SQL & Insight Generation |
| 📊 Power BI | Dashboard & Visualization |
| 🎨 Lovable | Frontend UI |
| 🐍 JavaScript | Parsing & Automation |
| 📁 CSV/Excel | Dataset Handling |

---

# 📂 Project Structure

```bash
Zomato_AI_Analytics/
│
├── workflows/
│   ├── sql_query_agent.json
│   ├── insight_generation_agent.json
│
├── frontend/
│   ├── lovable_ui/
│
├── PowerBI_Dashboard/
│   ├── zomato_dashboard.pbix
│
├── SQL_Queries/
│
├── Data/
│   ├── zomato_data.csv
│
├── screenshots/
│   ├── workflow.png
│   ├── frontend_ui.png
│   ├── dashboard.png
│
└── README.md
```

---

# 💡 Business Value

This platform demonstrates how AI can simplify business analytics by allowing non-technical users to:
- Query databases without SQL knowledge
- Generate instant business insights
- Explore trends conversationally
- Make data-driven decisions faster

---

# 🔮 Future Improvements

- 🔐 User authentication
- 📡 Live database integration
- 📊 Advanced chart generation
- 🧠 Multi-agent orchestration
- ☁️ Cloud deployment
- 📈 Predictive analytics & forecasting
- 🎯 Role-based dashboards

---

# 📬 Author

Built as an AI-powered analytics and automation project focused on combining:
- Data Analytics
- AI Agents
- Workflow Automation
- Business Intelligence
- Conversational Analytics
