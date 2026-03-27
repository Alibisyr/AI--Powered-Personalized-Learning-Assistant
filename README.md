# AI-Powered Personalized Learning Assistant (Telegram + n8n)

A Telegram-based assistant that personalizes learning for each student using the school annual curriculum (KTP / Күнтізбелік-тақырыптық жоспар).  
Instead of giving the same tasks to everyone, it adapts assignments to the student’s current level, learning style, and progress — and keeps motivation high with a points system.

---

## The Problem

**One curriculum does not fit all.** In real classrooms:

1. **A single standardized curriculum** is used for all students, but students learn at different speeds.
2. **Students with different knowledge levels** often receive the same assignments → frustration for some and boredom for others.
3. **Teachers don’t have time** to manually create personalized tasks for every student.
4. **Motivation drops** and progress is hard to measure without personalized feedback and challenges.

---

## What This Assistant Does

The assistant supports true personalization by working directly from the **KTP (annual curriculum)**:

- Reads the annual curriculum (KTP)
- Evaluates the student’s knowledge (quick diagnostic test)
- Identifies learning style (visual vs text-based)
- Generates personalized assignments
- Increases difficulty automatically as the student improves
- Rewards students with points (gamification)

---

## How It Works (Flow)

1. **Teacher uploads the KTP**
2. **Student takes a quick diagnostic test**
3. The system **determines the student’s level**
4. **Personalized tasks are generated**
5. **Difficulty adapts automatically** over time
6. Student interacts via **Telegram interface + point system**

---

## Key Features

- Full personalization based on the **KTP**
- Learning-style adaptation (**visual / text-based**)
- Real-time **adaptive difficulty**
- Gamification through **points and leaderboards**
- Works directly inside **Telegram**
- Easy to add **new subjects**
- Suitable for **schools, colleges, and EdTech**
- Scalable at **regional and nationwide** level
- Integration-ready for educational systems

---

## Expected Impact

- Higher academic performance
- Faster gap-closing (helps students catch up)
- Saves teachers’ time
- Improves motivation and engagement
- Creates a personalized study path for every student

---

## Demo / Screenshots

Examples:
- KTP upload / parsing
- Student profile table (level, score, points)
- Telegram chat with generated tasks

---

## Tech Stack

- **n8n** (automation + orchestration)
- **Telegram Bot** interface
- Optional integrations (depending on your setup):
  - Google Sheets / Airtable / database for student profiles
  - HTTP API calls to LLMs or content services
  - Webhooks for teacher uploads and events


## Getting Started

### 1) Requirements
- n8n (self-hosted or cloud)
- Telegram bot token (via BotFather)
- Storage for student data (Google Sheets / DB / Airtable — depending on your workflow)

### 2) Setup (high level)
1. Import workflows from `/workflows` into n8n
2. Add environment variables / credentials:
   - Telegram Bot token
   - Database / Sheets credentials
   - Any API keys used in the workflow
3. Run n8n and start the Telegram bot
4. Upload a KTP and test the student diagnostic flow



---

## Roadmap (ideas)

- Better KTP parsing (tables, PDFs, scanned documents)
- Teacher dashboard (progress, weak topics, class statistics)
- More learning styles and task formats
- Stronger evaluation & tracking (mastery model)
- Safer content filters + plagiarism/cheating protection

