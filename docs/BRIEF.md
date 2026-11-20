# Website brief

The public website for **Hushcue**, an open-source desktop coach for job interviews, coding rounds, online assessments and meetings. The product itself lives in the `hushcue-app/hushcue` repo.

## Goal

Explain Hushcue in 10 seconds, show it working, earn trust (private, honest, open source), and get people to download it or star the repo.

---

## 1. Pages (launch set)

| Page | Path | Sections |
|---|---|---|
| **Home** | `/` | See below |
| **Features** | `/features` | See below |
| **Download** | `/download` | See below |
| **Pricing** | `/pricing` | See below |
| **Docs** | `/docs` | See below |
| **Privacy** | `/privacy` | See below |

### Home (`/`)
1. **Hero:** one-line promise, a sub-line, Download and "View on GitHub" buttons.
2. **Demo:** a short looping clip of the live window answering a question.
3. **The four modes:** Interview, Coding, Meeting, Online assessment.
4. **How it works:** 3 steps (listen → understand → answer).
5. **The stealth explainer:** "what you see vs. what they see".
6. **Privacy and bring-your-own-key.**
7. **AI interview practice:** marked "coming later".
8. **FAQ:** 5–6 questions.
9. **A final call to action.**

### Features (`/features`)
1. **One section per mode:** Interview, Coding, Meeting, Online assessment.
2. **The Notetaker.**
3. **The live window:** transparency slider, snapping, compact and bird layouts.
4. **Keyboard shortcuts.**
5. **Supported AI providers.**

### Download (`/download`)
1. **The Windows installer button.**
2. **System requirements.**
3. **macOS and Linux:** "coming soon".
4. **A link to the release notes.**

### Pricing (`/pricing`)
1. **"Free and open source. Bring your own key."**
2. **A cost calculator:** pick a provider and the interview length, and see the estimated API cost.
3. **Practice mode:** "coming later" (the future paid tier).

### Docs (`/docs`)
1. **Install.**
2. **Add your API keys.**
3. **Your first session.**
4. **Shortcuts.**
5. **Troubleshooting:** audio devices, Windows permissions.

### Privacy (`/privacy`)
1. **The data that exists,** and where it lives (on your computer).
2. **What is never collected.**
3. **Plain language first,** then the formal text.

### Footer
- Responsible use (`/responsible-use`)
- Terms (`/terms`)
- Changelog (`/changelog`)
- GitHub
- A copyright line

### Responsible use (`/responsible-use`)
- **What Hushcue will never do:** no impersonation, no deepfakes, no voice cloning.
- **What the user is responsible for:**
  - following the rules of their interviews and tests
  - telling people when they record a meeting

---

## 2. Rules

### Honest claims only
- **Say what it does:** it helps you show your best, privately, in a call you are really in.
- **Never say:**
  - "undetectable"
  - "pass any interview"
  - "guaranteed", or money-back promises
- **Never name or compare with competitors.**

### Original design and words
- **Everything is our own:** layout, illustrations, mascot, icons and text.
- **Never copy** other copilot or interview-tool websites: no layouts, mock-ups, wording or images.
- **Icons:** open-source sets with a permissive licence (for example Lucide or Tabler).

### No tracking
- **No Google Analytics,** no ad pixels, no session replay, no third-party chat widgets.
- **Visitor counts:** if wanted, only a cookieless tool (Cloudflare Web Analytics or Plausible), and only after Cyrus agrees.
- **No cookie banner,** because there are no cookies to ask about.

### Fast and accessible
- **Lighthouse:** ≥ 95 for performance, accessibility, best practices and SEO, on mobile.
- **Responsive and keyboard-navigable,** with visible focus and alt text on every image.
- **Light and dark themes,** following the system setting.
- **Motion:** respect `prefers-reduced-motion`.

### SEO
- **Every page:** a unique title and description, an Open Graph image, and a canonical URL.
- **Site-wide:** a `sitemap.xml` and `robots.txt`.

### Screenshots and demo clips
- **Use only Hushcue itself.** Until the app is ready, use clearly marked placeholders. Cyrus provides the real captures.

---

## 3. Suggested stack

| Part | Suggestion |
|---|---|
| Framework | Next.js (App Router) + TypeScript |
| Styling | Tailwind CSS |
| Docs | MDX pages |
| Hosting | Vercel or Cloudflare Pages (free tier) |
| Domain | `hushcue.app` (not bought yet; Cyrus decides) |

**Not settled yet.** The developer may propose another stack (for example Astro) in the first pull request, with the reason.

---

## 4. First pull requests (suggested order)
1. Project scaffold, linting, the base layout (header, footer) and theme.
2. The home page with placeholder visuals.
3. Features, Download and Pricing (with the cost calculator).
4. Docs (MDX), Privacy, Responsible use and Terms.
5. SEO metadata, Open Graph images, sitemap and the Lighthouse pass.
