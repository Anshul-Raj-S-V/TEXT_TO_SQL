## Text-to-SQL App 🧠 

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.11+-blue.svg" alt="Python"/>
  <img src="https://img.shields.io/badge/SQLite-3-lightgrey.svg" alt="SQLite"/>
  <img src="https://img.shields.io/badge/LangChain-Framework-green.svg" alt="LangChain"/>
  <img src="https://img.shields.io/badge/Groq-LLM-orange.svg" alt="Groq"/>
  <img src="https://img.shields.io/badge/dotenv-Environment%20Variables-blue.svg" alt="dotenv"/>
</p>

> 🧩 Convert natural language queries into SQL commands and retrieve results directly from a SQLite database using **Llama 3.3 via Groq**.

---

## 🚀 Overview

The **Text-to-SQL App** enables users to interact with databases using **plain English**.
It leverages **LangChain** and **Groq’s Llama 3.3 model** to translate natural language into **SQL queries**, executing them instantly on a **SQLite** database.

---

## 🧩 Tech Stack

| Category                  | Technology                                                                                                                 |
| ------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| 💻 **Language**           | [![Python](https://img.shields.io/badge/Python-3.11+-blue.svg)](https://www.python.org/)                                   |
| 🗄️ **Database**          | [![SQLite](https://img.shields.io/badge/SQLite-3-lightgrey.svg)](https://www.sqlite.org/)                                  |
| 🧠 **LLM Framework**      | [![LangChain](https://img.shields.io/badge/LangChain-Framework-green.svg)](https://www.langchain.com/)                     |
| ⚙️ **Model API**          | [![Groq](https://img.shields.io/badge/Groq-LLM-orange.svg)](https://groq.com/)                                             |
| 🌱 **Environment Loader** | [![dotenv](https://img.shields.io/badge/dotenv-Environment%20Variables-blue.svg)](https://pypi.org/project/python-dotenv/) |

---

## 📁 Project Structure

```bash
TEXT_TO_SQL_APP/
│
├── main.py               # Main application file
├── student.db            # SQLite database
├── .env                  # Environment file containing Groq API key
├── requirements.txt      # List of dependencies
└── README.md             # Project documentation
```

---

## ⚙️ Installation

### 1️⃣ Clone the repository

```bash
git clone https://github.com/yourusername/TEXT_TO_SQL_APP.git
cd TEXT_TO_SQL_APP
```

### 2️⃣ Create and activate a virtual environment

```bash
python -m venv venv
venv\Scripts\activate   # On Windows
# or
source venv/bin/activate  # On macOS/Linux
```

### 3️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Set up `.env` file

Create a `.env` file in your project root and add your Groq API key:

```bash
GROQ_API_KEY=your_groq_api_key_here
```

---

## 🧠 How It Works

1️⃣ **User Input**
Enter a question like:

> “Show all students in Data Science course.”

2️⃣ **Query Generation**
Llama 3.3 model (via Groq) converts it into SQL:

```sql
SELECT * FROM STUDENT WHERE COURSE = "Data Science";
```

3️⃣ **Execution**
The SQL query runs on the `student.db` database.

4️⃣ **Output**
Results are fetched and displayed instantly.

---

## 🧪 Example

**Input:**

> How many students scored more than 80 marks?

**Generated SQL:**

```sql
SELECT COUNT(*) FROM STUDENT WHERE MARKS > 80;
```

**Output:**

```
3
```

---

## 🛠️ Requirements

* 🐍 Python 3.11+
* 🔑 Groq API key
* 🗄️ SQLite

Manual install (if needed):

```bash
pip install langchain langchain-groq langchain-core python-dotenv sqlite3
```

---

## ⚡ Features

✅ Converts natural language to valid SQL queries
✅ Powered by Llama 3.3 via Groq for precise conversions
✅ Simple local setup with SQLite
✅ Easily extendable to other databases

---

## 🧰 Future Enhancements

🚧 Add support for MySQL and PostgreSQL
🤖 Integrate visual result dashboards
🧮 Include query optimization suggestions

---




