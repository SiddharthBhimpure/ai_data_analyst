# 🤖 AI Data Analyst

An AI-powered Data Analyst that converts natural language questions into SQL queries and retrieves insights from a database. The project leverages **LangChain**, **Ollama (DeepSeek-R1)**, **SQLAlchemy**, and **SQLite** to provide an intelligent interface for querying structured data without writing SQL manually.

---

## 📌 Features

* 💬 **Natural Language to SQL:** Convert plain English questions into SQL queries using an LLM.
* 🗄️ **Automatic Database Schema Extraction:** Dynamically extracts database tables and columns using SQLAlchemy.
* 🤖 **Local LLM with Ollama:** Uses the DeepSeek-R1 model locally through Ollama for privacy and offline usage.
* 📊 **SQLite Database Integration:** Executes generated SQL queries on an Amazon sales database.
* ⚡ **LangChain Prompt Pipeline:** Uses prompt templates and LLM chaining for structured SQL generation.
* 🔍 **Schema-Aware Query Generation:** Restricts SQL generation to the available database schema for improved accuracy.
* 🧠 **AI-Powered Data Analysis:** Enables users to retrieve business insights using natural language instead of SQL.

---

## 🛠️ Tech Stack

* **Python**
* **LangChain**
* **Ollama**
* **DeepSeek-R1 (1.5B)**
* **SQLAlchemy**
* **SQLite**
* **Regex (Response Cleaning)**

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/SiddharthBhimpure/ai_data_analyst.git

cd ai_data_analyst
```

### 2. Create a virtual environment

Using **uv** (Recommended)

```bash
uv venv
```

Activate the virtual environment

**Windows**

```bash
.venv\Scripts\activate
```

**Linux / macOS**

```bash
source .venv/bin/activate
```

---

### 3. Install dependencies

Using **uv**

```bash
uv sync
```

or using pip

```bash
pip install -r requirements.txt
```

---

### 4. Install Ollama

Download and install Ollama from:

https://ollama.com

Pull the required model:

```bash
ollama pull deepseek-r1:1.5b
```

Verify the installation:

```bash
ollama run deepseek-r1:1.5b
```

---

## ▶️ Usage

### 1. Generate the Database

Run the script to create and populate the SQLite database.

```bash
python database.py
```

---

### 2. Start the AI Data Analyst

```bash
python main.py
```

---

### 3. Ask Questions

Example queries:

* Show all products costing more than ₹1000.
* Which category generated the highest revenue?
* Show the top 5 selling products.
* What is the total revenue?
* List all orders placed in January.
* Which customer placed the highest number of orders?

---

## 📂 Project Structure

```text
ai_data_analyst/
│
├── amazon.db
├── database.py
├── main.py
├── requirements.txt
├── README.md
├── .gitignore
├── LICENSE
└── ...
```

---

## 🚀 Future Improvements

* 📈 Interactive dashboard with Streamlit
* 📊 Data visualization using Plotly/Matplotlib
* 🌐 REST API with FastAPI
* 💾 Conversation memory
* 🔄 Multi-database support (PostgreSQL, MySQL)
* 📑 CSV & Excel data analysis
* ☁️ Cloud deployment

---

## 👤 Author

**Siddharth Bhimpure**

🎓 B.E. in Artificial Intelligence & Data Science
