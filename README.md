# PrepAI — AI-Powered Technical Interview Preparation

**An AI-powered platform for personalized technical interview practice, study planning, and progress tracking.**

PrepAI is a Python-based application that uses large language models (LLMs) to make technical interview preparation more personalized and structured.

Built with Streamlit, the OpenAI API, and SQLite, PrepAI brings together role-specific interview questions, AI-generated feedback, personalized study schedules, and progress analytics in one interactive interface.

The project explores practical applications of generative AI, API integration, backend development, and persistent data storage.

## Features

### AI-Powered Interview Practice

- Generate technical interview questions based on engineering role, topic, and difficulty.
- Submit written responses for AI-generated feedback.
- Receive suggestions for improving technical explanations and problem-solving approaches.
- Track completed practice sessions and self-reported confidence.

### Personalized Study Plan Generator

- Generate study plans tailored to target roles and experience levels.
- Customize preparation duration, technical topics, and weekly study hours.
- Receive structured weekly learning recommendations.
- Export generated study plans in Markdown format.

### Progress Tracking Dashboard

- Record interview practice activity using SQLite.
- Track practice frequency, topics, and confidence levels.
- Visualize preparation history using Streamlit charts.
- Export practice records to CSV for further analysis.

## Tech Stack

| Technology | Application |
|---|---|
| Python | Core application logic |
| Streamlit | Interactive frontend and dashboard |
| OpenAI API | LLM-powered question generation, feedback, and study planning |
| SQLite | Persistent local storage |
| Pandas | Data processing and progress analysis |
| LangChain | LLM experimentation and prompt workflows in supporting examples |
| Git / GitHub | Version control |

## System Architecture

```text
                  USER
                    |
                    v
            Streamlit Interface
                    |
          +---------+---------+
          |         |         |
          v         v         v
     Interview    Study     Progress
      Practice    Planner   Dashboard
          |         |         |
          v         v         v
       OpenAI API         SQLite Database
          |                   |
          v                   v
    AI-Generated          Practice Records
    Questions and         and Analytics
       Feedback
```

### Application Workflow

1. **User Input:** Users select an engineering role, technical topic, difficulty, or study goal.
2. **LLM Integration:** The application sends structured prompts to the OpenAI API to generate relevant content.
3. **Response Handling:** AI-generated questions, feedback, and study plans are displayed through Streamlit.
4. **Data Persistence:** Practice sessions are stored in a local SQLite database.
5. **Progress Analysis:** Stored records are processed and visualized through the progress dashboard.

## Getting Started

### Prerequisites

- Python 3.10+
- pip
- OpenAI API key

### Installation

Clone the repository:

```bash
git clone https://github.com/OnahiJoel-Ukama/PrepAI.git
cd PrepAI
```

Create and activate a virtual environment:

**Windows**

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

**macOS / Linux**

```bash
python3 -m venv .venv
source .venv/bin/activate
```

Install the application dependencies:

```bash
pip install -r requirements-prepai.txt
```

### Run PrepAI

```bash
streamlit run prepai_app.py
```

Open the local URL displayed in your terminal.

Enter your OpenAI API key in the application's sidebar to enable AI-powered features. API usage may incur charges.

## Project Structure

```text
PrepAI/
├── prepai_app.py
├── requirements-prepai.txt
├── README.md
│
├── Chatbot.py
├── 1_File_Q&A.py
├── 2_Chat_with_search.py
├── 3_Langchain_Quickstart.py
├── 4_Langchain_PromptTemplate.py
├── 5_Chat_with_user_feedback.py
└── app_test.py
```

The repository also includes earlier Streamlit and LangChain experiments exploring conversational interfaces, retrieval, prompt templates, and feedback collection.

## Engineering Highlights

### Generative AI Integration

Integrated an LLM API into an interactive application to generate technical questions, evaluate written responses, and produce personalized study plans.

### Backend Development and Data Persistence

Implemented application logic for managing practice sessions and storing structured progress records in SQLite.

### Data Processing and Visualization

Used Pandas and Streamlit to transform stored activity data into progress metrics, visualizations, and downloadable records.

### Application State Management

Used Streamlit session state to coordinate user interactions, generated content, and practice workflows.

## Current Limitations

- AI feedback is advisory and does not replace verified coding assessments.
- Submitted code is not executed against automated test cases.
- Practice records are stored locally rather than in a cloud-hosted database.
- The application does not currently provide multi-user authentication.

## Future Improvements

- Automated coding assessments and secure code execution
- Adaptive question recommendations based on practice history
- Cloud deployment using Google Cloud Run
- Cloud-hosted PostgreSQL for persistent multi-user data
- User authentication and personalized profiles
- Exploration of Vertex AI for managed generative AI integration

## Why I Built PrepAI

Preparing for technical interviews requires more than solving individual problems. It also involves identifying knowledge gaps, practicing explanations, and maintaining consistency over time.

I built PrepAI to explore how generative AI could support that learning process through personalized questions, feedback, and structured study plans.

The project has allowed me to apply Python, API integration, data persistence, and interactive application development to a practical problem while continuing to explore the capabilities and limitations of LLM-powered software.

## Attribution

This repository includes experiments adapted from the [Streamlit LLM Examples](https://github.com/streamlit/llm-examples) repository. Those examples are distinct from the PrepAI application features described above.

---

**Built with Python, Streamlit, OpenAI API, SQLite, and Pandas.**
