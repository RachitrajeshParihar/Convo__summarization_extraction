# Conversation Summarization & Structured Extraction with Groq API

This project provides a Jupyter/Colab Notebook that:
- Summarizes **user ↔ assistant conversations** into concise text.
- Extracts **structured JSON** including:
  - `intent`
  - `topics`
  - `sentiment`
  - `named_entities`
  - `action_items`
  - `confidence score`

---

##  Features
- Powered by [Groq](https://groq.com) API (**OpenAI SDK compatible**).
- Lightweight: **no frameworks**, just plain Python with `openai`-style calls or fallback to `requests`.
- **Robust retry** mechanism with exponential backoff.
- Supports **batch processing** of datasets with JSONL output.
- Includes **example conversations** for quick testing.

---

##  Requirements
Install dependencies:


pip install -r requirements.txt
##  Authentication
Before running, export your Groq API key:


export GROQ_API_KEY=gsk_your_real_key_here
Or create a .env file with:


GROQ_API_KEY=gsk_your_real_key_here

 Note:

- Only Groq API keys are required.

- You do not need an OpenAI API key.

- Groq keys start with gsk_....

- Use the grok API which has access to openAI's supproted models. This notebook does not provide any such API.

##  Usage
Run the notebook-

### In Google Colab:
Upload and open conv_extraction.ipynb.

### Locally in Jupyter:

jupyter notebook conv_extraction.ipynb

The notebook will:

1. Load sample conversations.

2. Summarize them.

3. Extract structured JSON.

4. Save outputs to results.jsonl.

##  Repo Structure
Convo__summarization_extraction/

├── Convo__summarization_extraction.ipynb   # Colab notebook

├── README.md

├── requirements.txt

├── .gitignore

└── LICENSE

## 📜 License
This project is licensed under the MIT License – see the LICENSE file for details.
