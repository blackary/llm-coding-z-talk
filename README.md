---
marp: true
title: LLM Coding Z Talk
paginate: true
theme: default
class: lead
footer: LLM Coding Z Talk, 2025-08-13
---

# LLM Coding Z Talk

Using LLMs to help when building software.

---

## What we'll cover

- The Tooling Landscape Today
- LLM Workflows
- Where are AI Coding Tools Most Useful?
- Obvious Risks and Pitfalls
- Tips and Tricks
- Demo
- Q&A

---

## The Tooling Landscape Today

- Dedicated coding tools:
    - Cursor
    - Claude code
    - (Aider, etc.)


---

## The Tooling Landscape Today

- Agents (can check https://prarena.ai/ for one measure of performance):
    - Codex
    - Github Copilot
    - Cursor Agents

---

## The Tooling Landscape Today

- Standalone Chat tools:
    - ChatGPT
    - Perplexity
    - etc.

---

## The Tooling Landscape Today

- Today's Top Models (can check https://www.swebench.com/ for one measure of performance):
    - GPT-5
    - Claude 4
    - Gemini 2.5

---

## Where are AI Coding Tools Most Useful?

* Repetitive transformations (refactoring, etc.)
* Researching and applying code examples
* Updates with feedback
    - e.g. "Fix then run the tests", "Fix then query the table", etc.
* Popular packages
* Typed code (static typed languages, python + type hints)
* Understanding existing codebases
* Contexts where you (or the reviewer) are able to judge quality and architectural decisions

---

## Obvious Risks and Pitfalls

* Looks good, must be right?
* No need to learn new tools, just outsource them
* Is this a good pattern?
* "Code's compiling" (https://m.xkcd.com/303/)
* Inefficiencies
    - Code way too complex/long
    - Code could be much more efficient

---

## LLM Workflows

-

---

## Tips and Tricks

* Let the models fight
    -  "My coworker wrote this, but I don't think it's right"
* You're the PM
* Ask it to make a plan for the approach it will take, and review it
* Learn to use the tool's pre-instructions (e.g. .cursor/rules, CLAUDE.md)
* Give it the right context--point to files, docs urls, etc.

---

## Tips and Tricks

* Set up good rules in your repo (e.g. linting and testing with pre-commit hooks)
* Empower it to check the work (e.g. "use npx <tool> to run a SQL query", "use use uvx pytest to run all the tests")
* https://www.anthropic.com/engineering/claude-code-best-practices -- generally helpful

---

## Demo


---

## Q&A

Questions, comments, ideas?
