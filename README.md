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

## UX & Front-End: The Relationship

UX and front-end development are not the same thing — but they're the closest two roles in a product team. A UX designer decides *what* gets built and *why*. A front-end developer decides *how* it actually works in the browser.

**Where they overlap:**
- Component behavior and interaction states
- Accessibility (both are responsible for this)
- Performance — a slow page is a bad user experience
- Error states and empty states

**Where they diverge:**

| | Senior UX Designer | Full-Stack Developer |
|---|---|---|
| **Owns** | Research, wireframes, prototypes, user flows, design system | Architecture, APIs, database, implementation |
| **Doesn't own** | How it's built technically | Why design decisions were made |
| **Depends on each other for** | Designer needs dev to flag what's technically possible early; Dev needs designer to define edge cases before building |

The breakdown usually happens when both sides work in isolation — a designer hands off a Figma file without thinking about edge cases, or a developer builds without asking what happens when something goes wrong. The best teams close that gap early.

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

Since we won't have direct access to modify Journey itself, the output of this journey map wouldn't be changes to the codebase — it'd be a **separate companion web app**: a lightweight, step-by-step onboarding guide that runs alongside Journey and walks new users through the platform for the first time. Think of it like Notion's "learn the basics" portal, or how Loom has a dedicated getting-started experience separate from the product itself.

[Notion's learn the basics portal](https://academy.notion.com/page/essentials-catalogue?reg=1)
![Notion](./photos/notion.png)

[Loom's onboarding experience](https://support.atlassian.com/loom/)
![Loom](./photos/Loom.png)

The journey map is what tells us what that companion app needs to cover:

| Step | User Action | Potential Friction |
|---|---|---|
| **1. Land on the platform** | Arrives at the app for the first time | Unclear what Journey actually does — no context, no "start here" |
| **2. Create an account** | Signs up or logs in | Too many fields, no progress indicator |
| **3. Orient to the dashboard** | Looks around, tries to understand the layout | No onboarding guide or tooltips — everything is unfamiliar |
| **4. Find "Create a Course"** | Looks for where to start | Button buried, label unclear, or hidden behind a role/permission |
| **5. Fill out course details** | Names the course, sets basic info | Form too long up front — asks for everything before the user is committed |
| **6. Publish or save draft** | Tries to move forward | No clear difference between "save" and "publish" — what happens next? |
| **7. See the course exist** | Lands on their new course page | If this moment doesn't feel like a win, they won't come back |

Each friction point in the map becomes a screen or step in the companion app — guiding the user through exactly what to do without us needing to touch Journey's code at all.

---

## A Personal Anecdote

Filling out a W-9 on a government website for the first time felt like the site hadn't been updated in years — the PDF form didn't work properly on mobile, fields were confusing with no guidance, and when I made a mistake the "go back and edit" button didn't work. For someone filling it out for the first time with no tax background, something that should take 5 minutes turned into a frustrating experience that made you second-guess every answer.

**Bad UX doesn't fail everyone equally. It fails the people with the least margin for error first.**

---

## Why UX at Cambio Labs Is Different

Most products are designed for users who can abandon a frustrating experience. At Cambio Labs:

- **No easy exit** — there's no competitor app for NYCHA housing resources
- **Trust is fragile** — one confusing flow confirms the platform wasn't built for them
- **Stakes are real** — missing a deadline or misreading eligibility has actual consequences
- **The opportunity is real** — getting it right builds trust with communities that have historically been underserved by technology

UX here isn't about delight. It's about dignity.