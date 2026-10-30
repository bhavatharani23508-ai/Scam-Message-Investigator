# Scam Message Investigator

### AI-Based Suspicious Message Detection System

## Overview

Scam Message Investigator is a Python-based application that uses Artificial Intelligence to analyze suspicious SMS messages, emails, job offers, and online messages. It uses the Gemma 3 1B language model through Ollama to identify potential scam indicators and provide safety recommendations.

## Features

- Analyzes suspicious messages.
- Identifies possible scam indicators.
- Classifies messages into Low, Medium, and High Concern.
- Explains warning signs and supporting evidence.
- Provides safety recommendations.
- Generates downloadable JSON reports.
- Uses a locally running AI model.

## Technologies Used

- Python
- Streamlit
- Ollama
- Gemma 3 1B
- Requests
- JSON

## Project Structure

```text
Scam Message Investigator/
│
├── app.py
├── requirements.txt
└── README.md
```

## Installation

**1. Install the required software**

- Python 3.10 or newer
- Visual Studio Code
- Ollama

**2. Download the AI model**

```bash
ollama pull gemma3:1b
```

**3. Install dependencies**

```bash
python -m pip install -r requirements.txt
```

**4. Run the application**

```bash
python -m streamlit run app.py
```

Open the application at:

http://localhost:8501

## Working Process

1. Enter a suspicious message.
2. Click the Investigate Message button.
3. The Gemma AI model analyzes the message.
4. The application identifies possible warning signs.
5. A concern level and investigation report are displayed.
6. Download the report in JSON format.

## Concern Levels

| Level | Description |
|---|---|
| High Concern | Strong indicators of a possible scam |
| Medium Concern | Potentially suspicious activity |
| Low Concern | No obvious warning signs identified |

## Limitations

- The application analyzes message text only.
- It does not independently verify URLs or sender identities.
- AI predictions may not always be accurate.
