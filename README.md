# InsightGen: Autonomous Data Analyst API

**InsightGen** is a high-performance AI agent designed to automate the initial stages of Exploratory Data Analysis (EDA). By combining **FastAPI** with **Generative AI (GPT-4o)**, it allows non-technical stakeholders to upload raw CSV datasets and extract statistical insights or visualizations using natural language queries.

This project demonstrates the integration of **Large Language Models (LLMs)** into robust **Data Pipelines**, bridging the gap between raw data and actionable business intelligence.

---

### 🚀 Key Features

* **Natural Language to Insight:** Transforms questions like *"What is the total profit?"* into Python analysis logic automatically.
* **Dynamic Visualization:** capable of generating on-the-fly charts (Bar, Line, Scatter) using **Matplotlib** based on user prompts.
* **Production-Ready Backend:** Built on **FastAPI** for high concurrency and Swagger UI documentation.
* **Seamless Data Handling:** Uses **Pandas** for efficient in-memory data processing and schema extraction.

---

### 📸 Live Demo

*Asking the agent to analyze a sales dataset for profitability:*

![InsightGen Demo](demo_result.png.png)

---

### 🛠️ Tech Stack

* **Framework:** Python, FastAPI, Uvicorn
* **AI & Logic:** OpenAI API (GPT-4o), Prompt Engineering
* **Data Processing:** Pandas, NumPy
* **Visualization:** Matplotlib
* **Tools:** Git, Postman/Swagger UI

---

### 💻 Installation & Usage

1.  **Clone the Repository**
    ```bash
    git clone [https://github.com/Anvesh-Git26/InsightGen.git](https://github.com/Anvesh-Git26/InsightGen.git)
    cd InsightGen
    ```

2.  **Install Dependencies**
    ```bash
    pip install -r requirements.txt
    ```

3.  **Set Up Environment**
    Export your OpenAI API Key:
    ```bash
    # Windows (PowerShell)
    $env:OPENAI_API_KEY="your-key-here"
    ```

4.  **Run the Server**
    ```bash
    uvicorn main:app --reload
    ```

5.  **Test the API**
    Open your browser to `http://127.0.0.1:8000/docs` to access the interactive Swagger UI.
    * **Endpoint:** `POST /analyze` - Upload a CSV and ask a text question.
    * **Endpoint:** `POST /plot` - Upload a CSV and ask for a chart.

---

### 📂 Project Structure

```text
InsightGen/
├── charts/              # Directory where generated plots are saved
├── main.py              # Core application logic and API endpoints
├── requirements.txt     # Python dependencies
├── demo_result.png      # Proof of work screenshot
└── README.md            # Project documentation
