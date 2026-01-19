🏡Here's the README without hashtags and asterisks:

AI Real Estate Assistant Workflow

A smart, automated workflow that helps real estate businesses manage leads and client interactions effortlessly using AI.

📋 What Does This Do?

This workflow automates your entire real estate lead management process:

1. Collects client information through a simple web form
2. Stores all data automatically in Google Sheets
3. Responds to client inquiries using an AI assistant (Google Gemini)
4. Books property viewing appointments in Google Calendar
5. Sends confirmation emails through Gmail

Think of it as having a 24/7 virtual assistant that never misses a lead!

Features

- Automated Data Collection - No more manual data entry
- AI-Powered Responses - Intelligent, personalized replies to client questions
- Smart Scheduling - Automatic appointment booking
- Email Automation - Instant confirmations and follow-ups
- Centralized Database - All client info in one organized spreadsheet

Built With

- n8n - Workflow automation platform
- Google Gemini AI - For intelligent client conversations
- Google Sheets - Client database management
- Google Calendar - Appointment scheduling
- Gmail - Email communications

What's Inside

The workflow consists of 7 connected nodes:

1. Form Trigger - Captures client submissions
2. Google Sheets Append - Saves data to spreadsheet
3. AI Agent - Processes client interests and responds intelligently
4. Gemini Chat Model - Powers the AI responses
5. Calendar Tool - Books appointments
6. Gmail Tool - Sends emails
7. Database Update Tool - Keeps records current

Getting Started

Prerequisites

Before you begin, you'll need:
- An n8n account (free tier works!)
- Google account with access to:
  - Google Sheets
  - Google Calendar
  - Gmail
- Google Gemini API key

Installation

1. Clone this repository
   ```bash
   git clone https://github.com/yourusername/ai-real-estate-workflow.git
   ```

2. Import into n8n
   - Open your n8n instance
   - Click on "Workflows" then "Import from File"
   - Select the workflow JSON file

3. Set Up Credentials
   
   You'll need to connect the following:
   - Google Sheets OAuth2
   - Google Calendar OAuth2
   - Gmail OAuth2
   - Google Gemini API

4. Configure Your Spreadsheet
   - Create a Google Sheet with columns: Name, Interests, Budget, Email, submittedAt, formMode
   - Update the documentId in the workflow with your sheet ID

5. Activate the Workflow
   - Click the "Active" toggle in n8n
   - Your workflow is now live!

Usage

For End Users (Clients)
1. Fill out the web form with their details
2. Receive instant AI-powered responses about properties
3. Get automatic appointment confirmations via email

For You (Real Estate Agent)
1. All leads automatically appear in your Google Sheet
2. Appointments sync to your Google Calendar
3. Monitor AI interactions and step in when needed

Use Cases

Perfect for:
- Real estate agencies managing multiple inquiries
- Individual agents looking to scale their business
- Property management companies
- Anyone wanting to automate lead follow-ups

Customization

You can easily customize:
- Form Fields - Add/remove questions in the form trigger
- AI Personality - Modify the system message in the AI agent node
- Email Templates - Adjust the Gmail node message format
- Database Structure - Change Google Sheets columns to match your needs

Contributing

Found a bug or have an idea? Feel free to:
- Open an issue
- Submit a pull request
- Share your improvements!

License

This project is licensed under the MIT License - feel free to use it for your projects!

Tips

- Test the workflow with sample data first
- Keep your API keys secure and never commit them
- Monitor the AI responses initially to ensure quality
- Adjust the system prompt to match your brand voice

Troubleshooting

Form not triggering?
- Check that the webhook is active
- Verify the form submission URL

AI not responding?
- Confirm your Gemini API key is valid
- Check API usage limits

Calendar booking fails?
- Ensure calendar permissions are granted
- Verify the calendar ID is correct
