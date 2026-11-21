# Practice Midterms

Four interactive practice exams for Midterm 2 of the MS1 Nervous System block (Weeks 4–5), hosted with GitHub Pages.

**Homepage:** https://chandingo.github.io/chandingo4prez/

| Exam | Items | Link |
|---|---|---|
| Midterm Mock #1 | 59 (50 session + 9 lab image) | [Open](https://chandingo.github.io/chandingo4prez/midterm2-mock-1/) |
| Midterm Mock #2 | 59 (50 session + 9 lab image) | [Open](https://chandingo.github.io/chandingo4prez/midterm2-mock-2/) |
| Midterm Mock #3 | 59 (50 session + 9 lab image) | [Open](https://chandingo.github.io/chandingo4prez/midterm2-mock-3/) |
| Midterm Mock #4 | 59 (weak-area retest) | [Open](https://chandingo.github.io/chandingo4prez/midterm2-mock-4/) |

## Features

- Untimed, with an elapsed clock you can hide
- Feedback mode: immediate (answer locks, key and explanation shown) or at the end
- Explanation for the correct answer plus why each wrong choice is wrong; annotated figures on image items
- Highlight stem text; cross out answer choices (right-click, or long-press on touch screens)
- Flags, item navigator, keyboard shortcuts (A–E, arrow keys, F)
- Results by section, week, session and faculty-style order; retakes keep earlier attempts

## How it works

Each exam is a single self-contained static page (`midterm2-mock-N/index.html`) with its questions embedded as JSON
and its figures in `images/`. There is no build step and no server code. Progress is stored in the browser's
`localStorage`, under a separate key per exam, so it stays on the device you used.

```
index.html                 homepage
midterm2-mock-1/           Midterm Mock #1 (index.html + images/)
midterm2-mock-2/           Midterm Mock #2
midterm2-mock-3/           Midterm Mock #3
midterm2-mock-4/           Midterm Mock #4
```

To run locally, serve the folder with any static server, for example `py -m http.server 8000`, then open
http://localhost:8000/.

## Notes

Questions and explanations are Claude-written for personal study. Figures come from course materials and textbooks
and remain the property of their owners. The pages carry `noindex` tags so search engines skip them.
