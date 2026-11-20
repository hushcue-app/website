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
- **The repo is public,** so `main` is protected (Cyrus's decision, 2026-11-20). The ruleset `protect-main`:
  - no direct pushes, force-pushes or deletion
  - every change through a pull request, with 1 approval from a code owner (Cyrus), threads resolved, and stale approvals dismissed on new pushes
  - repo admins may merge their own pull requests without an approval, but still only through a pull request
  - squash-merge only
- **Never write these in repo files** (docs, code, comments, commits or pull requests). Maintainers keep them in private notes outside the repo:
  - who is assigned to what, and start dates
  - people's access levels
  - personal contact details
  - business plans (pricing, paid tiers, deals)
  - account and domain status
  - private feedback about people
  - the backstory of decisions (2026-11-20)
- **Original design and words only:** never copy other copilot or interview-tool websites (layouts, mock-ups, text, images). (2026-11-20)
- **No tracking:** no analytics, pixels, session replay or cookies. Cookieless visitor counts only, and only with Cyrus's OK. (2026-11-20)
- **Honest claims:** never "undetectable", "pass any interview" or "guaranteed". Never name competitors. (2026-11-20)

## Decisions
- **Design bar:**
  - the site must look **very good, clear and premium** (`docs/BRIEF.md` §2)
  - the product is the hero, with restraint and one accent colour
  - Cyrus approves the visual direction (fonts, colours, hero) **before** any pages are built (2026-11-20)
- **One shared design system** for the app and the site: `design/` in the app repo (`tokens.css`, `DESIGN.md`, `preview.html`), v0.1, 2026-11-20. Its decisions:
  - **Fonts:** Geist, Geist Mono and Instrument Serif.
  - **Colour:** one accent, cue teal; mode tints only as small accents.
  - **Icons:** Lucide.
  - **The collapsed live UI is the "orb".**
  - **The site copies `tokens.css`** and never invents its own colours or fonts. Changes to the look go to the design system first.
- **Quality reference: railway.com,** chosen by Cyrus (2026-11-20).
  - **What to learn:** the product drawn in code on the page, a mode switcher under the hero scene, and the same anatomy in every section (label pill → serif headline → short text → three feature rows → product scene).
  - **Scroll effects:** gentle fade-ins only, with no heavy parallax or scroll hijacking.
  - **What never to copy:** Railway's own signature pieces (the track rail, the split-flap board, the sky art, their words and colours).
  - **Our signatures:** a sound-wave progress line, the mode switcher, and the "you see / they see" stealth slider.
- **Showing the app before it exists:**
  - design the app's live UI first, as one shared look for app and site
  - the site shows it with coded, scripted "product scenes" labelled "Interactive preview"
  - real recordings are added as each part ships
  - every feature has a status badge (Available / In development / Planned)
  - never invent testimonials, user counts, logos or numbers (2026-11-20)
- **What the site is:** the website for Hushcue (desktop app repo: `hushcue-app/hushcue`). The pages are listed in `docs/BRIEF.md`. (2026-11-20)
- **Stack:** Next.js + TypeScript + Tailwind is suggested, not settled. The first pull request may propose otherwise. (2026-11-20)
