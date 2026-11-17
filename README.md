# PrepAI — Streamlit + LLM experiments

A repository of experiments with Streamlit, OpenAI APIs, and LangChain. These examples explore building conversational interfaces, file Q&A, search-assisted chat, prompt templates, and feedback flows.

> **Current repository scope:** The checked-in code contains Streamlit LLM examples. It does not currently demonstrate the complete role-specific interview practice, personalized study-plan generation, or progress dashboards described in my broader PrepAI plans.

## Contents

- `Chatbot.py` — Streamlit chat interface using the OpenAI API
- `1_File_Q&A.py` — file question-answering experiment
- `2_Chat_with_search.py` — chat with search experiment
- `3_Langchain_Quickstart.py` — LangChain introduction
- `4_Langchain_PromptTemplate.py` — prompt template experiment
- `5_Chat_with_user_feedback.py` — user-feedback experiment
- `app_test.py` — Streamlit app testing experiments

## Run locally

```bash
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
pip install -r requirements.txt
streamlit run Chatbot.py
```

Supply your own OpenAI API key in the app sidebar. Never commit credentials. API usage may incur costs.

## Technical focus

Python · Streamlit · OpenAI API · LangChain · UI state · API integration · application testing

## Attribution

The repository includes examples based on the [Streamlit LLM examples](https://github.com/streamlit/llm-examples). Original upstream links remain in some source files. This README describes the checked-in code rather than claiming all example code was authored from scratch.

