# 🚀 MVP SPEEDRUN: 7-DAY LAUNCH PROTOCOL

**Context for Agent:**
We are executing a "Vibe Coding" sprint.
*   **Goal:** A working, sellable MVP in 7 days.
*   **Stack:** Izi SaaS Kit (Next.js 15, Tailwind, Supabase).
*   **Rule:** If a feature takes >4 hours to build, we cut it. **Simplicity is the feature.**

---

## 📅 DAY 1: THE SKELETON & DEPLOY
**Goal:** Hello World in Production.
**Focus:** Infrastructure, Config, Auth.

*   **Task 1:** Clone Izi SaaS Kit.
*   **Task 2:** Configure `izi.config.ts` (Set App Name, Theme, Description).
*   **Task 3:** Setup Supabase Project (Database + Auth).
*   **Task 4:** **DEPLOY TO VERCEL.** (Must happen on Day 1).

> **Agent Prompt:**
> "Initialize the project based on `izi.config.ts`. Connect Supabase Auth using the 'Magic Link' method (simplest). Deploy to Vercel and verify the live URL. Do not build UI yet, just the plumbing."

---

## 📅 DAY 2: THE FACE (LANDING PAGE)
**Goal:** User falls in love before they login.
**Focus:** Hero, Value Prop, Mobile Dock.

*   **Task 1:** Customize Hero section (Copywrite + Visual).
*   **Task 2:** Setup MobileDock (Glassmorphism check).
*   **Task 3:** Create "Features" grid (Sell the benefits).
*   **Task 4:** Add a "Waitlist/Signup" button that leads to Auth.

> **Agent Prompt:**
> "Build the Landing Page using izi-blocks. Use the 'Glass' theme settings. Ensure the MobileDock is visible on small screens. The 'Get Started' button must redirect to /login."

---

## 📅 DAY 3: THE ONE THING (CORE FEATURE)
**Goal:** The app does **ONE** thing useful.
**Focus:** The main value loop.

*   **Constraint:** Only build the primary function. (e.g., if it's a PDF generator -> Form + PDF Output). No settings, no profiles, no fluff.
*   **Task 1:** Build the Input Interface (Form/Chat).
*   **Task 2:** Connect the Logic (API Route / AI Call).
*   **Task 3:** Display the Result.

> **Agent Prompt:**
> "We are building the Core Feature: [DESCRIBE FEATURE]. Create a simple interface at /dashboard. When the user submits, run [LOGIC] and show the result immediately. Keep it ugly but functional."

---

## 📅 DAY 4: DATA & STATE
**Goal:** Users don't lose their work.
**Focus:** Database, User Dashboard.

*   **Task 1:** Create Supabase Table (e.g., projects, invoices).
*   **Task 2:** Enable RLS (Row Level Security) - Users see only their own data.
*   **Task 3:** Build a "History" or "My Projects" list on the Dashboard.

> **Agent Prompt:**
> "Create a Supabase table for [DATA]. Write an RLS policy so users can only read/write their own rows. Fetch this data on the Dashboard and display it in a simple list."

---

## 📅 DAY 5: MONETIZATION (THE GATE)
**Goal:** The ability to take money.
**Focus:** Pricing, Paywall.

*   **Task 1:** Create a Stripe Payment Link (Product: "Pro Access", Price: $49).
*   **Task 2:** Build a Pricing page/modal.
*   **Task 3:** Gate the "Core Feature" (or limits).
    *   *Simple version:* Just put a "Upgrade" button.
    *   *Hard version:* Check subscription status.
    *   *MVP Hack:* Allow 3 free tries, then redirect to Stripe.

> **Agent Prompt:**
> "Add a 'Pricing' section. Create a limit of [X] uses for free users. If they exceed it, show a modal with a link to [STRIPE_LINK]. No complex webhooks yet, just the UI flow."

---

## 📅 DAY 6: POLISH & SEO
**Goal:** Look professional.
**Focus:** Meta tags, OG Images, Mobile responsiveness.

*   **Task 1:** Fill metadata in `layout.tsx` (Title, Description).
*   **Task 2:** Generate an OpenGraph image (The link preview).
*   **Task 3:** Mobile QA (Open on phone, fix broken padding).
*   **Task 4:** Add a simple "Support" link (mailto: or Twitter DM).

> **Agent Prompt:**
> "Update SEO metadata for [APP NAME]. Generate a generic OG image code or placeholder. Check all paddings on mobile view and fix any overflow issues."

---

## 📅 DAY 7: THE LAUNCH (RED BUTTON)
**Goal:** Ship it.
**Focus:** Final Test, Socials.

*   **Task 1:** Full User Walkthrough (Register -> Use -> Upgrade).
*   **Task 2:** Social Launch:
    *   Twitter Thread ("I built this in 7 days").
    *   Product Hunt (Schedule or Instant).
    *   Reddit (relevant subreddits).
*   **Task 3:** Switch mode to "Marketing".

> **Agent Prompt:**
> "Run a final smoke test. Check console for errors. Verify the Stripe link works. If all green, we are ready to ship."
