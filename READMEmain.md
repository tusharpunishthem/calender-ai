# calender_assistant
 calender ai assistant


# 📅 Calendar Assistant (Gradio + Cohere + Google Calendar + Gmail)

An AI-powered Calendar Assistant built using **Gradio**, **Cohere NLP**, and **Google Calendar/Gmail API**. It can:
- Parse natural language commands like "Show me free time tomorrow"
- List calendar events for today/tomorrow/week
- Create events and send email notifications
- Run locally or deploy publicly

---

## 🚀 Features
- 🧠 Cohere NLP command understanding
- 📆 Google Calendar Integration
- 📧 Gmail notifications on event creation
- 🎤 Gradio frontend interface

---

## 📁 Project Structure
calendar-assistant/
│
├── generate_token.py        # 🔑 Run first to generate token.pickle from credentials.json
├── main.py                  # 🚀 Launch Gradio-based Calendar Assistant
├── nlp_parser.py            # 🧠 Cohere NLP command interpreter
├── calendar_assistant.py    # 📆 Handles Google Calendar & Gmail API logic
├── requirements.txt         # 📦 Python dependencies
├── .env                     # 🗝️ Cohere API key (❌ DO NOT COMMIT)
├── credentials.json         # 🔐 Google OAuth client secret (❌ DO NOT COMMIT)
├── token.json / token.pickle# 🔒 OAuth tokens (❌ Auto-generated, DO NOT COMMIT)
└── README.md                # 📘 This file


calendar-assistant/ │ ├── generate_token.py # Run FIRST to generate token.pickle using credentials.json ├── main.py # Runs the Gradio app ├── nlp_parser.py # Cohere-based NLP command parser ├── calendar_assistant.py # Google Calendar + Gmail integration ├── requirements.txt # Python dependencies ├── .env # Cohere API Key (Do NOT commit) ├── credentials.json # Google OAuth file (Do NOT commit) ├── token.json / token.pickle# Generated tokens (Do NOT commit) └── README.md # This file

yaml
Copy
Edit

---

## 🧰 Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/YOUR_USERNAME/calendar-assistant.git
cd calendar-assistant
2. Install Dependencies
bash
Copy
Edit
pip install -r requirements.txt
3. Add .env with Cohere Key
Create a .env file in the root:

env
Copy
Edit
COHERE_API_KEY=your-cohere-api-key-here
---

1. Go to [https://dashboard.cohere.com/api-keys](https://dashboard.cohere.com/api-keys)
2. Sign in with your email or GitHub
3. Copy your default API key (or create a new one)
4. Create a file called `.env` in your project root and paste:

4. Get Google OAuth credentials.json
Go to Google Cloud Console

Enable:

Google Calendar API

Gmail API

Create OAuth client ID > Application: Desktop App

Download credentials.json and place it in root

5. 🔑 Generate Token (Run Once)
Run the following script to authenticate Google:

bash
Copy
Edit
python generate_token.py
This will create token.pickle for future access.

6. 🚀 Run the App
bash
Copy
Edit
python main.py
🧪 Try These Commands
What are today's events?

Show meetings tomorrow

Find 30-minute free slots

Create an event for 5 PM


