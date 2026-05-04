# Make.com Automation Bots – SourceFellow

A collection of Make.com scenario blueprints used to automate business 
workflows at SourceFellow.

## 🤖 Bot 1 – LinkedIn Auto-Poster (Airtable + Groq + LinkedIn)

Automatically generates and publishes LinkedIn posts using AI.

**How it works:**
1. Fetches the next unused topic from an Airtable base (Topics table)
2. Sends the topic to Groq AI to generate a professional LinkedIn post
3. Publishes the post directly to LinkedIn (public, main feed)
4. Marks the topic as used in Airtable to avoid repetition

**Tools used:** Make.com · Airtable · Groq API · LinkedIn API

## ⚙️ Setup Instructions

1. Import the `.json` blueprint into your Make.com account
2. Reconnect your own Airtable, Groq, and LinkedIn connections
3. Set your Groq API key in the HTTP module headers
4. Make sure your Airtable base has a Topics table with: 
   `Topic`, `Category`, `Used`, `Last used date` columns

## 🔐 Security Note
Never commit API keys to this repo. 
Use Make.com's built-in connections or environment variables instead.s