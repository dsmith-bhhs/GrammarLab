# Grammar Lab

A self-contained web app for Grade 9 Edit Notes: one grammar and punctuation lesson per month, September through June.

Each lesson has three phases:

1. **Learn** — the rule, worked examples, and a reteach explanation
2. **Practice** — handout sentences with instant feedback
3. **Practice quiz** — 10 shuffled questions, 70% to pass

Students who fall short of 70% get reteach content, a review of every missed question, and a freshly shuffled retake. Progress (best score, attempts, mastery) is saved in the browser on the student's own device — no accounts, no server, no data leaves the machine.

At the end of a quiz, students can press **Email my results to my teacher**, which opens a pre-filled Gmail draft (name, lesson, score, and every missed question) addressed to dsmith@byramhills.net and jmarinaro@byramhills.net.

## Files

- `index.html` — the entire app in one file. No build step, no dependencies, no internet connection required.

## Posting it for students

**GitHub Pages (recommended):** push this repo, then Settings → Pages → Source: `main` branch, `/ (root)`. Students open the published URL — share it in Google Classroom.

**Or as a file:** students download `index.html` and double-click it. It runs offline.

## Schedule

Lessons unlock on the 1st of their month during the 2026–2027 school year (Lesson 1 in September 2026 through Lesson 10 in June 2027). Once a month has passed, its lesson stays open for the rest of the year.

## Changing the schedule or settings

Open `index.html` in a text editor and search for:

- `const startYear = 2026` — the school year the lessons are pinned to
- `dsmith@byramhills.net` — the teacher email recipients
- `passThreshold` / `quizLength` — pass percentage and questions per quiz
- `unlockAll` — set the default to `true` to open every lesson regardless of date
