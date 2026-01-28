# n8n Instagram AI Content Generator

An automated AI-powered Instagram content generator built using n8n, Google Gemini, and HTTP APIs.
This workflow takes user input, generates Instagram captions + image prompts using AI, calls an image generation API, and finally sends the output via email.

## ✨ Features

📝 User input via Form Trigger

🤖 Instagram caption & content generation using Google Gemini

🎨 AI-powered image prompt generation

🌐 Image generation using HTTP Request API

📧 Automatically sends generated content & image link via Email

🔁 Fully automated end-to-end workflow

## 🧠 Workflow Overview
Form Submission
      ↓
Instagram Content Generator (Gemini)
      ↓
Image Prompt Generator (Gemini)
      ↓
HTTP Request (Image API)
      ↓
Send Email (Final Output)

## 🛠 Tech Stack

n8n – Workflow automation

Google Gemini API – Text & prompt generation

HTTP Request Node – Image generation API call

Email Node – Send final results

JavaScript Expressions – Data mapping inside n8n

## ⚙️ Prerequisites

Before using this workflow, make sure you have:

n8n (Cloud or Self-hosted)

Google Gemini API Key

Image Generation API (any provider)

Email credentials configured in n8n


GEMINI_API_KEY=your_gemini_api_key
IMAGE_API_KEY=your_image_api_key


⚠️ Never commit real API keys to GitHub.

## 🚀 Setup Instructions
1️⃣ Clone the Repository
git clone https://github.com/your-username/n8n-instagram-ai-agent.git
cd n8n-instagram-ai-agent

2️⃣ Import Workflow into n8n

Open n8n

Click Import workflow

Upload instagram-content-image-email.json

Save the workflow

3️⃣ Configure Credentials

Add Google Gemini credentials

Configure HTTP Request API Key

Set up Email (SMTP / Gmail) credentials

4️⃣ Update HTTP Request Node

Method: POST

Headers:

{
  "Authorization": "Bearer YOUR_API_KEY",
  "Content-Type": "application/json"
}


Body: Uses image prompt generated from Gemini

5️⃣ Execute the Workflow

Open the workflow

Click Execute workflow

Submit the form

Receive Instagram content + image link via email 🎉

📧 Email Output Includes

Instagram caption

Hashtags

Image description

Image URL or attachment (based on API)

## 🧪 Example Use Cases

Social media managers

Content creators

Marketing agencies

AI automation demos

Portfolio projects

## 🧩 Customization Ideas

Schedule posts automatically

Post directly to Instagram

Add multiple image styles

Support multiple languages

Save outputs to Google Sheets / Notion

## 🐞 Common Issues
❌ 403 / API Key Error

Check if API key is active

Ensure headers are correctly set

❌ Email sent without attachment

Ensure image URL exists

Use binary data for attachments

## 📌 Future Improvements

Instagram auto-posting

Multi-platform support (LinkedIn, Twitter)

Image storage (S3, Cloudinary)

User authentication

## 🤝 Contributing

Pull requests are welcome.
For major changes, please open an issue first.


## 👤 Author

Built by Neha Geete

AI • Automation • n8n 
