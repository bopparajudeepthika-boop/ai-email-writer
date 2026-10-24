# ✉️ AI Email Writer

### Write Better Emails in Seconds with AI

AI Email Writer is an AI-powered web application that helps users create clear, professional, and personalized emails in seconds. Users can enter their email requirements, choose a tone and length, and generate an email draft using Google's Gemini AI.

## 🚀 Features

- **AI-Powered Email Generation:** Generate email drafts using Gemini AI.
- **Multiple Email Categories:** Create internship applications, job applications, leave requests, follow-ups, meeting requests, thank-you emails, and more.
- **Custom Email Tones:** Choose professional, formal, friendly, persuasive, polite, confident, apologetic, or casual tones.
- **Adjustable Email Length:** Generate short, medium, or detailed emails.
- **Editable Email Drafts:** Modify generated content before using it.
- **Copy to Clipboard:** Copy your email with a single click.
- **Regenerate Emails:** Generate a new version using the same requirements.
- **Responsive Design:** Access the application on desktop, tablet, and mobile devices.
- **Secure API Integration:** Keep the Gemini API key on the backend rather than exposing it in frontend code.
- **User-Friendly Interface:** Simple and clean design for an easy writing experience.

## 🛠️ Technologies Used

**Frontend**
- React
- Vite
- JavaScript
- HTML5
- CSS3

**Backend**
- Node.js
- Express.js

**Artificial Intelligence**
- Google Gemini API
- Google Gen AI JavaScript SDK

**Development and Version Control**
- Replit
- npm
- Git
- GitHub

## ⚙️ How It Works

1. Open the AI Email Writer website.
2. Select the email category.
3. Enter the subject and details of the email.
4. Choose your preferred tone and length.
5. Click **Generate Email**.
6. Gemini AI processes the request and generates an email draft.
7. Edit the draft, copy it, or generate another version.

## 📂 Project Structure

The project is organized into frontend and backend components. The exact structure may vary depending on the implementation.

```text
ai-email-writer/
├── client/
│   ├── src/
│   │   ├── App.jsx
│   │   ├── App.css
│   │   ├── index.css
│   │   └── main.jsx
│   └── package.json
├── server/
│   ├── server.js
│   └── package.json
├── .env.example
├── .gitignore
├── package.json
└── README.md
```

## 🔑 Gemini API Configuration

The application requires a valid Gemini API key to generate emails.

1. Visit [Google AI Studio](https://aistudio.google.com/apikey).
2. Obtain an API key if API access is available to your account.
3. Open your project in Replit.
4. Open the Secrets or environment variables section.
5. Add the following secret:

```text
GEMINI_API_KEY=your_actual_api_key
```

6. If the application uses a configurable model, set `GEMINI_MODEL` to a currently supported Gemini text-generation model.
7. Restart the application if required.

**Security:** Never publish your real API key in GitHub, frontend code, screenshots, or public messages. Use environment variables for sensitive configuration.

## ▶️ Running the Project

The following commands apply if the project has the corresponding root-level npm scripts configured.

Install dependencies:

```bash
npm install
```

Start the development application:

```bash
npm run dev
```

Create a production build:

```bash
npm run build
```

Start the production server:

```bash
npm start
```

If the frontend and backend use separate package files, follow the commands configured in those directories and the actual project scripts.

## 🔌 Backend API

### Health Check

```http
GET /api/health
```

Checks whether the backend server is running.

### Generate Email

```http
POST /api/generate-email
Content-Type: application/json
```

Example request:

```json
{
  "recipient": "Hiring Manager",
  "category": "Internship Application",
  "subject": "Application for a Software Development Internship",
  "details": "I am a computer science student interested in applying for an internship.",
  "tone": "Professional",
  "length": "Medium",
  "includeSubject": true,
  "includeGreeting": true
}
```

Example successful response:

```json
{
  "success": true,
  "email": "Dear Hiring Manager,\n\nI am writing to express my interest..."
}
```

The response format may vary slightly depending on the implemented backend.

## 🛡️ Security and Privacy

- API keys should be stored in server-side environment variables.
- Secrets must not be committed to GitHub.
- The backend should validate incoming requests.
- Error messages should not reveal private credentials or internal server details.
- Generated emails should be reviewed by users before sending.
- The application generates email drafts; it does not automatically send emails.

## 🐛 Troubleshooting

**Email generation is not working**
- Verify that `GEMINI_API_KEY` is configured in Replit Secrets.
- Check whether the API key is valid.
- Review API quota, billing requirements, model availability, and network errors.
- Inspect the server logs for the actual error.

**The website is not opening**
- Check whether the frontend and backend processes started successfully.
- Verify the npm scripts and dependency installation.
- Review the Replit console for errors.

**API requests return 404**
- Verify the backend route and frontend API URL.
- Check the Vite proxy configuration in development.

**The application returns a configuration error**
- Configure the required environment variables and restart the application if necessary.

## 🌱 Future Improvements

- Email templates for different professions and situations.
- Support for multiple languages.
- AI-powered grammar correction and email rewriting.
- Save favorite email drafts.
- Download emails as text files.
- User accounts and cloud-based draft storage.
- Gmail integration with explicit user authorization.
- Additional writing assistance features.

These are potential future enhancements and may not be included in the current version.

## 📌 Project Goal

The goal of AI Email Writer is to make professional communication easier, faster, and more accessible by using generative AI to help users write effective emails.

## 👩‍💻 Author

**Deepthika Bopparaju**

Student Developer | AI and Full-Stack Development Enthusiast

## 📄 License

This project is intended for educational and portfolio purposes. Add an open-source license, such as the MIT License, if you wish to distribute the project under those terms.
