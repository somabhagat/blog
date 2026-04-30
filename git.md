# 🚀 Antigravity Blog Project & Setup Guide

This repository contains my personal blog HTML files, Antigravity workspace settings, and my complete Branding & Content Strategy.

## 💻 How to Set This Up on a New PC

If you are reading this from a brand new computer, follow these steps to get back to work:

### Install Git
- Download Git for Windows.
- **Important:** If using a secondary drive (like `Q:`), remember the path! (e.g., `Q:\Program Files\Git`).
- During installation, ensure "Add to PATH" is checked.

### Configure Your Identity
Open **Git Bash** and type these two commands so Git knows who is saving the work:
- `git config --global user.email "bhagatsoma@gmail.com"`
- `git config --global user.name "somabhagat"`

### Connect to GitHub
To allow the PC to upload to your private account without a password:
- Open Git Bash and run: `git config --global credential.helper manager`
- The first time you "Push," a window will pop up. Sign in via your browser.

### Fix the Antigravity Source Control and Terminal
If the colorful terminal (Git Bash) doesn't show up inside the Antigravity editor:
1. Press `Ctrl + Shift + P` and search for **"Open User Settings (JSON)"**.
2. Add the path to the git executable: `"git.path": "Q:\\Program Files\\Git\\bin\\git.exe"`
3. In the **Workspace Settings** (`blog.code-workspace`), ensure the terminal profile points to: `Q:\\Program Files\\Git\\bin\\bash.exe`.

---

## 📝 Daily Workflow (How to Save)

Don't use the Windows Command Prompt. Use the **Terminal window at the bottom of Antigravity** (make sure it says `bash`).

### Step 1: See what you changed
`git status`

### Step 2: Stage changes
`git add .`

### Step 3: Commit
`git commit -m "Write a note here about what you did"`

### Step 4: Push
`git push origin main`

---

# Brand & Content Strategy

## Core Content Pillars
- **Payments & Strategy (Blue):** The "Why" and "How" of money movement. Includes Regulation (PSD3), Infrastructure (SEPA, SIC), Standards (ISO 8583), and Products (Wero, BaaS).
- **Engineering & AI (Green):** The "Builder" perspective. Includes DevOps, AI Agents in Payments, and technical architecture.
- **Motivational & Resilience (Yellow):** The "Human" perspective. Personal branding, career navigation, and industry mindset.

## Social Media Schedule
| Day | Time Window | Content Format | Strategy |
| :--- | :--- | :--- | :--- |
| **Tuesday** | 10:00 AM – 11:00 AM | Carousel (Technical) | "Power Day" for deep insights. Senior tech professionals check LinkedIn after morning stand-ups. |
| **Friday** | 9:00 AM – 11:00 AM | Blog Share (Summary) | Engagement drops after noon, so morning summaries perform best. |

---

# Content Idea Bank

## Next Priority Topics (Germany/EU Focus)
- **Bill Payments:** The friction in recurring household payments.
- **Stablecoins:** Corporate treasury use cases vs. retail hype.
- **Wero:** The final battle for the European checkout interface.
- **The EU AI Act & Payments:** Mapping compliance to actual code.

## Global Market Research (Secondary Focus)
- **Pix (Brazil):** The global benchmark for central-bank-driven instant payment adoption.
- **UPI (India):** How interoperability solved the "last mile" of financial inclusion.
- **FedNow vs. RTP (USA):** The fragmentation of the American instant payment landscape.
- **The Nordic Model (Swish/Vipps/MobilePay):** Cross-border P2P consolidation.

---

# AI Content Generation Prompts

## Low Friction LinkedIn Posts
- **Authority-First Listicle:** Create a list of 5 "Technical Truths" that sales decks usually miss. Tone: "I’ve seen the backend, here is the reality."
- **Regulatory Translation:** Take a dry regulatory update (e.g., PSR) and translate it into "Human" for Product Managers.
- **Dual-Profile Hook:** Frame career transitions as a "Research & Specialization" phase. Turns a gap into a strength.

## Informative Blog Deep Dives
- **Technical Depth:** Ensure blogs reflect 13 years of seniority (Mastercard/IHK background).
- **Shared Industry Trauma:** Use "Insider" jokes to build tribe engagement. See the **Reference Section** below for inspiration.
- **The Hook:** Use "Dwell Time" optimization (e.g., "I spent 13 years in Payments and 6 months in AI Agents...").

---

# Technical & Design Standards

## Design Principles
- **Color System:** Blue (Payments), Green (Engineering), Yellow (Motivational). Red is merged into Blue for German/EU market focus.
- **Golden Template:** Every blog MUST include a "References & Resources" section to ensure academic integrity.
- **Byline:** Use "Soma Bhagat, Payments Product Leader | Payment Strategy Blog".

## AI Layout Instructions
- **Timeless Dates:** Never hardcode months/years. Use "at the time of writing".
- **Diagram Flows:** Use "S-Curve" (zigzag) logic for multi-layer .diagram-wrap components.
- **Image Paths:** Always use relative paths: `src="images/filename.svg"`.
- **Maps:** Prefer factual SVG vectors from Wikimedia over AI-generated images to avoid geographic hallucinations.

---

# Reference: Shared Industry Trauma & Terminology

Use these "insider" definitions to build a tribe and show that you've "been in the room."

1. **Acquirer** – The merchant's bank. The middleman nobody talks about.
2. **Issuer** – The customer's bank. The one that says yes or no.
3. **Interchange** – The fee that travels invisibly with every card swipe. You never see it. It's always there.
4. **Chargeback** – When the customer calls their bank and says, "I didn't do it." Merchants cry.
5. **PCI DSS** – A long compliance checklist that makes everyone nervous.
6. **Settlement** – When the money finally, actually moves. Usually T+1 or T+2. Patience.
7. **Authorisation** – The card network asking, "Got the funds?" and the issuer saying, "Maybe."
8. **Tokenisation** – Your card number in a witness protection program.
9. **Payment orchestration** – Having a backup plan for your backup plan.
10. **A2A payments** – Skipping Visa and Mastercard entirely. They're not happy about it.
11. **ISO 20022** – XML-based messaging standard. Thrilling at parties.
12. **Scheme** – Visa and Mastercard. The landlords of card payments.
13. **MDR** – The small cut the merchant never fully understood when they signed up.
14. **3DS** – The extra step that makes you find your phone to complete a €4 purchase.
15. **Open Banking** – Your bank finally sharing your data. Reluctantly.
16. **Soft decline** – “not now.” The most optimistic kind of failure.
17. **Hard decline** – “not ever.” Brutal, but honest.
18. **Scheme fees** - Fees that are invisible for merchants and unpredictable for charging.
19. **BIN** - The first 6-8 digits that decide your fate before the transaction even starts.
20. **FX markup** - Where “competitive rates” quietly disappear.
21. **Blacklisting** - One mistake, permanent memory.
22. **Transaction ID** - A unique identifier that every player generates in a different format, helping them point at each other when customers get angry.
23. **KYC** - When a merchant or bank requires you to prove your existence.
24. **Callback or webhook** - When one system tells another system the final status of a transaction.
25. **Reversal** - When you make a wrong transaction and ask the issuer bank to reverse the money.
26. **PAN / FPAN / DPAN** - Because remembering one number is too easy.
