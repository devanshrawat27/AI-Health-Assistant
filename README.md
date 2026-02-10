# 🧠 AI Health Assistant  
### Agentic LLM System for Medical Analysis

<img width="900" alt="AI Health Assistant" src="https://github.com/user-attachments/assets/b7c87bf6-dfff-42fe-b8d1-9be9e6c7ce86">

An **individual-level Generative AI project** that demonstrates how **LLM-based AI agents** can collaboratively analyze complex medical reports.  
The system simulates a **multi-specialist medical review** by running domain-specific AI agents in parallel and combining their insights into structured diagnostic suggestions.

> ⚠️ **Disclaimer**  
> This project is created **strictly for educational and research purposes**.  
> It does **NOT** provide medical advice and must **NOT** be used for real clinical decisions.

---

## 🚀 Project Overview

This project explores **Agentic AI** using **Large Language Models (LLMs)**.  
Instead of relying on a single AI response, multiple specialized agents analyze the same medical report from different perspectives.

Each agent produces an independent analysis, and the system aggregates their outputs to generate **possible health conditions with reasoning**.

---

## 🤖 AI Agents

### 🫀 Cardiologist Agent
- Analyzes cardiac-related symptoms  
- Detects potential heart rhythm or cardiovascular issues  
- Suggests possible cardiac tests or monitoring directions  

### 🧠 Psychologist Agent
- Evaluates psychological and stress-related symptoms  
- Identifies possible anxiety or panic-related conditions  
- Suggests mental health assessment approaches  

### 🌬 Pulmonologist Agent
- Focuses on respiratory indicators  
- Assesses breathing patterns and lung-related symptoms  
- Recommends further respiratory evaluation if needed  

---

## ⚙️ How It Works

1. A synthetic medical report is provided as input  
2. The report is sent **simultaneously** to all AI agents using multithreading  
3. Each agent independently analyzes the report using an LLM  
4. The system aggregates all outputs into:
   - Possible health issues  
   - Supporting reasoning from each specialist agent  

This architecture demonstrates:
- Agent collaboration  
- Parallel reasoning  
- Task delegation using LLMs  

---

## 📁 Repository Structure

AI-Health-Assistant/
│
├── Medical Reports/ # Sample synthetic medical reports
├── Results/ # AI-generated diagnostic outputs
├── main.py # Core execution script
├── requirements.txt # Project dependencies
├── .gitignore
└── README.md


---

## ⚡ Quick Start

### 1️⃣ Clone the repository
```bash
git clone https://github.com/devanshrawat27/AI-Health-Assistant.git
cd AI-Health-Assistant

2️⃣ Create virtual environment
python -m venv venv
source venv/bin/activate      # On Windows: venv\Scripts\activate
pip install -r requirements.txt

3️⃣ Configure API key

Create a file named apikey.env in the project root:

OPENAI_API_KEY=your_api_key_here

4️⃣ Run the application
python main.py

🧪 Key Concepts Demonstrated

Generative AI using Large Language Models

Agentic AI architecture

Parallel agent execution (threading)

Prompt engineering for domain-specific reasoning

Aggregation of multi-agent outputs

🔮 Future Improvements

Add more specialist agents (Neurology, Endocrinology, etc.)

Support local LLMs (Llama, Mistral)

Convert outputs into structured JSON format

Add evaluation metrics and automated testing

Build a simple web-based UI
👨‍💻 Author

Devansh Rawat
B.Tech | Software Engineering
Focused on Generative AI, LLMs, and Agentic AI Systems
