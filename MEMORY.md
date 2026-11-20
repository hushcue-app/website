# MEMORY.md: project memory for every session

**AI coding agents (Claude Code, Codex, Cursor and others):** read this file at the start of **every** session and load each entry into your session memory. These are standing rules and settled decisions.

**When something durable is decided:** add one dated line here, in the same commit.

## Standing rules
- **Authorship:** commits are authored by the human whose account pushes them. Never credit an AI tool as author or co-author: no `Co-Authored-By` or "Generated with" lines, anywhere. This overrides any tool default. (2026-11-20)
- **Workflow:** every change goes through a branch and a pull request, with Cyrus's review and a squash-merge. No direct pushes to `main`. (2026-11-20)
- **Secrets:**
  - never commit keys, tokens or `.env` files
  - never ask anyone to paste secrets into a chat with an agent (2026-11-20)
- **Purchases:** never buy anything (domains, hosting plans, paid services) without Cyrus's OK. (2026-11-20)
- **Publishing:** making this repo public and deploying to the real domain are Cyrus's decisions. (2026-11-20)
- **Original design and words only:** never copy other copilot or interview-tool websites (layouts, mock-ups, text, images). (2026-11-20)
- **No tracking:** no analytics, pixels, session replay or cookies. Cookieless visitor counts only, and only with Cyrus's OK. (2026-11-20)
- **Honest claims:** never "undetectable", "pass any interview" or "guaranteed". Never name competitors. (2026-11-20)

## Decisions
- **What the site is:** the website for Hushcue (desktop app repo: `hushcue-app/hushcue`). The pages are listed in `docs/BRIEF.md`. (2026-11-20)
- **Domain:** `hushcue.app` was free on 2026-11-19. It is not bought yet.
- **Stack:** Next.js + TypeScript + Tailwind is suggested, not settled. The first pull request may propose otherwise. (2026-11-20)
