# Email-Bot

This project is a simple AI-powered email bot that integrates OpenAI's GPT with the SimpleGmail API. The bot reads emails, generates replies based on the content, and sends automated responses. It leverages the power of OpenAI’s language model to streamline email management and improve productivity.

Features
Automatically reads emails from your Gmail inbox.
Generates context-aware replies using OpenAI's GPT model.
Sends AI-generated responses through Gmail.
Easy setup using the Gmail API and OpenAI.
Getting Started
Follow the steps below to set up and run the email bot on your local machine.

1. Clone the Repository
bash
Copy code
git clone https://github.com/varshat/Email-Bot/tree/main
cd email-bot
2. Setup Gmail API
Go to the Google Cloud Console.
Create a new project (if you don’t have one already).
Navigate to APIs & Services > Library.
Search for Gmail API and enable it.
Go to APIs & Services > Credentials and click Create Credentials.
Select OAuth 2.0 Client IDs and set the application type to Desktop app.
3. Create Desktop OAuth2 Credentials
After creating the OAuth 2.0 credentials, download the JSON file.
Move the downloaded JSON file into the project directory.
4. Rename JSON to client_secrets.json
bash
Copy code
mv your_downloaded_json_file.json client_secrets.json
5. Install Requirements
Install the required dependencies by running the following command:

bash
Copy code
pip install -r requirements.txt
6. Set OpenAI API Key
Make sure you have an OpenAI API key. Set it as an environment variable:

bash
Copy code
export OPENAI_API_KEY="your-api-key"
7. Run the Email Bot
Once everything is set up, run the bot using:

bash
Copy code
python email_bot.py
Project Structure
email_bot.py: Main script that connects to Gmail, reads emails, generates replies using OpenAI, and sends responses.
client_secrets.json: OAuth2 credentials required for Gmail API access.
requirements.txt: Python dependencies required for the project (SimpleGmail, OpenAI, etc.).
Environment Variables
Make sure to export your OpenAI API key before running the bot:

bash
Copy code
export OPENAI_API_KEY="your-api-key"
Future Enhancements
Add more personalized email responses based on specific user preferences.
Enable scheduling for checking emails and sending replies.
Implement smarter filtering for email content to prioritize important emails.
