# Biology EOC Digital Study Guide

A self-scoring Georgia Milestones Biology EOC study guide for McIntosh County Schools. It has 72 questions, 3 for each of the 24 standard elements, organized by the five blueprint domains. Every domain a student submits is logged to a Google Sheet that shows each student's score on every element and who needs help.

## Links

- **Students:** https://arosenbaum993.github.io/biology-digital-study-guide/
- **Teachers:** https://arosenbaum993.github.io/biology-digital-study-guide/teacher.html

Both links work once GitHub Pages is on (Settings > Pages > Branch: `main`, folder `/ (root)`).

## Files

| File | What it is |
| --- | --- |
| `index.html` | The student study guide: sign-in, Key Ideas, questions, submit by domain, My Results |
| `teacher.html` | Teacher page: the student link to share, the score Sheet link, and how to read the Sheet |

## How scores reach the Sheet

`index.html` posts each domain submission to a Google Apps Script web app (`SHEETS_URL` near the bottom of the file). The script lives in the score Sheet, not in this repo. It writes the submission to the **Responses** tab and rebuilds **Gradebook**, **Needs Help**, and **Element Summary**.

- To point the guide at a different Sheet, replace `SHEETS_URL` in `index.html`.
- To show the score Sheet button on the teacher page, paste the Sheet's URL into `SHEET_URL` near the bottom of `teacher.html`.

The answer key in `index.html` is obscured, not encrypted. Treat this as a study guide, not a secure assessment.
