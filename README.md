# 🌊 WA Holiday Deal Finder

**An AI-powered travel agent that searches the web in real time for the best holiday deals across Western Australia.**

Built by [ECU School of Business & Law](https://www.ecu.edu.au) · Powered by [Claude AI](https://www.anthropic.com)

🔗 **Live App:** [stevend1-cyber.github.io/WA-Holiday-Maker-AI-travel-Agent](https://stevend1-cyber.github.io/WA-Holiday-Maker-AI-travel-Agent/)

---

## What It Does

This is a standalone web app that acts as your personal WA travel agent. You tell it what kind of holiday you're after, and it uses Claude AI with live web search to find current deals on accommodation, transport, activities, and dining across Western Australia.

The app walks you through five steps:

1. **Pick your region** — Perth, Margaret River, Ningaloo, Kimberley, Goldfields, Pilbara, or let AI suggest the best fit
2. **Select your interests** — beach, wine & food, wildlife, adventure, luxury, budget, and more
3. **Choose your duration** — weekend through to extended trips
4. **Set your budget** — from budget to luxury per night
5. **Add details** — preferred travel month, group size, kids, pets, accessibility needs

Then it searches the web and delivers a personalised deal report covering accommodation, transport, activities, dining, money-saving tips, and seasonal timing advice.

---

## Features

- **Live web search** — finds real, current deals with actual prices and provider names (not generic travel guide content)
- **⚡ Fast / 🔬 Detailed modes** — choose between quick results (~10 sec) or deeper research (~30 sec)
- **Compare destinations** — search two regions side by side to help you decide
- **✨ Open to Suggestions** — let the AI recommend the best region based on your interests
- **📅 Seasonal timing** — picks up on your preferred travel month and advises on weather, crowds, and events
- **Follow-up questions** — ask for more detail on any part of the results without starting over
- **🖨️ Print / Save as PDF** — export your results as a formatted, print-ready report with ECU branding
- **Remembers your API key** — saved in your browser so you only enter it once per device
- **ECU branded** — teal and navy colour scheme, Arial typeface, institutional header and footer
- **Fully standalone** — single HTML file, no build tools, no server, no dependencies

---

## Getting Started

### Prerequisites

You need an **Anthropic API key** to use this app. Here's how to get one:

1. Go to [console.anthropic.com](https://console.anthropic.com) and create a free account
2. Click **API Keys** in the left sidebar
3. Click **Create Key** and give it a name (e.g. "Holiday Finder")
4. Copy the key — it starts with `sk-ant-` and is only shown once
5. Add credit to your account under **Plans & Billing** (even $5 USD gives you 100+ searches)

### Cost per search

| Mode | Model | Approx. cost per search |
|------|-------|------------------------|
| ⚡ Fast | Claude Haiku 4.5 | ~$0.01–0.03 USD |
| 🔬 Detailed | Claude Sonnet 4.6 | ~$0.05–0.15 USD |

### Using the app

1. Visit the [live app](https://stevend1-cyber.github.io/WA-Holiday-Maker-AI-travel-Agent/)
2. Paste your Anthropic API key (first visit only — it's saved in your browser)
3. Follow the steps to describe your ideal holiday
4. Review your personalised deal report
5. Ask follow-up questions or export to PDF

---

## Hosting Your Own Copy

This is a single HTML file — no server or build step required.

### Option 1: GitHub Pages (free)

1. Fork or clone this repository
2. Go to **Settings → Pages**
3. Set source to **Deploy from branch → main → / (root)**
4. Your app will be live at `https://yourusername.github.io/your-repo-name/`

### Option 2: Any web server

Upload `index.html` to any static hosting provider (Netlify, Vercel, university web space, etc.) and it works immediately.

### Option 3: Open locally

Double-click `index.html` to open it in your browser. It works offline for the UI, but needs an internet connection for the AI search functionality.

---

## Embedding in Canvas LMS

Canvas strips JavaScript from its HTML editor, so you need to embed via iframe:

```html
<iframe
  src="https://stevend1-cyber.github.io/WA-Holiday-Maker-AI-travel-Agent/"
  width="100%"
  height="800"
  style="border: 1px solid #ddd; border-radius: 8px;"
  sandbox="allow-scripts allow-same-origin allow-forms allow-popups"
  title="WA Holiday Deal Finder">
</iframe>
```

Your Canvas admin may need to allowlist the GitHub Pages domain and `api.anthropic.com` in the Content Security Policy settings.

---

## Technology

- **Frontend:** Vanilla HTML, CSS, and JavaScript (no frameworks, no build tools)
- **AI:** [Anthropic Claude API](https://docs.anthropic.com) with web search tool
- **Models:** Claude Haiku 4.5 (fast mode) / Claude Sonnet 4.6 (detailed mode)
- **Hosting:** GitHub Pages (static)
- **Design:** ECU brand guidelines — Teal (#26B298), Dark Navy (#0E2841), Magenta (#B11D75), Arial typeface

---

## Privacy & Security

- Your API key is stored **only in your browser's local storage** — it is never sent to any server other than the Anthropic API
- No user data is collected, stored, or tracked by this app
- All searches go directly from your browser to Anthropic's API
- The app contains no analytics, cookies, or third-party tracking
- You can clear your saved key at any time using the "Change Key" link

---

## Project Structure

```
WA-Holiday-Maker-AI-travel-Agent/
├── index.html          # The entire app (single file)
└── README.md           # This file
```

---

## Customisation

Since it's a single HTML file, you can easily adapt it:

- **Regions** — edit the `REGIONS` array in the `<script>` section to add or change destinations
- **Interests** — edit the `INTERESTS` array to match your audience
- **Branding** — update the CSS variables in `:root` and the ECU bar HTML to match your institution
- **Prompt** — edit the `buildPrompt()` function to change what information the AI searches for
- **Models** — update the `MODELS` object to use different Claude models

---

## Acknowledgements

- Built as a demonstration of AI-powered consumer decision tools for the hospitality and tourism industry
- Developed by Steven D'Alessandro [Edith Cowan University](https://www.ecu.edu.au), School of Business & Law
- Powered by [Anthropic Claude](https://www.anthropic.com) with web search

---

## Licence

This project is provided for educational and demonstration purposes. All rights are copyrighted by the owner
