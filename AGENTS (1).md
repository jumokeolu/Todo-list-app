# AGENTS.md

Instructions for AI coding agents working on this project.

## Project overview

A small to-do list web app built for an internship assignment. Users can add tasks, mark them done, delete them, filter by All / Active / Done, and clear completed tasks. Tasks are saved in the browser with `localStorage`.

## Structure

```
.
├── index.html   # The whole app: HTML, CSS and JavaScript in one file
└── AGENTS.md    # This file
```

There is no build step, no framework and no backend. Keep it that way unless the task says otherwise.

## Run and deploy

- Run locally: open `index.html` in a browser.
- Deploy: connect this repository to a static host (Netlify, Vercel or similar). Publish the repository root. No build command is needed.

## Conventions

- Keep everything in `index.html` unless the file grows too large to read comfortably. If it is split, use `style.css` and `app.js` next to it.
- Use plain JavaScript. Do not add dependencies without a clear reason.
- Colours are CSS variables defined on `:root`, with a dark-mode set. Change colours there, not inline.
- Wrap every `localStorage` read and write in `try/catch`. The app must still work if storage is unavailable.
- Keep the UI usable on a phone screen and keyboard accessible: labelled controls, visible focus, sentence-case text.
- Button text says what it does ("Add task", "Clear completed").

## Working process

1. Read this file and `index.html` before making changes.
2. Make one small change at a time and describe what changed.
3. After each change, check: add a task, complete it, filter, delete, reload the page and confirm tasks persist.
4. Commit with a short, plain message such as "Add task filter".
5. Do not commit secrets or API keys. This app needs none.

## Ideas for later

- Edit an existing task.
- Due dates.
- Drag to reorder.

## AI use

The first version was written with Claude from a plain-language description of the app. Later changes should follow the process above.
