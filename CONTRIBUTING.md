# Contributing to the Hushcue website

**What to read first:**
1. **[docs/BRIEF.md](docs/BRIEF.md):** what to build.
2. **[MEMORY.md](MEMORY.md):** the rules that never change.

## 1. Authorship
- **Commit under your own name and email:** the person whose GitHub account pushes the commit is its author.
- **Never credit an AI tool as author or co-author:**
  - no `Co-Authored-By` lines, and no "Generated with…" lines
  - not in commits, pull requests or code comments
- **AI tools are fine to use.** You own the code you submit, so read every line of it.

## 2. Workflow: branch → pull request → review → squash-merge

```bash
git switch main && git pull
git switch -c feat/home-hero            # one branch per change
# ...work, run the checks...
git add -A && git commit -m "feat(home): add the hero section"
git push -u origin feat/home-hero
gh pr create --fill                     # or open it on github.com
```

### Branch names

| Prefix | For |
|---|---|
| `feat/<topic>` | a new page or section |
| `fix/<topic>` | a bug fix |
| `docs/<topic>` | documentation |
| `refactor/<topic>` | restructuring |
| `chore/<topic>` | maintenance |

### Rules for pull requests
- **Never push straight to `main`.** Every change goes through a pull request.
- **One pull request does one thing.**
- **Visual changes need screenshots** (desktop and mobile).
- **Review:** Cyrus reviews every pull request (CODEOWNERS requests him automatically).
- **Merging:** once it is approved and the checks pass, use **squash and merge**.

### Commit messages: [Conventional Commits](https://www.conventionalcommits.org/)
- **Format:** `type(area): what changed`, at most 72 characters.
- **Types:** `feat`, `fix`, `docs`, `style`, `refactor`, `perf`, `chore`, `ci`.
- **Areas:** the page or part changed: `home`, `features`, `download`, `pricing`, `docs`, `privacy`, `layout`, `seo`.

## 3. Before every pull request
- [ ] The site builds, and lint and typecheck pass.
- [ ] It works on mobile and desktop, in light and dark themes.
- [ ] No tracking scripts, cookies or third-party widgets were added.
- [ ] All text is honest (see the brief) and all design is original.
- [ ] No secrets or `.env` files are committed.
