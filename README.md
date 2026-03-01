# UX Foundations for Developers
**Cambio Labs — Onboarding Research, Part 1**

---

## What UX Actually Means for Developers

UX isn't a design phase — it's a lens applied across the whole product lifecycle. For developers, that means asking *"what does the user see when this fails?"* not just *"did it work?"*

The practical overlap between UX and dev lives in:
- Component behavior and edge cases
- Accessibility and performance perception
- Error states and empty states — the moments most devs skip

---

## 3 Tools Being Used in the Wild

| Tool / Method | Who's Using It | Why It Matters |
|---|---|---|
| **Journey Mapping** | Etsy (Brooklyn HQ) | Maps emotional highs/lows across a user flow to prioritize backend reliability, not just UI polish |
| **Assumption Mapping** | NY Times Product Design | Cross-functional FigJam sessions to surface risk *before* sprints — designers and devs in the same room |
| **Guerrilla Usability Testing** | BetaNYC (civic tech, NYC) | Fast, low-cost testing in libraries and community centers — catches language and literacy gaps that lab testing misses |

---

## The One I'd Bring to Journey: Onboarding Journey Map

For a first-time user who's never touched the app, the goal isn't to show them everything — it's to get them to one win. That win is **creating their first course**.

A journey map for that flow would look something like:

| Step | User Action | Potential Friction |
|---|---|---|
| **1. Land on the platform** | Arrives at the app for the first time | Unclear what Journey actually does — no context, no "start here" |
| **2. Create an account** | Signs up or logs in | Too many fields, no progress indicator |
| **3. Orient to the dashboard** | Looks around, tries to understand the layout | No onboarding guide or tooltips — everything is unfamiliar |
| **4. Find "Create a Course"** | Looks for where to start | Button buried, label unclear, or hidden behind a role/permission |
| **5. Fill out course details** | Names the course, sets basic info | Form too long up front — asks for everything before the user is committed |
| **6. Publish or save draft** | Tries to move forward | No clear difference between "save" and "publish" — what happens next? |
| **7. See the course exist** | Lands on their new course page | If this moment doesn't feel like a win, they won't come back |

Mapping this flow shows developers exactly what empty states, tooltips, and confirmation moments need to be built — not as nice-to-haves, but as the difference between a user who gets it and one who bounces.

---

## A Personal Anecdote

My high school used a college prep portal that required Internet Explorer. The library ran IE — but most students accessed it from phones or Chrome laptops where the layout broke and key links didn't render.

Those students didn't miss the workshops because they weren't trying. They used what they had.

**Bad UX doesn't fail everyone equally. It fails the people with the least margin for error first.**

---

## Why UX at Cambio Labs Is Different

Most products are designed for users who can abandon a frustrating experience. At Cambio Labs:

- **No easy exit** — there's no competitor app for NYCHA housing resources
- **Trust is fragile** — one confusing flow confirms the platform wasn't built for them
- **Stakes are real** — missing a deadline or misreading eligibility has actual consequences

UX here isn't about delight. It's about dignity.