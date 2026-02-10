🧠 AI Health Assistant – Agentic LLM System for Medical Analysis
<img width="900" alt="image" src="https://github.com/user-attachments/assets/b7c87bf6-dfff-42fe-b8d1-9be9e6c7ce86">

An individual-level Generative AI project that demonstrates how LLM-based AI agents can collaborate to analyze complex medical reports.
The system simulates a multi-specialist medical review by running domain-specific AI agents in parallel and combining their insights into structured diagnostic suggestions.

⚠️ Disclaimer
This project is created strictly for educational and research purposes.
It does not provide medical advice and must not be used in real clinical decision-making.

🚀 Project Overview

The goal of this project is to explore Agentic AI using Large Language Models (LLMs).
Instead of relying on a single AI response, the system uses multiple specialized agents, each acting like a medical expert, to analyze the same patient report from different perspectives.

Each agent produces an independent analysis, and the system aggregates the results to generate possible health concerns with reasoning.

🤖 AI Agents Used
🫀 Cardiologist Agent

Analyzes cardiac-related symptoms

Looks for signs of heart rhythm issues or cardiovascular abnormalities

Suggests possible cardiac tests or monitoring directions

🧠 Psychologist Agent

Evaluates psychological and stress-related symptoms

Identifies possible anxiety or panic-related conditions

Suggests mental health evaluation approaches

🌬 Pulmonologist Agent

Focuses on respiratory indicators

Assesses breathing patterns and lung-related symptoms

Recommends further respiratory evaluation if needed

⚙️ How the System Works

A medical report (synthetic sample) is provided as input

The report is sent simultaneously to all AI agents using multithreading

Each agent independently analyzes the report using an LLM

The outputs are collected and summarized into:

Possible health issues

Supporting reasoning from each agent

This architecture highlights parallel reasoning, task delegation, and agent collaboration — key ideas in Agentic AI systems.

📁 Repository Structure
AI-Health-Assistant/
│
├── Medical Reports/   # Sample synthetic medical reports
├── Results/           # AI-generated diagnostic outputs
├── main.py            # Core execution script
├── requirements.txt   # Project dependencies
└── README.md

⚡ Quick Start
1️⃣ Clone the repository
git clone https://github.com/devanshrawat27/AI-Health-Assistant.git
cd AI-Health-Assistant

2️⃣ Set up virtual environment
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate
pip install -r requirements.txt

3️⃣ Configure API key

Create a file named apikey.env in the project root:

OPENAI_API_KEY=your_api_key_here

4️⃣ Run the project
python main.py

🧪 Key Concepts Demonstrated

Generative AI using Large Language Models

Agentic AI architecture

Parallel agent execution (threading)

Prompt engineering for domain-specific reasoning

Structured aggregation of multiple AI outputs

🔮 Possible Improvements

Add more specialist agents (Neurology, Endocrinology, etc.)

Support local LLMs (Llama, Mistral)

Convert outputs to structured JSON format

Add evaluation metrics and testing pipeline

Build a simple web UI for interaction

👨‍💻 Author

Devansh Rawat
B.Tech | Software Engineering
Focused on Generative AI, LLMs, and Agentic Systems
