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
A Railway-style story, explained in §2 under "The reference: Railway-level polish".
1. **Hero:**
   - a serif headline (two lines at most) and a one-line sub-line
   - Download and "View on GitHub" buttons
   - a **large product scene** below: the live window over a realistic video call, in a framed window on an atmospheric background of our own design
   - a **mode switcher** under the scene: Interview · Coding · Meeting · Assessment. It swaps the scene in place.
2. **One section per idea,** each built the same way (§2 "Section anatomy"):
   - **Interview:** the cue card under your camera: the question, the whole answer from your own stories, and live captions. (Headline to be written fresh, in our own words.)
   - **Coding:** reads the problem on your screen; gives the approach, code and complexity, or hints only.
   - **Meeting and Notetaker:** live notes, decisions, action items, and talking points when you are asked.
   - **Online assessment:** the likely answer, with an honest confidence level.
   - **Stealth (the signature section):** the interactive "you see / they see" slider.
   - **Yours only:** bring your own key, local storage, no tracking, open source.
   - **AI interview practice:** rehearse against an AI interviewer. Badge: Planned.
3. **Proof:** once real, GitHub stars, releases and contributor counts, pulled live. Until then this section does not exist; never use invented numbers.
4. **FAQ:** 5–6 questions.
5. **The final call to action,** then the footer.

### Features (`/features`)
1. **One section per mode:** Interview, Coding, Meeting, Online assessment.
2. **The Notetaker.**
3. **The live view:** the cue card (question, answer, live captions), the side panel, the command palette; Full, Compact and Orb views; transparency per surface.
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
3. **Practice mode:** "coming later".

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

### The shared design system (use it, don't reinvent it)
The app and the website share **one design system**. It lives in the app repo, in the `design/` folder of `hushcue-app/hushcue` (you have read access):
- **`tokens.css`:** every colour (dark and light), font, type size, spacing step, radius, shadow and motion timing. Copy this file into the site and use only its variables.
- **`DESIGN.md`:** principles, brand, colour, typography, the Lucide icon map, every component, and every app screen and live layout.
- **`preview.html`:** open it in a browser to see everything, including the live window over a call with a working transparency slider. The site's product scenes should look exactly like this.

**Already decided there:**

| | Decision |
|---|---|
| **Fonts** | **Geist** (UI and body), **Geist Mono** (code, keys, numbers), **Instrument Serif** (headlines). All open-licensed; self-host them. |
| **Accent** | One brand colour, **cue teal** (`#2fd3b3` dark / `#0e9f86` light) |
| **Mode tints** | Small dots, labels and faint glows only: Interview teal, Coding periwinkle, Meeting amber, Assessment rose |
| **Icons** | **Lucide**, 1.75 px stroke |

**On the website:**
- **Display sizes:** 72 / 56 / 40 px headlines with -0.02em letter-spacing.
- **Body text:** 16–18 px, with a line length of 60–75 characters.
- **Layout:** a 12-column grid at most ~1200 px wide, 120–160 px between sections on desktop.
- **Gradients and glows:** subtle, only behind product visuals.
- **Contrast:** WCAG AA.

**Want to change the look?** Propose it as a pull request to the design system in the app repo, not as a one-off on the site.

### Visuals
- **Product shots:** high-resolution (2×) screenshots and short, muted, looping clips of the real live window over a realistic call.
  - Clips are WebM/MP4, under 2 MB each, with a poster image.
  - They sit in clean window frames with a soft shadow or glow.
- **Signature moment: the stealth explainer.** A "you see / they see" comparison the visitor can slide between: one side shows the call with Hushcue's answers on top, the other shows the same screen as the interviewer sees it, with Hushcue gone.
- **Icons:** Lucide, 1.75 px stroke, used everywhere (as in the design system).
- **No stock photos,** and no clip-art mascots at launch. The brand mark is three rising sound bars; the collapsed live UI is called the **orb**.

### Motion
- **On scroll:** subtle fades and slides as content appears (200–400 ms, ease-out). No heavy parallax.
- **Small touches:** micro-interactions on buttons and cards.
- **Reduced motion:** everything respects `prefers-reduced-motion`.

### Words
- **Style:** short, confident, specific. Plain words, no buzzwords.
- **Numbers:** only true ones (for example measured answer speed, install size, cost per interview), and only once they are measured.

### Showing Hushcue before it is built
The app is still being built, so the site shows it in three stages.

**Stage 1: design the app's live UI first, as one look for app and site.**
- **What gets designed:** the cue card (one for each mode), the side panel and its tabs, the command palette, the orb, pre-flight, Today and an opportunity page. **Done as v0.3 in the design system** (`design/preview.html` in the app repo).
- **Everything follows the shared design system:** the same fonts, colours and radii. The app's Phase 1 builds from these designs too.
- **So the website never shows a product that looks different from the real one.**

