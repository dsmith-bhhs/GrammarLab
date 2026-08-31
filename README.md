# Grammar Lab

A self-contained web app for Grade 9 Edit Notes: one grammar and punctuation lesson per month, September through June.

Each lesson has three phases:

1. **Learn** — the rule, worked examples, and a reteach explanation
2. **Practice** — handout sentences with instant feedback
3. **Practice quiz** — 10 shuffled questions, 90% to earn mastery

Students who fall short of 90% get reteach content, a review of every missed question, and a freshly shuffled retake. Progress (best score, attempts, mastery) is saved in the browser on the student's own device — no accounts, no server, no data leaves the machine.

At the end of a quiz, students pick their teacher from a dropdown (Smith / Marinaro, Salvato, or Vernola) and press **Email my results to my teacher**, which opens a pre-filled Gmail draft with their name, lesson, score, and every missed question.

## Files

- `index.html` — the entire app in one file. No build step, no dependencies, no internet connection required.

## Posting it for students

**GitHub Pages (recommended):** push this repo, then Settings → Pages → Source: `main` branch, `/ (root)`. Students open the published URL — share it in Google Classroom.

**Or as a file:** students download `index.html` and double-click it. It runs offline.

## Schedule

All ten lessons are open at all times, so teachers can assign them in any order and on any timeline. The months are labels for the intended 2026–2027 sequence, not locks.

## Changing settings

Open `index.html` in a text editor and search for:

- `teachers()` — the teacher names and email addresses in the dropdown
- `passThreshold` — the score needed to earn mastery (default 90%)
- `quizLength` — questions per quiz (default 10)
