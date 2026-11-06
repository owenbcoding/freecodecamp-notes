# freeCodeCamp Study Notes

A personal, curriculum-aligned notebook for working through freeCodeCamp's current technical certifications. The notes and practice prompts here are original study material; use freeCodeCamp for the official lessons, tests, and certification requirements.

## Start here

1. Follow the [curriculum map](curriculum/README.md) to choose a certification.
2. Read the topic notes and attempt the practice prompts before checking their solutions.
3. Add a dated entry to [DAILY-LOG.md](DAILY-LOG.md) after each study session.
4. Commit and push a day's work when it is ready. This workspace has no GitHub remote configured yet.

## Current study set

- [Responsive Web Design v9](curriculum/responsive-web-design-v9/README.md): HTML, CSS, accessibility, and responsive layout notes; [HTML practice](curriculum/responsive-web-design-v9/html/practice.md) and [CSS practice](curriculum/responsive-web-design-v9/css/practice.md).
- [JavaScript v9](curriculum/javascript-v9/README.md): [JavaScript practice](curriculum/javascript-v9/practice.md).

Other current technical certification tracks are indexed in the [curriculum map](curriculum/README.md). Work through them in small, daily increments rather than treating this repository as a one-day course.

## Daily Git routine

```sh
git status
git add curriculum DAILY-LOG.md
git commit -m "Complete YYYY-MM-DD freeCodeCamp study"
git push
```

Set a remote once the GitHub repository exists:

```sh
git remote add origin https://github.com/USERNAME/REPOSITORY.git
git push -u origin HEAD
```

Never put a password or access token in the remote URL. Use GitHub's normal credential manager or SSH authentication.
