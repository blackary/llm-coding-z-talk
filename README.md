---
marp: true
title: LLM Coding Z Talk
paginate: true
size: 16:9
theme: gaia
footer: LLM Coding Z Talk, 2025-08-13
style: |
  section {
    font-size: 34px;
    line-height: 1.35;
  }
  h1, h2, h3 {
    color: #0f172a;
    letter-spacing: -0.01em;
  }
  h1 {
    font-size: 72px;
    margin-bottom: 0.2em;
  }
  h2 {
    font-size: 46px;
    margin-bottom: 0.4em;
    border-bottom: 2px solid #e2e8f0;
    padding-bottom: 0.2em;
  }
  a {
    color: #0369a1;
    text-decoration-thickness: 2px;
    text-underline-offset: 3px;
  }
  ul {
    margin-top: 0.4em;
  }
  li {
    margin: 0.25em 0;
  }
  section.lead h1 {
    font-size: 88px;
    color: #ffffff;
  }
  section.lead p, section.lead a {
    font-size: 30px;
    color: #e2e8f0;
  }
  section.lead {
    background: radial-gradient(1200px 600px at 20% 20%, #0ea5e9 0%, transparent 60%),
                radial-gradient(1000px 500px at 80% 10%, #22d3ee 0%, transparent 55%),
                linear-gradient(160deg, #0b1020 0%, #111827 60%, #0b1020 100%);
    color: #e2e8f0;
  }
  section.lead footer {
    display: none;
  }
  section:not(.lead) {
    background: #ffffff;
    color: #0f172a;
  }
  footer {
    color: #64748b;
    font-size: 18px;
  }
  .marp-pagination {
    color: #64748b;
    font-weight: 600;
  }
---

<!-- _class: lead -->
<!-- _paginate: skip -->

# LLM Coding Z Talk

Using LLMs to help when building software.

[blackary.com/llm-coding-z-talk](https://blackary.com/llm-coding-z-talk)

---

## What we'll cover

- The Tooling Landscape Today
- Where are AI Coding Tools Most Useful?
- Obvious Risks and Pitfalls
- LLM Workflows I use most
- Tips and Tricks
- Demo
- Q&A

---

## Caveats

- This is largely based on personal reading and experience, more than deep understanding of LLMs
- This is already out of date

---

## The Tooling Landscape Today

Dedicated coding tools:
    - Cursor
    - Claude code
    - (Aider, etc.)

---

## The Tooling Landscape Today

Agents
    - Codex
    - Github Copilot
    - Cursor Agents

 (can check https://prarena.ai/ for one measure of performance):

---

## The Tooling Landscape Today

Cloud-based coding tools:
    - Replit
    - Lovable
    - Bolt

---

## The Tooling Landscape Today

Standalone Chat tools:
    - ChatGPT
    - Perplexity
    - etc.

---

## The Tooling Landscape Today

Today's Top Models
    - GPT-5
    - Claude 4
    - Gemini 2.5

 (can check https://www.swebench.com/ for one measure of performance):

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
    - Code way too complex/long/ugly
    - Code performance could be much better

---

## LLM Workflows I use most

* Claude for vibe-coding -- "give me a website that does x"
* Cursor as extra-powerful auto-complete
* Cursor as agent
    - Choose a model
    - Describe the task, how to test it, etc.
    - Let it go, review code/output, provide feedback, repeat

---

## Tips and Tricks

* Let the models fight
    -  "My coworker wrote this, but I don't think it's right"
* You're the PM
* Ask it to make a plan for the approach it will take, write down steps, then review it
* Learn to use the tool's pre-instructions (e.g. .cursor/rules, CLAUDE.md)
* Give it the right context--point to files, docs urls, etc.

---

## Tips and Tricks

* Set up good rules in your repo (e.g. linting and testing with pre-commit hooks)
* Empower it to check the work (e.g. "use npx <tool> to run a SQL query", "use use uvx pytest to run all the tests")
* Don't PR code unless you're willing to maintain it
* https://www.anthropic.com/engineering/claude-code-best-practices -- generally helpful

---

## Demos

* Fancy auto-complete/refactoring
* Quick one-off code generation with new library feature
* Real-world codebase understanding/refactoring


---
<!-- _paginate: skip -->

## Q&A

Questions, comments, ideas?
