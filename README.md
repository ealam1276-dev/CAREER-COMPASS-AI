CareerCompass AI 🧭 - Your Personal AI Career Coach
Welcome to the official repository for CareerCompass AI! This is a complete, AI-powered toolkit designed to guide students from career confusion to clarity, built entirely with HTML, Tailwind CSS, JavaScript, and the Google Gemini API.

(Note: You can take a screenshot of your app and upload it to a site like Imgur to get a link for this image.)

🚀 Live Demo
You can view and interact with the fully deployed version of the project here:

https://your-netlify-link.netlify.app 👈 (Replace this with your actual Netlify link after deploying)

✨ Features
CareerCompass AI is more than just a single tool; it's a complete ecosystem to help students prepare for their professional journey.

🤖 AI Career Assessment: A conversational quiz that analyzes your personality and interests to recommend the top 3 career paths for you.

🗺️ Detailed Roadmap Generator: Get a step-by-step learning plan from beginner to advanced for any career role you can imagine.

📄 Resume Builder & ATS Scorer: Input your details in simple points, and the AI will generate a professional, ATS-friendly resume draft and provide an estimated score.

🎙️ AI Mock Interview: Practice for real interviews with a voice-based AI interviewer (Shreya!) who asks questions and provides instant feedback.

💼 Live Job Listings: Find simulated real-time job openings from platforms like LinkedIn based on your target role and skills.

💖 Daily Motivation: A unique check-in feature where you can share how your day was and receive a personal, encouraging message and a motivation score from the AI.

🏆 Progress Tracker & Badges: Save your generated roadmaps and track your learning progress with an interactive checklist. Unlock badges as you complete milestones!

🌐 Multi-Language Support: Fully functional in both English and Hindi.

🗣️ Community Hub (AI Mentor): Ask any career-related question and get a detailed, supportive answer from an AI acting as an experienced mentor.

🛠️ How to Run This Project Locally
The live demo works out-of-the-box. However, if you want to clone this repository and run the project on your own computer, you will need to add your own secret Google Gemini API key. The key has been intentionally removed from the public code for security.


*****if you can avoid this all step to go index.html file and go line no 873 paste your api  this place(netlify/function/gemini) and go live it work perfectly**


Step 1: Initial Setup
Clone the Repository:
First, get the project files on your computer. Open your terminal and run:

git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name

(Replace your-username/your-repo-name with your actual GitHub repository path)

Get Your API Key:
This project runs on the Google Gemini API. You can get your own free API key here:

Visit Google AI Studio.

Click on "Create API key" and copy the key. Keep it safe like a password.

Step 2: Install Netlify CLI
This project uses Netlify Serverless Functions to protect your secret API key. The Netlify Command Line Interface (CLI) will help you run this special setup on your local machine.

In your terminal, run this command to install the Netlify CLI globally:

npm install -g netlify-cli

Step 3: Configure Your Secret Key
Now, we'll link your project to Netlify and securely tell it your secret API key.

Log in to Netlify:
Connect the CLI to your Netlify account. This will open your browser for you to log in.

netlify login

Initialize the Project:
This is the most important step. Run this command from inside your project folder:

netlify init

Follow the on-screen steps. It will ask you to connect to a new or existing site. Choose to create a new site.

When it asks for your Build command and Deploy directory, you can just press Enter to leave them blank.

Set the Secret Key:
Now, tell Netlify your secret API key without writing it in the code. Run this command:

netlify env:set GEMINI_API_KEY

It will ask you for the value. Paste your new Google Gemini API key here and press Enter.

Step 4: Run the Project!
You're all set! Start the local development server by running:

netlify dev

This command will start a local server (usually at http://localhost:8888) that knows how to use your secret API key securely. Open this URL in your browser, and the application will be fully functional!
