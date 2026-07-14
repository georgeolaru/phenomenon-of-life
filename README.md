# The Phenomenon of Life — an interactive game

A single-file, self-contained learning game inspired by Christopher Alexander's
**The Nature of Order, Book One: The Phenomenon of Life**.

Build the **fifteen fundamental properties of living structure** into a Persian
carpet, tune each property with granular controls, and train your eye against a
real *degree-of-life* model — one where complexity is **not** the same as life.

## Files
- `phenomenon-of-life.html` — the current game (the one that's published).
- `pattern-weaver.html` — the earlier prototype based on *A Pattern Language*
  (Towns 1–94), kept for reference.

Both are single self-contained HTML files: no build step, no dependencies.

## Run it locally
Just open the file in a browser:
```
open phenomenon-of-life.html
```

## Live public site (GitHub Pages)
**https://georgeolaru.github.io/phenomenon-of-life/** — open with no login, on any device.

Served from `index.html` on the `master` branch (repo is public). `index.html`
is `phenomenon-of-life.html` with a `<!doctype html>` line prepended (standards
mode). **When you change the game, regenerate it:**
```
printf '<!doctype html>\n' | cat - phenomenon-of-life.html > index.html
git add -A && git commit -m "update" && git push
```
Pages rebuilds in ~1 minute.

## Published artifact (private link)
Also at: https://claude.ai/code/artifact/0fee8dcb-bc01-4e4c-933e-ca23c568f313
Private to the owner's Claude account until shared from the page's share menu.
Keep `phenomenon-of-life.html` free of `<!doctype>`/`<html>`/`<head>`/`<body>`
tags — the artifact host adds them at publish time. Browse yours at
https://claude.ai/code/artifacts

## How to continue in a future Claude Code session
1. Open a Claude Code session in this folder.
2. Say e.g. *"continue working on phenomenon-of-life.html"*.
3. After changes, ask Claude to **republish to the same artifact URL above**
   (pass that URL to the Artifact tool) so the link and version history are kept.

## Ideas / backlog
- "Why is this crowded?" live hint in Compose mode — name which property to
  remove, or which calm/void to add, to restore balance.
- The Nature of Order Book 2 (The Process of Creating Life) as a third mode.
- A second worked example beyond the carpet (a building facade, a wave).
- A short quiz: name the property from its visual.
