📬 Gmail Summary Automation with n8n and Google Gemini
This workflow automates the process of summarizing recent Gmail messages using Google's Gemini language model via n8n.

🔁 Workflow Name
My workflow 2

🧩 Workflow Overview
⏰ Schedule Trigger
Executes daily at 8 PM.

📥 Gmail Node
Retrieves the latest 10 email snippets from your Gmail inbox.

📊 Aggregate Node
Extracts and prepares the snippet fields from the emails.

🧠 Summary Agent
Uses Google Gemini (PaLM) via LangChain to generate a concise summary of the email snippets.

📝 Gmail Draft Node
Sends the generated summary as a draft email with the subject "Your Gmail Summary".

⚙️ Technologies Used
n8n

Gmail API (OAuth2)

LangChain Agent with Google Gemini

Google Gemini (PaLM)

Aggregate Node for data shaping

🧪 Setup Instructions
Clone or import the workflow into your n8n instance.

Configure the following credentials:

gmailOAuth2: Link to your Gmail account.

googlePalmApi: Access to Gemini API.

Ensure the schedule is correct (default is 8 PM).

Activate the workflow.

🛡️ Notes
Ensure required Gmail and Gemini API credentials are properly set up and authorized in your n8n instance.

This workflow creates drafts and does not auto-send emails.

Modify the prompt or output format if needed to suit your email summarization style.
