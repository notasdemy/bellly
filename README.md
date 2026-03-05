# bellly 🌿
A personal gut health companion app for the low-FODMAP protocol. Built with Lovable.


## What is Bellly?

Most FODMAP apps track what you eat. Bellly tracks your whole life, because IBS doesn't care if it's the garlic or the stress or the terrible night's sleep that set you off.

Bellly is a mobile-first web app built to support the full low-FODMAP journey — from strict elimination, through systematic food reintroduction, all the way to building a personalised new normal. It was born out of personal necessity: managing IBS with severe, fast-onset bloating and needing something that actually fits real life, not just a generic food list.

Most FODMAP apps are either too clinical, too rigid, or ignore the fact that gut health doesn't happen in isolation. Bellly tracks not just what you eat, but the full picture — stress, sleep, training, travel, and other lifestyle triggers that are just as responsible for flares as food.

It's also built for people who train and care about their body composition, so protein and macro tracking sit alongside gut symptom logging without one getting in the way of the other.

---

## Core features

Bellly has 6 tabs:

### 🌅 Today
A scrollable daily overview showing all meals logged, symptoms reported, and a full wellbeing check-in. The wellbeing strip covers stress level, sleep quality, exercise type and intensity, travel, medication, electrolytes (with a polyol warning), and menstrual cycle. A "how's your belly today?" scale sits at the top. Tapping any warning badge on a meal card expands an inline panel showing exactly which ingredients are flagged, colour-coded by severity (🔴 avoid, 🟡 caution) with their FODMAP category. Every logged meal also has an edit button — tap to reopen the full form pre-filled with saved data, change anything, and save.

