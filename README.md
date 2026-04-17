# RepoScope

RepoScope is a tool that analyzes GitHub repositories and gives quick insights into code quality, technical debt, and possible improvements.

It was built during a hackathon with the goal of making code reviews faster and more accessible.

---

## What it does

* Gives a tech debt score for a repository
* Highlights critical issues in the codebase
* Suggests improvements and refactoring ideas
* Points out strengths in the project
* Shows basic repository stats (stars, forks, contributors, etc.)
* Visualizes language distribution
* Allows comparison between two repositories

---

## Tech stack

* Frontend: React
* Backend: Flask
* APIs: GitHub API, Groq API
* Model: LLaMA 3.3 (via Groq)

---

## How it works

1. Enter a GitHub repository name
2. The backend fetches repository data using GitHub API
3. The code is processed and sent to an AI model
4. The results are structured and shown in the dashboard

---

## Running locally

### Backend

```
pip install -r requirements.txt
python app.py
```

### Frontend

```
npm install
npm start
```

---

## Environment variables

Create a `.env` file in the root:

```
GITHUB_TOKEN=your_token_here
GROQ_API_KEY=your_key_here
```

---

## Note

This project focuses on giving quick, useful insights rather than perfect analysis. The results are meant to guide developers, not replace manual code reviews.

---

## About

Built as part of a hackathon project. Main focus was on speed, usability, and making the output easy to understand.
