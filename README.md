# EduGenie — Google Gemini Powered Learning Assistant

EduGenie is a student-friendly learning assistant powered by Google's Gemini API.

## Features

- AI Tutor chat for explanations and follow-up questions
- Explain a topic at beginner, intermediate, or advanced level
- Generate practice quizzes
- Summarize notes
- Generate a personalized study plan
- Quick example prompts
- Responsive dashboard UI
- Server-side Gemini API integration so the API key is not exposed to the browser
- Friendly error handling and loading states

## Requirements

- Node.js 20+
- A Gemini API key from Google AI Studio

Google's current JavaScript SDK is `@google/genai`. The app uses Gemini's Interactions API.

## Setup

1. Extract the ZIP.
2. Open a terminal in the `EduGenie` folder.
3. Install dependencies:

```bash
npm install
```

4. Copy `.env.example` to `.env`:

```bash
cp .env.example .env
```

On Windows, simply duplicate `.env.example` and rename it to `.env`.

5. Put your Gemini API key in `.env`:

```env
GEMINI_API_KEY=YOUR_KEY_HERE
```

6. Start the app:

```bash
npm start
```

7. Open:

http://localhost:3000

## Development

```bash
npm run dev
```

## Project structure

```text
EduGenie/
├── public/
│   ├── index.html
│   ├── styles.css
│   └── app.js
├── .env.example
├── .gitignore
├── package.json
├── README.md
└── server.js
```

## Notes

- The browser calls only the local EduGenie server.
- The Gemini API key stays in the server environment.
- Do not upload your real `.env` file to GitHub.
- AI-generated answers should be checked against your textbook, teacher, or trusted sources for schoolwork.

## Customization

You can change the Gemini model in `server.js` through the `GEMINI_MODEL` constant.

The default model in this project is `gemini-3.8-flash`.
