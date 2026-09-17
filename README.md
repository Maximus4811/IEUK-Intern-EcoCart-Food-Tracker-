# EcoCart FridgeSmart

**IEUK 2026 Sector Skills Project — Proof of Concept**

A mobile-first grocery inventory and recipe suggestion app designed to reduce household food waste by tracking expiration dates and generating AI-powered meal ideas from items about to go bad.

---

## What It Is

EcoCart FridgeSmart is a UX/UI design prototype for a consumer app that helps budget-conscious households (think time-poor parents and student cooks) stop throwing money away in the bin. The core loop:

1. **Scan your grocery receipt** → OCR extracts line items and auto-logs them to a digital inventory
2. **Track expiration dates** → Each perishable gets an estimated shelf life and a traffic-light urgency tag (red = today, amber = 1–2 days, green = safe)
3. **Get recipe suggestions** → AI generates quick, beginner-friendly meals that prioritize your expiring ingredients
4. **Cook and save** → Completing a recipe decrements your inventory and logs waste prevented

This repo contains the full design system, wireframes, and interactive HTML mockups for the core screens: receipt scanning, inventory dashboard, and AI recipe suggestions.

---

## What It Does (From a User Perspective)

- **Frictionless logging**: Receipt OCR means users don't manually type every item—just snap, confirm, and save
- **Urgency-first dashboard**: Expiring items are surfaced at the top with color-coded cards, so you see what needs using before it's too late
- **Smart recipe generation**: Recipes are ranked by how many expiring ingredients they use, filtered by time (≤30 min) and difficulty (beginner/kid-friendly)
- **Waste tracking**: Users see how much food they've saved from landfill via completed recipes

The design directly supports two personas from the project brief:
- **Sarah (32, working parent)**: Needs 30-minute, kid-friendly dinners using items expiring this week
- **Liam (20, uni student)**: Wants simple, step-by-step leftover recipes with ≤2 extra pantry ingredients

---

## How It Was Built

- **Design**: 100% my own work—wireframes, component hierarchy, color system, and interaction specs
- **Code**: All HTML/CSS/JS mockups generated with **Sonnet** (Anthropic's coding assistant) from my detailed UX prompts
- **Process**: Started from the IEUK PRD excerpt, built low-fi wireframes, then iterated into high-fi interactive prototypes

This isn't a production app end-to-end—there's no backend, no real OCR integration, and no live AI recipe API. But the front-end architecture, component specs, and user flows are production-ready and could be handed to an engineering team to implement.

---

## Repo Structure

```
EcoCart-FridgeSmart/
├── README.md
├── EcoCart_PRD_Excerpt.docx      # Original requirements from IEUK
├── EcoCart_Wireframes.html       # Low-fi mockups (3 core screens)
├── EcoCart_InventoryDashboard.html  # High-fi dashboard mockup
├── EcoCart_ReceiptScanner_UISpec.html  # Camera/OCR screen spec
└── EcoCart_RecipeSuggestions.html   # AI recipe card grid mockup
```

All mockups are self-contained HTML files—open them in a browser to interact with the designs.

---

## Key Design Decisions

- **Traffic-light expiry system**: Red/amber/green tags make urgency scannable in <2 seconds
- **Expiring ingredients banner**: Recipe screen opens by showing which items the AI is trying to save—transparency builds trust
- **Pantry limit**: Recipes require ≤2 supplementary ingredients outside the user's inventory (per PRD constraint)
- **Compact type scale**: Web app typography stays dense and functional (no giant display headings wasting space)
- **Dark mode first**: All mockups default to dark theme with light mode toggle

---

## What's Missing (For Now)

- Backend API for OCR, expiration database, and recipe generation
- User authentication and sync across devices
- Push notifications for 48-hour expiry warnings
- Real inventory persistence and recipe completion tracking

This is a **proof of concept**, not a shippable product. But it's solid grounds for a full implementation—every screen has a clear user story, acceptance criteria, and component spec.

---

## License

MIT License — feel free to fork, adapt, or use this in your own portfolio. Built with AI assistance for the IEUK 2026 Sector Skills Project.

---

## Contact

Samie Qureshi — Liverpool, UK  
[Your GitHub profile link] | [Your LinkedIn/Portfolio]

*Questions? Open an issue or DM me.*
