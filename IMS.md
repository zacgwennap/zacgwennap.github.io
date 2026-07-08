---
layout: default
title: IMS — Personal Information System
parent: Projects
nav_order: 3
---

# IMS — Personal Information System

IMS is a self-hosted system I built to manage my personal information — tasks, calendar events, notes, and project documentation — and to let AI agents read and write that information directly. Everything runs on my own hardware.

---

## Use Case

I use it daily for task tracking, quick capture, and project work. From my phone or desktop I can type or dictate a task, an event, or something to remember, and the system files it in the right place without me formatting anything. When I start an AI work session on a project, the session already has the relevant history: what was done last time, what was decided, and what's still open.

---

## How Information Is Captured

Captured text or dictation is passed to an AI triage step that classifies each item as a task, calendar event, or note and attaches metadata such as tags and due dates. Tasks go to a database behind a self-hosted web app, events go to the calendar, and notes are saved as Markdown files. Notes containing links are enriched automatically with fetched page context, keywords, and a short summary.

AI work sessions also write information: each session ends with a dated log covering the work done, the decisions made and their reasoning, and open items. Significant choices are appended to a running decision log.

---

## How Information Is Stored and Retrieved

All records are plain Markdown files in a git repository. A vector index (ChromaDB, locally computed embeddings) is built over the repository and kept current by a file watcher; agents query it through an MCP server for semantic search. Sessions open by searching current state and reading the task list and the latest session log, then continue from there.
