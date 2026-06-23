# SLATE

> **The notes app that does one thing.** No databases, no templates, no toggles, no AI. You write, you find it later, that's it.

---

## Status

- Phase 1 Exploration: draft 2026-06-23
- Phase 2 Execution: not started
- Phase 3 Validation: not started

Last updated: 2026-06-23

---

## 1. Overview

**Problem**

You opened Notion to write down a thought, and 45 minutes later you were watching a YouTube tutorial on how to build a "second brain." You have a graveyard of half-built workspaces: a Notion dashboard with broken databases, an Obsidian vault with 200 untagged files, an Apple Notes folder you have not opened in a year. The tools promise productivity and deliver decision fatigue. Every time you go to write a note, you are first asked to design the system that holds it. The note itself, the actual thought, never gets written. You wanted a place to think and you got a software project.

**Target users**

Primary: 25-45 year olds who have churned out of Notion, Obsidian, or Roam because the tool became the work. They take notes for themselves, not for a team, and just want to capture and find ideas without building infrastructure.

Not for: power users who genuinely love building databases and templates, teams collaborating on shared docs, or anyone who needs structured data (tables, relations, formulas). Slate is for solo writing only.

---

## 2. Product experience

Slate has no homepage. You open it and the cursor is already in a new note. You start typing. There is no title field, no template picker, no folder to choose. The first line becomes the title, automatically, the rest is the body. Markdown works but is not required. Pressing escape saves and gets out of your way. That is the entire write flow.

To find a note, you swipe down to search. Search is fast, full-text, and the only retrieval mechanism, no tags, no folders, no graph view, no backlinks. If you cannot find a note by typing two words from it, the note was probably not important. The list shows the most recent notes by default, and you can pin up to 5 if you want quick access to a current project.

There are no databases. There are no toggles. There are no templates. There is no AI button. There are no integrations. There is no mobile-vs-desktop sync drama because the app is a small native client backed by a single text file per note in iCloud or a folder you point at. Your notes are .md files on disk. If Slate disappears tomorrow, you open them in any text editor.

Slate is paid once, owned forever, like a piece of software used to be. There is no subscription because there is no server. We do not need to keep extracting value from you, the app is finished.

In short: a notes app that lets you write a note in 2 seconds and find it again in 5, and refuses to be anything more.

---

## 3. Hypotheses and success metrics

| #   | Hypothesis                                                                                                          | Metric                                                                                  | Target |
| --- | ------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | ------ |
| H1  | The audience of "Notion refugees" is large and willing to pay upfront for a deliberately minimal alternative.        | # of paying users in first 90 days at $20-40 upfront.                                    | TBD    |
| H2  | Users who switch from Notion to Slate write more notes per week, because the friction to start is near zero.         | Median notes/week, compared to self-reported Notion usage of same user pre-switch.       | TBD    |
| H3  | The app is sticky despite having no engagement hooks: people use it because it does its job, not because it pulls.   | % of paying users still active at day 90 and day 180.                                    | TBD    |

---
