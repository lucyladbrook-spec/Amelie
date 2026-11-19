# Amelie's Physics Club

A personal GCSE Physics revision site (AQA 8463, Higher), built as a calm, accessible study journal.

## What's inside

| File | What it holds |
|---|---|
| `index.html` | The whole site: design, layout and code (no build step, no frameworks) |
| `data.json` | The 42-session plan, weeks, exam tips, past papers, resources, study habits |
| `content.json` | Revision content for every session: key ideas, key words, worked examples, practice questions and answers, exam warnings |
| `enrich.json` | Session objectives, hints, number answers, worked solutions, exam-watch pairs, equation cards, question decoder |

## Running it

The site loads its `.json` files with `fetch`, so it needs to be served over the web rather than opened as a local file.

- **GitHub Pages:** Settings → Pages → Source: *Deploy from a branch* → `main` / root. The site appears at `https://<your-username>.github.io/<repo-name>/`.
- **On your computer:** in this folder run `python3 -m http.server`, then open http://localhost:8000.

## Progress

Progress, confidence ratings, charms, rewards and past paper scores are saved in the browser (localStorage), so each device keeps its own copy. On claude.ai the same page can also sync progress between devices; that part switches itself off anywhere else.

## Editing content

All revision content lives in the three `.json` files, separate from the design. Questions in `content.json` line up one-to-one with the hints and answers in `enrich.json` (same session number, same order).
