# AWS SAA-C03 Study Hub

A single-page study app for the AWS Solutions Architect Associate (SAA-C03) exam. No build step required — open `index.html` in a browser and go.

## Features

- **Quiz** — 65+ multiple-choice questions across all four SAA-C03 domains (Secure, Resilient, High-Performing, Cost-Optimized), plus official AWS practice questions
- **Practice Exam** — timed, full-length mock exams with per-domain scoring
- **Flashcards** — concept cards and vocab cards with a confidence-based filter (New / Nope / Sorta / Know)
- **Daily Lessons** — structured lessons covering core services (SES, Hybrid & Edge, and more)
- **Architect's Mindset** — scenario-based decision-making exercises and core design principles
- **Glossary** — filterable vocab by service category
- **Analytics** — quiz and exam history with domain-level breakdown
- **Notes** — freeform study notes saved to localStorage
- **Readiness Score** — rolling estimate of exam readiness based on quiz history

## Getting Started

```bash
# Install dependencies (generates assets/tailwind.css)
npm install
npm run build   # or: npx @tailwindcss/cli -i input.css -o assets/tailwind.css

# Then open in a browser
open index.html
```

All progress is saved to `localStorage` — no server or login needed.

## Project Structure

```
index.html          # Entire app (React via Babel standalone, ~3 400 lines)
input.css           # Tailwind source
assets/
  tailwind.css      # Built CSS
  react.js          # React 18 (local copy)
  react-dom.js      # ReactDOM 18 (local copy)
  babel.min.js      # Babel standalone for JSX in-browser
```

## Domain Weights (SAA-C03)

| Domain | Weight |
|---|---|
| Design Secure Architectures | 30% |
| Design Resilient Architectures | 26% |
| Design High-Performing Architectures | 24% |
| Design Cost-Optimized Architectures | 20% |
