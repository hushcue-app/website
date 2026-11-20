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

## 2. Look and feel: premium and clear

**The bar:** the site must look **very good, clear and premium**, the way the best developer-tool sites do.
- Study sites like Linear, Vercel, Raycast and Stripe for their **level of polish**: spacing, type, restraint, motion.
- Never copy their layouts, wording or assets. Our look is our own.

### Principles
1. **The product is the hero.** Real, crisp product visuals do the selling, not stock art or cartoons.
2. **Restraint.**
   - Lots of space, and one idea per section.
   - One accent colour.
   - Nothing on the page that doesn't earn its place.
3. **Clarity.**
   - A visitor understands what Hushcue does from the hero alone, in 10 seconds.
   - Every section has a plain headline, at most two short lines under it, and one visual.
   - Only one primary button per screen.
4. **Details are the premium:**
   - perfect alignment
   - consistent corner radii and spacing
   - designed hover and focus states
   - a designed 404 page, favicon and Open Graph images
5. **Speed is part of the feel.** It loads instantly: no layout shift, no spinner, no heavy scripts.

### Typography
- **Typefaces:** one high-quality typeface family, or a refined pair (an elegant display face for big headlines, a clean sans for body text). Self-hosted, open-licensed fonts only.
- **Type scale:** for example 72 / 56 / 40 / 28 / 20 / 16 px on desktop, scaled down on mobile.
- **Display headlines:** slightly tight letter-spacing.
- **Body text:** 16–18 px, with a line length of 60–75 characters.

### Colour
- **Dark first, with an equally polished light theme:**
  - a near-black background
  - off-white text
  - quiet greys for secondary text
  - hairline borders (about 8% white on dark)
- **Accent:** one calm colour, used sparingly: the main button, links, key highlights.
- **Gradients and glows:** subtle, only behind product visuals. Never rainbow gradients.
- **Contrast:** all text passes WCAG AA.

### Layout and spacing
- **Grid:** a 12-column grid, with content at most ~1200 px wide.
- **Spacing:** an 8 px scale. Big vertical rhythm between sections (about 120–160 px on desktop).
- **Corner radii:** one consistent set, for example 12 / 16 / 24 px.

### Visuals
- **Product shots:** high-resolution (2×) screenshots and short, muted, looping clips of the real live window over a realistic call.
  - Clips are WebM/MP4, under 2 MB each, with a poster image.
  - They sit in clean window frames with a soft shadow or glow.
- **Signature moment: the stealth explainer.** A "you see / they see" comparison the visitor can slide between: one side shows the call with Hushcue's answers on top, the other shows the same screen as the interviewer sees it, with Hushcue gone.
- **Icons:** one open-source set (Lucide or Tabler), one stroke weight, used everywhere.
- **No stock photos,** and no clip-art mascots at launch.

### Motion
- **On scroll:** subtle fades and slides as content appears (200–400 ms, ease-out). No heavy parallax.
- **Small touches:** micro-interactions on buttons and cards.
- **Reduced motion:** everything respects `prefers-reduced-motion`.

### Words
- **Style:** short, confident, specific. Plain words, no buzzwords.
- **Numbers:** only true ones (for example measured answer speed, install size, cost per interview), and only once they are measured.

### Quality gate (how "premium" is checked)
- **Direction first:** the visual direction is approved by Cyrus **before** the pages are built (first pull request, §5).
- **Screenshots in every visual pull request:** at 1440 px and 390 px wide, in light and dark themes.
- **Lighthouse:** ≥ 95 in every category on mobile.
- **What gets sent back:**
  - anything misaligned, inconsistent or cluttered
  - anything slow to load

---

## 3. Rules

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

## 4. Suggested stack

| Part | Suggestion |
|---|---|
| Framework | Next.js (App Router) + TypeScript |
| Styling | Tailwind CSS |
| Docs | MDX pages |
| Hosting | Vercel or Cloudflare Pages (free tier) |
| Domain | `hushcue.app` (not bought yet; Cyrus decides) |

**Not settled yet.** The developer may propose another stack (for example Astro) in the first pull request, with the reason.

---

## 5. First pull requests (suggested order)
1. **Visual direction, for Cyrus to approve:**
   - a short moodboard
   - the chosen fonts, colour tokens (dark and light), spacing scale and radii
   - a designed home-page hero (in Figma, or coded as a single page)
   - **Nothing else gets built until this is approved.**
2. **Project scaffold:** linting, the design tokens as code, the base layout (header, footer), and the theme switch.
3. **The home page:** placeholder product visuals, and the stealth "you see / they see" explainer.
4. **More pages:** Features, Download and Pricing (with the cost calculator).
5. **Docs and legal:** Docs (MDX), Privacy, Responsible use, Terms and the 404 page.
6. **Finishing:** SEO metadata, Open Graph images, the sitemap, and the Lighthouse pass.
