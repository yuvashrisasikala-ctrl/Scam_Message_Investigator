
# Scam Message Investigator

## Abstract

Scam Message Investigator is an AI-based application that analyzes suspicious SMS messages, emails, job advertisements, and online messages. It helps users identify potential scam activities by examining message content and highlighting suspicious elements.

The application uses a locally running AI model through Ollama or a hosted AI model through the Groq API. It provides a concern level, message summary, warning signs, recommended safety actions, and analysis limitations.

## Introduction

Online scams are increasing through SMS, emails, fake job offers, and fraudulent websites. Many users find it difficult to identify suspicious messages.

Scam Message Investigator uses Artificial Intelligence to analyze message content and provide useful safety recommendations. It helps users understand potential risks before responding to suspicious messages.

## Objectives

- Analyze suspicious messages using AI.
- Identify possible scam warning signs.
- Detect suspicious links and urgent requests.
- Identify requests for OTP, passwords, and financial details.
- Provide recommended safety actions.
- Help users improve online safety awareness.

## Features

- AI-based scam message analysis.
- Low, Medium, and High Concern classification.
- Message category identification.
- Suspicious activity detection.
- Warning signs identification.
- Safety recommendations.
- JSON report generation.
- Local AI support using Ollama.
- Optional hosted AI support using Groq API.

## Technologies Used

| Technology | Purpose |
|---|---|
| Python | Application development |
| Streamlit | Web application interface |
| Ollama | Local AI model execution |
| Qwen2.5:3B | Local language model |
| Groq API | Hosted AI analysis |
| Requests | API communication |
| JSON | Structured AI response |

## System Requirements

- Python 3.10 or later
- Streamlit
- Requests
- Ollama
- Qwen2.5:3B model
- Internet connection for Groq API usage

## Project Structure

    Scam Message Investigator/
    |
    ├── app.py
    ├── requirements.txt
    └── README.md

## Installation

### 1. Clone the Repository

    git clone https://github.com/your-username/Scam-Message-Investigator.git

### 2. Navigate to the Project Folder

    cd Scam-Message-Investigator

### 3. Install Dependencies

    py -m pip install -r requirements.txt

### 4. Install Ollama

Download Ollama from:

https://ollama.com/

### 5. Download the AI Model

    ollama pull qwen2.5:3b

### 6. Run the Application

    py -m streamlit run app.py

The application will open in your browser at:

http://localhost:8501

## How It Works

1. The user enters a suspicious message.
2. The application sends the message to the AI model.
3. The AI examines the message for suspicious characteristics.
4. The AI generates a structured JSON response.
5. The application displays the investigation report.
6. The user receives safety recommendations.

## Workflow

    User Input
        |
        v
    Streamlit Interface
        |
        v
    AI Model (Ollama / Groq)
        |
        v
    Message Analysis
        |
        v
    JSON Response
        |
        v
    Scam Investigation Report
        |
        v
    Safety Recommendations

## Sample Input

    Congratulations! You have won a ₹25,00,000 lottery.
    Click this link immediately to claim your prize.
    Send your bank account details and OTP to receive the money.
    Offer expires in 10 minutes.

## Sample Output

    Concern Level: High Concern

    Message Category: Other

    Message Summary:
    The message claims that the user has won a lottery
    and requests sensitive financial information.

    Warning Signs:
    - Unexpected lottery announcement
    - Urgent request to claim a prize
    - Request for bank account details
    - Request for OTP

    Recommended Actions:
    - Do not share OTP or bank details.
    - Do not click suspicious links.
    - Verify the message using official sources.
    - Report the suspicious message.

## Advantages

- Easy-to-use interface.
- Provides quick message analysis.
- Supports local AI execution.
- Helps users recognize suspicious activities.
- Provides useful safety recommendations.

## Limitations

- AI predictions may not always be accurate.
- Unknown messages cannot always be classified correctly.
- The application does not verify the actual sender.
- Local AI analysis requires Ollama and a downloaded model.
- The application cannot guarantee that a message is completely safe.

## Future Enhancements

- Add image-based scam detection.
- Support multiple languages.
- Add URL reputation checking.
- Include email attachment analysis.
- Improve scam classification accuracy.
- Add scam report history.
- Develop a mobile-friendly interface.

## Conclusion

Scam Message Investigator is an AI-powered application designed to help users identify potential online scams. By analyzing suspicious messages and providing warning signs and safety recommendations, the application supports safer digital communication.

The project demonstrates the practical application of Artificial Intelligence, Natural Language Processing, and web development in improving online security awareness.
