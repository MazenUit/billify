# Build challenge: three parts, one story

This file might be the **only thing** in the repo we give you. That is enough. Everything you need to build is below.

You invent a **small product** with a clear story. You choose the name, the screens, the stack, and the folder names.

Think of it like a video game quest: **three stations, one adventure.**

---

stacks to use [server : laravel latest  - client: { nextj latest , tailwindcss latest , anstack/react-query latest , axios latest , framer-motion , goey-toast , zustand} - ollama : [typescript, cors, dotenv, express, ollama, pdf-parse , tesseract.js, xlsx, zod] ] note: this my personal choices not compulsory

rules of coding:
 1- never create readme file or text file or any comment or explain or any documentation until I ask for
 2- every code generated must be super simple , smartly scalable , easy to read , humanly , most dynamic and easy in logic implmenting 
 3- every new file should be less than 50 lines otherwise to break into smaller files 
 4- make sure any tech I ask for you to use it get the latest from online for better implmentation
## First steps — clone the workspace

Do this on your machine before anything else:

1. Clone the repo:
   ```bash
   git clone https://github.com/MazenUit/billify.git
   cd billify
   ```
2. Open the brief in your clone (whichever exists):
   - `docs/DEVELOPER_ASSESSMENT_CHALLENGE.md`, or  
   - `README.md` at the repo root if that is all you were given.
3. Build your solution in a **separate** place (new repo, or a clearly named folder/branch) unless you were told to commit inside this repo. Hand in the link or zip your **three parts** plus README there.

Repo link: [https://github.com/MazenUit/billify](https://github.com/MazenUit/billify)

---

## Step 0 — The three parts (the map)

Your submission must include **three separate runnable programs**. You can name the folders whatever you like. Conceptually they are:

| Part (concept) | In one sentence |
|----------------|-----------------|
| **Client** | What people click and type in the browser. |
| **Server** | Saves data, checks rules, talks to other services over HTTP. |
| **Bridge** | A small side service with “smart” HTTP endpoints (real LLM later, mock or rules today — both fine). |

Rule of thumb: **Browser → Server → Bridge.** The browser should not need a secret key to talk to an LLM directly (unless you document a very good reason).

---

## Step 1 — Pick your adventure (10 minutes)

Choose any story that fits this flow:

1. User gives you **a file or pasted text**.
2. Your app **pulls out structured fields** (real AI later is fine — fake data now is fine too).
3. Your app **builds something useful** from that (summary, quote, checklist, ticket… your call).
4. User can **chat** with something that explains what happened (simple rules for v1 are fine — still goes through your **bridge** the same way you would for a real model).

Give your app a **name** and one short paragraph in the README: *what problem does it solve?*

---

## Step 2 — Build the three stations (the real quest)

Ship **three runnable programs**:

1. Web app (React or Next.js — your pick).
2. API server (Laravel, Node, whatever you like — your pick).
3. Bridge service — small HTTP API your **server** calls (language your pick).  
   Mock brain is OK. **Real HTTP between server and bridge** is required.

---

## Step 3 — The happy path (must work end-to-end)

Check these off:

- [ ] Someone can’t use the app without a **simple gate** (pick one: login, API key, shared demo password — your call). Say in README what you chose and why.
- [ ] User uploads or pastes something → **saved in a database** → bridge returns JSON → **UI shows the result**.
- [ ] User sends a chat message → **assistant reply** comes back through the same bridge-style call (even if the “assistant” is `if (msg.includes("hi"))` for now).
- [ ] If the “AI” is fake, the UI says so somewhere friendly (“Demo brain ON” or similar).

Also save **at least two** tables/entities that make sense for your story (you name them).

---

## Step 4 — One “grown-up” touch (pick one, easy mode)

Pick **one**:

- [ ] `/health` on all three services, or  
- [ ] Logs on the API when it calls the bridge (start/end or ok/fail), or  
- [ ] A request id header: browser → API → bridge (so you can trace one click in logs)

---

## Step 5 — README (this is part of the grade)

Your README should answer, in plain language:

1. Copy-paste commands: how do I run all three parts locally?
2. Tiny diagram (boxes and arrows are perfect): what calls what?
3. Three honest lines: “v1 is rough because ___ — v2 I’d fix ___.”
4. One line: what you would **not** ship to real customers yet.

Optional fun: add a “known bugs I’m proud of” section.

---

## Bonus loot (pick any 2 if you have time)

- Usage meter (even fake numbers with real counters).
- Admin vs normal user for one button.
- File size / type checks with nice error text.
- Pagination somewhere.
- A few tests (any layer — surprise us).

---

## How we’ll cheer (scoring)

We’re rooting for:

- Can a stranger run it from README alone?
- Does the data model match the story you tell in the UI?
- When something breaks, does the user get a clue?
- Did you cut scope instead of shipping 10 half features?
- Git / PR story we can follow without detective work.

---

## Oops list (these hurt your score)

- No README run steps.
- Secrets in git.
- API keys only in the browser talking straight to the LLM (unless you wrote why).
- One 3,000-line file named `everything.ts`.
- Turning in someone else’s project with renamed variables.

---

## Timebox (pick one and write it at the top of README)

- Weekend sprint: mock brain + one happy path + README.
- One week: real DB + sad paths + one bonus.
- Two weeks: two bonuses + a little polish.

---

## What to turn in

One of: repo link · zip · PR.

Plus a **~2 minute** screen recording: gate → upload → see result → chat.

---

## Tiny reflection (answer any two in README if you want extra sparkle)

1. Where did you validate input — client, API, bridge — and why?
2. What breaks first if 100 teams used your app tomorrow?
3. If you charged for “AI,” what would you actually meter?

---

Ship small. Ship weird. Ship working. Have fun.


I need u demo from me you can ask ho the current system looks like 


don't forget :

1- after clone 
2- create ur own branch e.g: mazen-app-v1 
3- inside mazen-app-v1 [sever - client - ollama]
4- after done commit and push 


