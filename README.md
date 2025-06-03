# Project: Search and Lead Automation
# 🔍 About the Project
This project automates the process of lead generation and personalization for cold email outreach using n8n. It integrates multiple tools to extract, summarize, and personalize business information from the web in a structured and scalable way.

#🛠️ Key Features
🔁 Automated Workflow using n8n

📄 Reads business queries (City + Store Type) from Google Sheets

🌐 Extracts business data from Google Maps using Apify API

🌍 Filters businesses with valid websites

🕷️ Scrapes website content

🧠 Summarizes web content using OpenAI GPT-4

✍️ Generates customized cold email openers ("icebreakers") based on content

📊 Saves enriched leads back into Google Sheets

# ⚙️ Tech Stack
n8n: Workflow automation

Google Sheets: Data input/output

Apify API: Google Maps scraper

OpenAI API (GPT-4): Summarization and personalization

JavaScript (code nodes): Custom filtering and processing

#  📈 Workflow Summary
Triggered manually or on schedule.

Reads location and business type from Google Sheets.

Sends data to Apify Google Maps extractor.

Cleans and filters businesses with active websites.

Scrapes HTML content of websites.

Summarizes the content with GPT.

Builds a cold-email icebreaker using another GPT prompt.

Appends full lead information back to a new sheet.

#📁 Google Sheets Structure
Input Sheet: Includes City, Store type.

# Output Sheet: Includes Title, Address, Website, and generated IceBreaker.


![Capturooo](https://github.com/user-attachments/assets/20c325a6-bd48-4213-a95d-b0c5f241ff0c)

🧠 Example IceBreaker Output
json


{![get search](https://github.com/user-attachments/assets/6f1c7764-a15b-4a02-9ac2-33556ceebaaa)

  "icebreaker": "Hey Sarah. Love BrightBean—noticed you're also into ethical sourcing. Got something you might dig.\n\nI've been diving into your setup and couldn't help but notice how much weight you put on transparency (at least judging by how you highlight your local partnerships). Built a lightweight AI automation system that clears grunt work, connects tools, and keeps ops lean. It's dead simple, fast to deploy, and I think it lines up with your focus on sustainable growth."
}
