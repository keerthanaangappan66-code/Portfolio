# Keerthana A — Portfolio Website
### *"KA — Crafted for the Digital World"*

A premium, recruiter-ready personal portfolio website for **Keerthana Angappan (Keerthana A)**, final-year Bachelor of Computer Applications (BCA) student and aspiring Full Stack Developer.

Built with **React**, **Vite**, modern **Custom CSS**, and high-performance **interactive SVG graph visualization**, with zero bloat and a luxury editorial aesthetic inspired by premium design studios.

---

## ✦ Key Features

- **Editorial Visual Identity:** Custom-crafted geometric `KA` monogram, warm ivory (`#F7F5F0`), deep charcoal (`#1C1B1A`), and muted lavender accents (`#7E6E99` / `#A797C4`).
- **Coordinated Dark / Light Mode:** Smooth theme switcher with automatic preference detection and persistent `localStorage` memory.
- **Interactive Technical Skills Constellation:** Connected-node visual network mapping frontend, programming, database, and analytics technologies with interactive node inspection, workflow linkages, keyboard accessibility, and mobile-friendly selector chips.
- **Project Case Studies:**
  - **MindBuddy** — Mental Health Journal App (Implemented core journaling, mood tagging, and client-side privacy architecture).
  - **Career Pilot** — AI Career Advisor (Concept & prototype exploring undergraduate skill gap diagnostics and career roadmaps).
  - *Distinguishes verified implementation from planned roadmap features with dedicated verification notices.*
- **Internship Timeline:** Editorial experience cards for internships at **Learnlike**, **Coding Blocks**, and **Livewire** with clean placeholders for personal dates and achievements.
- **Academic & Verified Credentials:** Dedicated sections for the BCA degree at *Rathinam College Of Liberal Arts And Science At Tips Global Intitution* and official certifications issued by the *Government of Tamil Nadu*.
- **Contact & Direct Dialogue:** One-click copy email button, secure external links to LinkedIn and GitHub, and an interactive contact form with instant client-side validation and clear instructions for connecting Formspree or EmailJS.
- **Accessibility & Performance:** Semantic HTML5, ARIA labels, focus states, `@media (prefers-reduced-motion)` support, and ultra-fast build times (sub-2.5s).

---

## ✦ Quick Start

```bash
# 1. Install dependencies
npm install

# 2. Run local development server
npm run dev
# The website will be running live at http://localhost:3000/

# 3. Create production build
npm run build

# 4. Preview production build locally
npm run preview
```

---

## ✦ How to Customize Your Content

All your personal details, project descriptions, links, and text are centralized in one single configuration file:
👉 **`src/data/portfolioData.js`**

### 1. Correcting or Updating College Name
In `src/data/portfolioData.js`, update:
```javascript
college: "Rathinam College Of Liberal Arts And Science At Tips Global Intitution",
```

### 2. Adding Your Real Resume
1. Save your resume as a PDF file named **`resume.pdf`**.
2. Place it in the **`public/`** folder: `public/resume.pdf`.
3. The "Resume" download buttons on the navigation bar and drawer will immediately download your real file.

### 3. Adding Real Project Screenshots
1. Capture screenshots of your apps (recommended size: `1200x750` or `16:10` aspect ratio).
2. Save them in `public/projects/` as `mindbuddy.png` and `careerpilot.png`.
3. In `src/data/portfolioData.js`, update the image path:
```javascript
image: "/projects/mindbuddy.png",
```

### 4. Updating Internship Dates & Achievements
In `src/data/portfolioData.js`, locate the `experienceData` array and replace:
```javascript
duration: "Internship Period [Add specific dates / duration]",
```
and fill in your verified tasks in `keyHighlights`.

### 5. Connecting the Contact Form to Receive Real Emails
Static React websites don't run an email server on their own. To receive messages submitted by recruiters directly in your inbox (`keerthanaangappan66@gmail.com`), choose either option:

#### Option A: Formspree (Free & 1-minute setup)
1. Go to [https://formspree.io](https://formspree.io) and register with `keerthanaangappan66@gmail.com`.
2. Create a new form and copy your Form ID (e.g., `xpznkora`).
3. In `src/components/Contact.jsx`, add your Formspree endpoint into the form handler or use standard Formspree action.

#### Option B: EmailJS
1. Install `@emailjs/browser` (`npm install @emailjs/browser`).
2. Add your Service ID and Template ID to dispatch directly on form submit.

---

## ✦ Directory Structure

```
portfolio/
├── index.html                   # HTML template with Google Fonts & SEO meta tags
├── package.json                 # Project dependencies & scripts
├── vite.config.js               # Vite config (port 3000)
├── public/
│   ├── favicon.svg              # Bespoke KA monogram favicon
│   ├── resume.pdf               # Resume download placeholder
│   └── projects/
│       ├── mindbuddy.svg        # MindBuddy preview mockup
│       └── careerpilot.svg      # Career Pilot preview mockup
└── src/
    ├── main.jsx                 # React root
    ├── App.jsx                  # Main application structure & theme state
    ├── index.css                # Color variables, design tokens & typography
    ├── editorial.css            # Component layouts, grids & animations
    ├── data/
    │   └── portfolioData.js     # Centralized content configuration
    └── components/
        ├── Monogram.jsx         # Custom SVG typographic KA monogram
        ├── Navbar.jsx           # Responsive nav, theme toggle & mobile drawer
        ├── Hero.jsx             # Editorial typography & identity frame
        ├── About.jsx            # Biography narrative & core principles
        ├── Projects.jsx         # Case studies showcase
        ├── ProjectModal.jsx     # Deep-dive case study modal dialog
        ├── SkillsConstellation.jsx # Interactive node graph & inspector
        ├── Experience.jsx       # Internship timeline
        ├── EducationCertifications.jsx # BCA degree & state certificates
        ├── Contact.jsx          # Direct email card & validated form
        ├── Footer.jsx           # Editorial signoff & back to top
        └── Icons.jsx            # Brand SVG icons (Github, LinkedIn)
```

---

## ✦ Recruiter Credibility Checklist

- [x] Authentic student & graduate status representation without exaggerated claims.
- [x] Clear demarcation between verified implemented code and conceptual roadmaps.
- [x] Centralized, editable college name and certificate titles matching official wording.
- [x] No invented proficiency scores or progress bars.
- [x] High-contrast, WCAG-compliant color palette with dedicated dark mode.
- [x] Accessible keyboard navigation across all interactive nodes, modals, and drawers.