**Stage 2: interactive "product scenes" on the site, coded rather than filmed.**
- **What a scene is:** the live window recreated in code from those designs, playing a scripted session. For example:
  - an interviewer's question appears in the transcript
  - the question appears, the answer's points fill in, and the live captions roll
  - the visitor can drag the transparency slider and switch between Interview, Coding, Meeting and Online assessment
- **The stealth explainer** is a scene too: slide between "you see" (the call, with Hushcue's answers on top) and "they see" (the same call, with Hushcue gone).
- **Why code instead of video:**
  - sharp at every size
  - tiny to load
  - follows light and dark themes
  - updates when the design changes
- **Every scene carries a small "Interactive preview" label.**
- **Scripted content is fictional:**
  - an invented role and company, an invented candidate
  - no real people, no real companies, no one's actual resume
- **The scripted answers must be good answers.** They are the product's first impression.

**Stage 3: real proof, once each part works.**
- As each part of the app ships, add real screen recordings and screenshots next to, or instead of, the scenes.
- Example: once the app's cue card exists, a 10-second real clip of it answering in a call.
- The scenes stay, because they explain things well. The recordings prove they are real.

**Honesty rules while the app is unfinished:**
- **A status badge on every feature:** **Available**, **In development** or **Planned**. Today almost everything is In development, and that is fine. Open-source projects that show their roadmap earn trust.
- **Download page:** says "Coming soon" until there is a real installer. Its main call to action is "Get notified" or "Watch on GitHub" (the second only once the repo is public).
- **Never invent:** testimonials, user counts, download numbers, company logos, ratings or press quotes.
- **No numbers until they are measured:** answer speed, install size and cost per interview appear only once measured.

### The reference: Railway-level polish
Cyrus's chosen bar is **railway.com**: clean, professional, and showing what the product is straight from the landing page.

**Patterns to learn from:**
- **The product is drawn in code.** The landing page rebuilds the real app interface as live, crisp UI (dashboards, logs, cards), not screenshots. **Our version:** the product scenes (§2 "Showing Hushcue before it is built").
- **A product tab bar under the hero scene** switches between the product's main areas in place. **Our version:** the mode switcher.
- **Every section is built the same way** (see "Section anatomy" below), so a long page still reads calmly.
- **Text and visuals alternate.** Words on the left, product scene on the right, or the scene full-width under the words. There is plenty of empty space around both.
- **Section colours:** one brand accent, plus a soft tint per section, used only in its small label and a faint glow behind its scene. Never loud.
- **Serif headlines and sans-serif body text.** The headlines feel editorial and calm; the body stays easy to read.
- **Hairline borders, gently rounded cards, quiet grey secondary text.**
- **A rich footer:** grouped link columns (Product, Resources, Project, Legal).

**Section anatomy** (every content section):
1. A small coloured **label pill** (for example "Interview", "Stealth").
2. A **serif headline**, one idea, at most two lines.
3. **Two or three sentences** of plain text, then "Learn more →".
4. **Three feature rows,** each an icon, a bold short title and one grey line.
5. The **product scene** for that section.

**Scroll effects:** a little, never much.
- **Content arrival:** content fades and rises 16–24 px as it comes into view, once (300–500 ms, ease-out).
- **Scenes start when seen:** each product scene starts playing when it scrolls into view, for example the answer begins to stream.
- **One quiet progress element** runs down the left side of the story sections and fills as you scroll. **Ours must be our own idea:** for example a thin **sound-wave line** that lights up section by section, as if Hushcue is listening. It fits the product.
- **No scroll hijacking,** and no parallax beyond a very slight drift on the hero background.
- **`prefers-reduced-motion`:** everything becomes static.

**What we must NOT copy:**
- **Railway's own signature elements:** the train-track progress rail, the split-flap stats board, the illustrated sky hero, their wording, icons and colours.
- **Learn the level, not the look.** Our signature pieces are the sound-wave progress line, the mode switcher and the "you see / they see" stealth slider.

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
| Domain | Chosen by Cyrus |

**Not settled yet.** The developer may propose another stack (for example Astro) in the first pull request, with the reason.

---

## 5. First pull requests (suggested order)
1. **The home-page hero, for Cyrus to approve:**
   - built with the shared design system's tokens, fonts and icons
   - the hero headline, the live-window product scene and the mode switcher
   - Include desktop and mobile screenshots, in light and dark.
   - **Nothing else gets built until this is approved.**
   - Suggestions for the design system itself go to the app repo as a pull request.
2. **Project scaffold:** linting, `tokens.css` copied in, self-hosted fonts, the base layout (header, footer), and the theme switch.
3. **The home page:** the interactive product scenes (scripted, labelled "Interactive preview") and the stealth "you see / they see" explainer.
4. **More pages:** Features, Download and Pricing (with the cost calculator).
5. **Docs and legal:** Docs (MDX), Privacy, Responsible use, Terms and the 404 page.
6. **Finishing:** SEO metadata, Open Graph images, the sitemap, and the Lighthouse pass.
