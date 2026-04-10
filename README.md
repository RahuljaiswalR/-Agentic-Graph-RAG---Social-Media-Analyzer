# 🤖 Agentic Graph RAG - Social Media Analyzer

An intelligent AI-powered system that combines **Graph Analysis + Retrieval-Augmented Generation (RAG)** to analyze social media data and answer queries using both structured data and semantic understanding.

---

## 🚀 Features

* 📊 Data Analytics (Top users, engagement, likes, etc.)
* 🌐 Graph-based User Relationship Analysis
* ⏳ Time-based Filtering (Recent posts, trends)
* 📈 Insights (Trending topics, hashtags)
* 🤖 RAG-based AI Chat (semantic search using embeddings)
* 📊 Interactive Streamlit Dashboard

---

## 📁 Project Structure

```
agentic_graph_rag/
│
├── app.py                  # Main Streamlit app
├── data/
│   └── socialmedia.csv     # Dataset
│
├── src/
│   ├── agent.py            # Main agent logic
│   ├── data_loader.py      # Load dataset
│   ├── graph_builder.py    # Build user graph
│   ├── embeddings.py       # Generate embeddings
│   ├── vector_store.py     # FAISS index
│   └── graph_viz.py        # Graph visualization
│
├── requirements.txt
└── README.md
```

---

## ⚙️ Installation Guide (Step-by-Step)

### 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/agentic_graph_rag.git
cd agentic_graph_rag
```

---

### 2️⃣ Create Virtual Environment

```bash
python -m venv rag_env
```

Activate environment:

👉 Windows:

```bash
rag_env\Scripts\activate
```

👉 Mac/Linux:

```bash
source rag_env/bin/activate
```

---

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

### 4️⃣ Run the Project

```bash
streamlit run app.py
```

👉 Open in browser:

```
http://localhost:8501
```

---

## 📊 Dataset Description

This project uses a **social media dataset** with the following columns:

* User ID, Username
* Platform (Instagram, Twitter, etc.)
* Post ID, Post Text
* Post Timestamp
* Likes/Reactions, Comments, Shares/Retweets
* Hashtags, Mentions
* Media Type, Media URL
* Location, Privacy Settings
* User Followers, Following
* User Engagement, Interactions, Activity

---

## 🤖 How the System Works

### 🔹 Step 1: Data Processing

* CSV file is loaded using Pandas
* Data is cleaned and structured

### 🔹 Step 2: Graph Creation

* Users are connected based on interactions
* Graph built using NetworkX

### 🔹 Step 3: Embeddings + Vector Search

* SentenceTransformer generates embeddings
* FAISS used for fast similarity search

### 🔹 Step 4: Intelligent Agent

The system detects query type:

* Analytics → DataFrame operations
* Graph → Network analysis
* Time → Date filtering
* Insight → NLP analysis
* RAG → Semantic search

### 🔹 Step 5: Response Generation

* Structured queries → Pandas results
* Graph queries → Relationship answers
* RAG queries → AI-based responses

---

## 💬 Example Queries

### 📊 Analytics Queries

* Top 5 users with highest engagement
* Top 10 users with highest likes
* Average engagement score kya hai?
* Total number of posts kitne hain?
* Lowest engagement wale users kaun hain?
* Most active users kaun hain?
* Kis platform par sabse zyada engagement hai?

---

### ⏳ Time-Based Queries

* Show posts from last 5 days
* Recent posts from last 7 days

---

### 🌐 Graph Queries

* Relation between user1 and user2
* Is Rahul connected with Aman?

---

### 📈 Insight Queries

* What are trending topics?
* Most common words in posts

---

### 🤖 RAG Queries

* What is social media engagement?
* How to increase engagement?

---

## 🛠️ Technologies Used

* Python 🐍
* Streamlit 📊
* Pandas 🧮
* NumPy
* Scikit-learn
* Sentence Transformers 🤖
* FAISS 🔍
* NetworkX 🌐
* Matplotlib 📉

---

## 📦 Requirements

Create a `requirements.txt` file with:

```
streamlit
pandas
numpy
scikit-learn
sentence-transformers
faiss-cpu
networkx
matplotlib
```

---

## 🧠 Key Improvements Done

* ✅ Fixed incorrect column mapping
* ✅ Improved query intent detection
* ✅ Added datetime filtering support
* ✅ Corrected aggregation logic
* ✅ Enhanced RAG + Analytics routing

---

## 🎯 Future Enhancements

* NLP-based advanced query understanding
* Better UI with charts and filters
* LLM-based reasoning system
* Real-time social media data integration

---

## 👨‍💻 Author

**Rahul Jaiswal**

---

## 🎤 Interview Explanation (Use This)

> "This project is an Agentic Graph RAG system that intelligently routes user queries between structured analytics, graph-based relationship analysis, and semantic retrieval using embeddings."

---

## ⭐ Support

If you like this project:

⭐ Star the repository
🍴 Fork it
📢 Share it

---

## 🚀 Final Note

This project demonstrates:

* Data Analytics
* Graph Intelligence
* AI + RAG Integration

👉 A complete end-to-end AI system.