### ✏️ Log
Add a meal or symptom entry in under 60 seconds. Meals are structured by slot: Breakfast, Morning Snack, Lunch, Afternoon Snack, Dinner, and Evening/Other — each slot can be logged, skipped, or left empty. Within each slot, food and drinks are logged as separate items, each with their own preparation state (raw / boiled / roasted / fried / grilled / fermented). Meal source is tracked (homemade / restaurant / takeout / canteen / friend's / packaged) with a hidden-trigger warning for eating away from home. Every saved meal is automatically checked against the FODMAP database — flagged ingredients show their FODMAP category and expected onset time. Symptom entries capture type, severity, onset speed, and likely trigger. Fast-onset reactions (30–60 min, fructose/polyols) are distinguished from slow-onset ones (1.5–4 hours, fructans/GOS).

### 🔍 Foods
A comprehensive, searchable FODMAP food database of 322+ entries based on Monash University and NHS guidelines, covering fruits, vegetables, grains, proteins, dairy, nuts, condiments, drinks and sweeteners. Foods are rated safe 🟢, portion-dependent 🟡, or avoid 🔴. The database is dynamic — if a "safe" food repeatedly appears before symptom entries, the app flags it and suggests moving it to a personal watch list 🔵. If a food isn't in the database, the user can add it manually with a custom rating, FODMAP category, safe portion, and personal notes — custom entries appear with a ✏️ badge throughout the app. Includes a full smart substitution guide for common triggers (e.g. garlic → garlic-infused oil, soy sauce → tamari, wheat pasta → rice noodles).

### 🧺 Pantry
A lightweight fridge and cupboard tracker. Items flagged as running low surface automatically in a shopping suggestions section, with gut-safe restock recommendations. A "meal ideas from what I have" button suggests simple combinations from current pantry contents.

### 🗺️ Phase
A structured guide through all three phases of the FODMAP protocol:

**Phase 1 — Strict Elimination (4–6 weeks)**
Progress bar, daily compliance heatmap, and a full "foods to avoid" reference card organised by FODMAP category (fructans, GOS, excess fructose, polyols, lactose, and hidden sources). Always accessible so there's no guessing during the hardest phase.

**Phase 2 — Reintroduction**
Tests one FODMAP group at a time. Each group card expands to show individual foods to choose from — so instead of just "test GOS", you pick whether to test chickpeas, lentils, kidney beans, or cashews specifically. Each selected food follows a structured 3-day challenge protocol (small portion → medium portion → rest day), with reaction rating (None / Mild / Moderate / Severe) saved per food. Results build into a "personal FODMAP map" — a colour-coded grid showing exactly what your gut tolerates and what it doesn't.

**Phase 3 — Your New Normal**
Pulls reintroduction results and builds a personalised eating guide: what to eat freely, what to limit by portion, and what to continue avoiding. Reframes the whole process — not as permanent restriction, but as self-knowledge built through data.

### 📊 Insights
Where all the logged data becomes meaningful. Includes:
- Weekly summary snapshot (symptom-free days, most common symptom, average stress and sleep, most flagged ingredient)
- Symptom frequency and severity charts over time
- Trigger food heatmap — automatically ranks ingredients by how often they appeared before a symptom entry
- Wellbeing correlation panel — overlays stress, sleep, training and travel against symptom days to reveal lifestyle patterns
- Meal source breakdown — shows whether eating out correlates with flares
- Protein tracker against a user-set daily goal
- Smart alerts: pattern warnings, trigger food flags, streak nudges, positive milestones, and electrolyte reminders
- CSV / text export for sharing with a doctor or dietitian

---

## Why it's different

**Trigger visibility** — not just a badge count but a full inline breakdown of which ingredients are flagged, colour-coded by FODMAP category, without leaving the Today view.

**Retroactive flagging** — when a food is added or its rating is updated, the app automatically scans all past meal logs and updates every entry containing that food. Past logs get smarter as knowledge grows. A notification tells you how many entries were affected, and a 30-second undo is available.

**Custom food database** — anything not in the built-in database can be added manually. Research it yourself, assign a rating, add notes. Custom entries live alongside database entries throughout the whole app.

**Tracks non-food triggers** — stress, sleep, workout type and intensity, travel distance, electrolytes (which often contain polyols), menstrual cycle and medication all logged alongside diet.

**Meal context matters** — logging where food came from and how it was prepared (raw vs cooked, homemade vs restaurant) adds a layer of nuance most FODMAP apps ignore entirely.

**Onset timing awareness** — fast-onset reactions (30–60 min, fructose/polyols) are tracked separately from slow-onset ones (1.5–4 hours, fructans/GOS) to help connect symptoms to the right meal.

**Built for fitness-conscious users** — protein and macros are first-class fields. Workout type and intensity are tracked because training affects gut motility.

**Three full phases** — not just elimination, but a complete protocol through reintroduction all the way to a sustainable, personalised new normal.

**Insights that surface patterns** — the trigger heatmap and wellbeing correlations turn a daily log into actual understanding of your gut.

---

## Tech

- Built with [Lovable](https://lovable.dev) — a natural language AI app builder
- React (single-page app)
- Mobile-first responsive design
- All data stored locally in the browser — no account, no backend, no data leaves your device
- Warm Sand design palette (`#C17F4A`, `#E8B88A`, `#FBF0E2`) — earthy tones, rounded corners, wellness journal aesthetic
- 322-entry FODMAP food database (`foods.json`) based on Monash University and NHS guidelines

---

## Status

🌱 MVP — actively being built and used personally. Features will evolve based on real daily use through the elimination and reintroduction phases.

---

## Background

This project started as a tool to manage a personal IBS flare-up and figure out, systematically, what was causing the symptoms. The low-FODMAP elimination and reintroduction protocol is evidence-based and effective, but the tools available to follow it felt either too bare-bones or too overwhelming. Bellly is an attempt to fix that — something personal, warm, and actually useful in daily life.

---

## Disclaimer

Bellly is a personal tracking tool, not a medical product. It is not a substitute for advice from a doctor, gastroenterologist, or registered dietitian. If you have IBS or suspect a gut condition, please seek professional guidance, especially before starting an elimination diet.

---

*Designed and built by Emy Osorio — [github.com/notasdemy](https://github.com/notasdemy)*

---
© 2026 Emy Osorio. All rights reserved.
This project is not open source. Please do not reproduce or distribute without permission.
