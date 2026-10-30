# Scam Message Investigator


## Overview

https://scamzzzz-agtvkd3yqfb3jex6trqjds.streamlit.app/

Scam Message Investigator is an AI-powered application that analyzes suspicious text messages and identifies potential scam indicators. It uses a locally running Large Language Model (LLM) through Ollama to investigate messages and explain warning signs.

The application helps users recognize suspicious messages, phishing attempts, fraudulent links, and social engineering tactics.

## Features

- AI-powered scam message analysis.
- Identifies suspicious words, urgent threats, and misleading claims.
- Detects potential phishing attempts and suspicious links.
- Explains warning signs in the submitted message.
- Uses a locally running LLM through Ollama.
- Provides a simple and user-friendly interface.
- Supports privacy-conscious local analysis when the model and application run locally.

## Technologies Used

- Python
- Ollama
- Large Language Models (LLMs)
- Streamlit (if used for the application interface)
- HTML and CSS (if used for UI styling)

## How It Works

1. Open the Scam Message Investigator application.
2. Paste a suspicious SMS, email, or other text message into the input box.
3. Submit the message for analysis.
4. The application sends the message to the locally running Ollama service.
5. The AI analyzes the message for potential scam indicators.
6. Review the results and warning signs provided by the application.

## Installation and Setup

### Prerequisites

- Python installed on your system.
- Ollama installed and running.
- A compatible language model downloaded through Ollama.

### Step 1: Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd scam-message-investigator
```

Replace `YOUR_GITHUB_REPOSITORY_URL` with your actual GitHub repository URL.

### Step 2: Install Dependencies

If your project contains a `requirements.txt` file, run:

```bash
pip install -r requirements.txt
```

### Step 3: Install Ollama

Download and install Ollama from its official website:

https://ollama.com/

### Step 4: Download a Language Model

For example, to download the Llama 3.2 model, run:

```bash
ollama pull llama3.2
```

Make sure the model name matches the one configured in your application.

### Step 5: Start Ollama

Run:

```bash
ollama serve
```

If Ollama is already running automatically, you do not need to start it again.

### Step 6: Run the Application

If your main application file is `app.py` and it uses Streamlit, run:

```bash
streamlit run app.py
```

If your project uses a different framework, follow the corresponding startup instructions.

## Example

### Input

```text
URGENT! Your bank account will be blocked today because your KYC verification is incomplete. Click this link immediately to update your details and avoid account suspension.
```

### Expected Analysis

The application may identify the following warning signs:

- Urgent language intended to create panic.
- Threats of account suspension.
- Requests to update KYC information through a link.
- Pressure to act immediately.

The message should be treated as suspicious until independently verified.

## Applications

- Identifying suspicious SMS messages.
- Analyzing potential phishing emails.
- Learning to recognize social engineering techniques.
- Improving awareness of online scams.
- Supporting cybersecurity education.

## Privacy

The application is designed to use a locally running language model through Ollama. When all processing remains local, submitted messages do not need to be sent to an external AI provider.

Privacy depends on the application's implementation and any additional services it uses.

## Limitations

- AI-generated results may not always be accurate.
- Genuine messages may sometimes be flagged as suspicious.
- Sophisticated scam messages may not always be detected.
- A suspicious message should be verified through official channels.
- Never share passwords, OTPs, PINs, or banking credentials through suspicious links.

## Future Enhancements

- Scam risk scoring.
- Multilingual scam message detection.
- Detection of suspicious URLs.
- Message classification into scam and legitimate categories.
- Analysis of email messages and uploaded screenshots.
- Improved explanations and recommendations.

## Conclusion

Scam Message Investigator demonstrates how locally running Large Language Models can help analyze suspicious messages and explain common scam indicators. It aims to improve digital safety awareness and help users make more informed decisions when they receive unexpected messages.
