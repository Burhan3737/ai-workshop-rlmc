# Facilitator Guide — "Your Co-Pilot, Not Your Pilot"

**AI as a tool for medical students · RLMC**
Duration: ~2 hr 40 min (incl. 10 min break) · Audience: 20–50 MBBS students, mixed years · Devices: phones + some laptops

> **The one sentence this workshop exists to deliver:**
> *You already use AI to get answers. The gap is using it to work with your own material, to examine you, and to build — with your hands on the controls the whole time.*

> **The through-line:** everything climbs one ladder — **write a better prompt → ground it in your own notes → make it test you → make it reusable → keep it honest → delegate whole tasks to an agent.** Each rung is more powerful than the last, and you stay the pilot at every step.

> **How to run this workshop:** there is a slide deck (`deck.html`) — put it on the projector — but **your screen is still the show.** You live-drive the real tools (Gemini, NotebookLM, Claude, Claude Code) and the students watch you do real things. This document is your private script: keep it open on a second screen or your phone, never mirrored. The **bold quoted lines are what you say out loud**; the `code blocks` are what you paste into the tool on screen.

> **You are not the medical expert — and the demos don't need you to be.** Levels 1 and 5 use a neutral, general topic you can run confidently (this guide uses **photosynthesis** for the prompt lesson). Levels 2, 3 and 4 use **a sample lecture on a neutral academic topic in your demo**, and in the **hands-on the students switch to their own real lecture notes** — that's where the medical content lives, supplied by the people who can actually judge it. The medical *framing* stays (it's why this matters to them); only the demo *content* is generic.

---

## Learning Outcomes

By the end of this workshop, students will be able to:

1. **Explain, in plain terms, how an AI language model works** — that it predicts the next word rather than "knowing" facts — and why that means its answers must be checked, not trusted blindly. *(Opening)*
2. **Write effective prompts** using a clear structure — Role · Context · Task · Format — to get useful, accurate responses. *(Level 1 — Prompt it)*
3. **Ground AI in their own study material** so answers are drawn from, and cited to, their real notes rather than the model's memory. *(Level 2 — Ground it)*
4. **Use AI to test themselves** on their own material through active recall, instead of only asking it for answers. *(Level 3 — Flip it)*
5. **Build a reusable AI "skill"** — custom instructions and a saved tutor — that supports them across the whole semester. *(Level 4 — Automate it)*
6. **Critically evaluate and verify AI output**, applying simple habits to catch errors before trusting anything — especially in a clinical context. *(Verify)*
7. **Describe what AI agents can do** — research, write, and build — and delegate a task to one while staying in control. *(Level 5 — Delegate it)*

> **The one-line version:** students leave able to use AI as a *co-pilot* for their studies — prompt it well, ground it in their notes, be tested by it, automate it, verify it, and delegate to it — without ever handing over the controls.

---

## PART 1 — PREP

### A. Accounts you need (all free unless noted)

| Tool | Link | Why | Your account |
|---|---|---|---|
| **Gemini** | gemini.google.com | L1 prompting, L3 quiz, L4 Gems | Free Google account |
| **NotebookLM** | notebooklm.google.com | L2 — grounded answers with citations | Free Google account |
| **Gemini app (mobile)** | iOS/Android store | optional voice "quiz me" | Same account |
| **Claude** | claude.ai | L5 free build (Artifacts), comparison | Free tier fine |
| **Claude Code** | claude.com/product/claude-code | **L5 agent + build demo — yours only, paid** | Your existing plan |
| ChatGPT | chatgpt.com | Optional comparison only | Free |

### B. Free-tier limits — memorise these, students will ask

| Tool | Free limit that matters | Consequence for the room |
|---|---|---|
| NotebookLM | 50 sources/notebook · 50 chats/day · ~3–5 audio overviews/day · Discover sources + URL + YouTube as inputs | Generous. Safe for hands-on. |
| Gemini | ~30 prompts/day · Gems unlimited (10 files each) · Live voice free on mobile | Safe, but tell them to spend prompts wisely |
| Claude | Artifacts free · Projects (5 max) · 20 files/chat · budget resets ~every 5 hrs | Safe. **No Claude Code / agents on free.** |
| **ChatGPT** | **3 file uploads per day** · agent mode is **paid** | Don't route file hands-on here. Agents aren't free. |

> **Rule for the day:** every single thing you ask a student to *do* must work on a free account. Paid tools (Claude Code, agents) appear only as *"here's the ceiling"* demos — clearly labelled, never followed along.

### C. Files to prepare (night before) — your demo set only

*All on one neutral academic topic you're comfortable with. Students bring their own real course material for the hands-on parts; you don't need any of it.*

1. **A sample lecture on photosynthesis** — a slide or short PDF. It carries straight over from the Level 1 prompt example, so your whole demo runs on one topic the room can follow. *(L2 grounding demo + L3 quiz demo + L4 Gem demo — this stands in for "your lecture". Swap for another school-level topic — the water cycle, the solar system — if you prefer.)*
   - *Easiest source:* in NotebookLM just click **Discover sources**, type "photosynthesis", and add what it finds — no file needed. Or paste a Wikipedia URL / YouTube link.
2. **A photo of any diagram or figure** you can talk about (a graph, a labelled diagram). *(Optional multimodal moment in L2/L4.)*

That's it. L1 is typed live; L5 is built live.

### D. Recordings to capture (night before) — NON-NEGOTIABLE

Wifi in a lecture hall is not a dependency you bet a workshop on. Screen-record every demo below and keep them in one folder, numbered.

- [ ] `01` — NotebookLM cited answer + a citation click (L2)
- [ ] `02` — NotebookLM Audio Overview playing (L2)
- [ ] `03` — the "quiz me" exchange (L3)
- [ ] `04` — a Gem / "Study Coach" being built and used (L4)
- [ ] `05` — **the end-to-end finale: the agent researching, then building the presentation, start to finish** (L5)

`05` is the most important recording you'll make. If the finale fails live, the closing moment fails with it.

### E. Room setup

- [ ] Laptop + HDMI tested, screen mirroring confirmed
- [ ] **Speakers tested and loud** — two demos are audio (Audio Overview, and narrating the agent build)
- [ ] `deck.html` open full-screen on the projector; arrow keys advance it
- [ ] Recordings folder open in a second window (your fallback if wifi dies)
- [ ] This guide open on a **second screen or your phone** — never mirrored to the projector
- [ ] Browser zoom bumped to ~125% so the back row can read what you type
- [ ] Each tool open in its own tab, in running order: Gemini → NotebookLM → Claude → Claude Code
- [ ] Browser: log into all accounts **before** students arrive, close every unrelated tab
- [ ] *(Optional)* phone mirroring ready if you want to show voice "quiz me"

---

## PART 2 — RUN SHEET

> Bold quoted lines = **what you say**. Code blocks = **what you paste**.

### `00:00–00:12` — OPENING: the honest start + how it actually works

**Two open questions. Take a few answers out loud — don't correct anyone.**

> "Before I show you anything — in your own words, what actually *is* AI?"
> *(take 3–4 answers — "a robot", "a computer brain", "ChatGPT", "it knows everything" — collect them, don't judge)*
> "And how do you actually use it, day to day?"
> *(assignments, summaries, "explain this topic" — that's the baseline you're about to widen)*

> "Hold those answers. In ten minutes you'll know which of you were right."

**Your story — this is what buys you the room:**

> "I'm a software engineer. As a student I used AI to finish assignments. That's all. I found out later I was using maybe 5% of it. Before I show you the rest — a quick game, because you can't use this thing well until you know what it actually is."

**The next-word game (no tools, no wifi — runs on the room). Don't say the answer — cut the stem off and let the room shout it.**

*Round 1 — the obvious one (everyone lands on the same word):*
> "Salt and…"

*Round 2 — a fork (different people, different words):*
> "I walked into the kitchen and picked up the…" *(kettle, cup, knife, phone, spoon)*

*Round 3 — build a whole sentence, one word each:*
> "This morning, on my way here, I…"
> Now **point at person after person around the room** — each adds **only the next word.** A full sentence appears out of nowhere, one word at a time. Let it run a good 6–8 people; the longer it goes, the better it lands.

> "That's the reveal. Nobody planned that sentence — each of you just added the most likely next word. **That is exactly what an AI does** — it read most of the internet and learned, given the words so far, what word probably comes next. Then it does it again, one word at a time, faster than you can read. There's no fact-box inside it — it's the most powerful autocomplete ever built."

**Land the two consequences:**

> "That's why *how you phrase things* changes everything — you're giving it better words to predict from. And it's why it can be **confidently, beautifully wrong** — a plausible answer and a true answer look identical to it. Hold that thought; we come back to it."

> "So here's the deal for today: **AI is your co-pilot, not your pilot.** You stay in the driver's seat the whole time. We're going to climb five levels of doing exactly that."

**Show the roadmap slide.** `PROMPT IT → GROUND IT → FLIP IT → AUTOMATE IT → (VERIFY) → DELEGATE IT`

---

### `00:12–00:27` — LEVEL 1: PROMPT IT

> **It only flies as well as you steer it. Level one is learning to give it a good instruction.**

**The bad prompt — type it live, let the vague wall of text land:**

```
what is photosynthesis
```

> "Technically correct. Totally useless — a wall of text, because I gave it nothing to aim at."

**The good prompt — same topic, four things added:**

```
You are a biology tutor (ROLE).
I'm revising for an exam and keep mixing up the light and dark
reactions of photosynthesis (CONTEXT).
Explain it in 5 simple steps with one everyday analogy, then ask
me 3 questions to test myself (TASK).
Keep it under 200 words, no jargon (FORMAT).
```

> "Same model, same topic. The only thing that changed is I told it **who to be, what I need, what to do, and what shape to hand back.** That's the whole skill."

**The takeaway — put it on screen, tell them to photograph it:**

```
A good prompt has four parts:
ROLE    — who it should be       ("you are a tutor…")
CONTEXT — your situation         ("I'm revising and I keep mixing up…")
TASK    — what to actually do    ("explain, then quiz me")
FORMAT  — the shape to hand back ("5 steps, under 200 words, no jargon")
```

**HANDS-ON (5 min).** Everyone takes a lazy prompt about something they're studying and rewrites it with all four parts. *Walk the room.*

---

### `00:27–00:55` — LEVEL 2: GROUND IT

> **Stop asking what it remembers. Make it read what you gave it. This is where it becomes *your* co-pilot.**

**Go to:** notebooklm.google.com

**Demo 1 — feed it real material (5 min).** Add your photosynthesis lecture — fastest is NotebookLM's **Discover sources → "photosynthesis"**, or upload a slide. Then ask:

```
You are my study tutor (ROLE). Using only the sources I gave you
(CONTEXT), write a one-page high-yield summary of this lecture (TASK).
Cite the slide or page number for every point (FORMAT).
```

Click a citation. It jumps to the exact spot. **Say the line:**
> "It's not remembering. It's reading your material — and showing you where it got every line. That's the difference between a co-pilot and a party trick."

**Demo 2 — Audio Overview (7 min).** Generate it, then **play it out loud**:

```
You're briefing a student revising for an exam (ROLE). Focus on
this lecture (CONTEXT). Cover the points most likely to be tested
(TASK), kept simple and high-yield (FORMAT).
```

> "Two AI hosts discussing your own lecture. That's your commute. That's the queue at the canteen. Your lecture deck is now a podcast."

**HANDS-ON (10 min).** Everyone opens notebooklm.google.com and adds **one of their own real lectures** — this is where the medical content comes in, theirs not yours (upload a PDF, paste a slide's text, or use Discover sources). Ask one question, click a citation, hit **Generate Audio Overview**.
*Walk the room. Expect: file too large, wrong Google account. Nobody stuck more than 2 min — pair them up.*

**Fallback:** recordings `01`, `02`.

---

### `00:55–01:13` — LEVEL 3: FLIP IT

> **It shouldn't just answer your questions. It should ask you questions. This is the single best way to actually learn.**

**Demo — the examiner (8 min).** Keep the same lecture material in play (Gemini with the slide attached, or your NotebookLM notebook):

```
You are a tough examiner (ROLE). Examine me on this lecture (CONTEXT).
Ask one question at a time, wait for my answer, never give it to me,
and probe deeper if I'm vague (TASK). After 8 questions, score me out
of 10 and name the two things to revise tonight (FORMAT).
```

Answer a couple wrong on purpose — the probing is the wow. **Then the meta-punchline:**
> "Notice what just happened — it *tested* me instead of *telling* me. Testing yourself is the single best-evidenced way to make something stick. You just learned the technique by having it done to you."

**Point at the labels in the prompt:**
> "And look at what that examiner actually is — a good prompt. Role, Context, Task, Format — the exact four parts from Level 1, reused. That's the whole trick."

*(Optional voice: run the same thing through Gemini Live on your phone — "quiz me out loud" — for hands-free revision.)*

*(One-click, grounded alternative: **NotebookLM → Studio → Quiz** generates a quiz straight from the lecture uploaded in Level 2 — exactly like the Audio Overview, no prompt needed. Use the Gemini prompt above to teach that "the examiner is just a good prompt"; point students to NotebookLM's Quiz for the fastest hands-on.)*

**HANDS-ON (5 min).** Everyone, on their own: run a **3-minute quiz** on a topic from your own course — either type "quiz me" in **Gemini**, or (easiest, and grounded) open the lecture you uploaded in Level 2 and hit **NotebookLM → Studio → Quiz** to generate one straight from your own material. See how hard it pushes.

**Fallback:** recording `03`.

---

### `01:13–01:23` — BREAK

Ten minutes. Walk the room, answer questions, and find out what people are studying — you'll fold real examples into Verify and the finale.

---

### `01:23–01:45` — LEVEL 4: AUTOMATE IT

> **If you set it up once and use it all semester, you never rebuild it. This is what people mean by giving AI a "skill."**

**Move 1 — custom instructions (5 min).** *Everyone does this — two minutes, improves every chat they have for the rest of the year.*

Claude → Settings → Profile · Gemini → Settings → Saved info · ChatGPT → Settings → Personalization

```
I'm a university student preparing for exams (CONTEXT).
Act as my study tutor (ROLE).

When you answer: explain in clear simple steps, tell me your
confidence, and flag anything I should double-check or that's
region-specific (TASK).
Structure every answer as: definition → key points → example →
common mistakes (FORMAT).
```

> "You write that once. It applies to every conversation from now on. Most people never open this screen."

> *To the room:* "In the hands-on you write your own — a medic would add: 'use drug names as used in Pakistan, structure answers viva-style, never give a dose without a source.' That's your content; you know what belongs there, I don't."

**Move 2 — build a reusable "skill" (12 min).** Use **Gemini Gems** (free, unlimited) — gemini.google.com → *Gems* → *New Gem*. Load your sample lecture into it.

Name: `Study Coach`

```
You are my study tutor (ROLE). My lecture notes are in your files
(CONTEXT). Teach from my material and end every answer with one
follow-up question to check I understood (TASK).
If I say "QUIZ ME", examine me instead: one question at a time, no
answers, 8 questions, then score me (FORMAT).
```

Use it, then **close it and reopen it** — show that it remembered everything.

> "That's a tutor that knows your material and your exam format, and it's still there in March. **This — a saved, reusable assistant you build once — is what people mean by giving an AI a 'skill'.** You'll hear about 'custom GPTs' and 'Claude Skills'; same idea, but creating those needs a paid plan. Gemini Gems does it for free. So this is the one you build tonight."

**Point at the labels in the prompt:**
> "And notice — the skill is just a good prompt you saved. Role, Context, Task, Format — the same four parts from Level 1. You already know how to write these."

*Mention only:* Claude Projects does the same (free, 5 projects). Claude Skills and custom GPTs are **paid to create**.

**HANDS-ON (5 min).** Everyone does **both**: (1) set your custom instructions — with your own subject and exam; (2) build one Gem loaded with your own lecture.

**Fallback:** recording `04`.

---

### `01:45–02:03` — VERIFY: HANDS ON THE CONTROLS

> **Co-pilot, not pilot. Everything above makes AI powerful. This is how you stay the one in charge. It matters most in your profession.**

**Callback to the game:**
> "Remember — it predicts the next likely word. It doesn't *know* things. So when it doesn't have a fact, it predicts what a plausible one looks like — confidently. A true answer and a made-up one look identical to it. In your field, a confident wrong answer isn't a typo — it's a patient."

**The three ways it will burn you:**

1. **Outdated information** — training has a cutoff; facts, prices, guidelines all move.
2. **Invented details** — it makes up specific facts, numbers and quotes that sound exactly right.
3. **Context mismatch** — advice written for another country, system or year. *For medics: US/UK guidance ≠ Pakistani practice, local drug availability, resistance patterns — you've never thought about it.*

**So how do you stay in charge? Four habits (8 min) — put them on screen, tell the room to photograph them:**

```
1. "Cite it, or tell me you can't."
2. "What would change this answer?"
3. "What's the strongest argument against what you just told me?"
4. "Which fact here is most likely to be out of date?"
```

Plus the hard rule: **never accept a number — a dose, a date, a statistic — without a source you can open.**

> "Use it to *get examined*, not to get finished. Your viva is oral, in person, in front of a consultant who asks the follow-up. If the AI learned it and you didn't, you find that out in the worst possible room."

---

### `02:03–02:28` — LEVEL 5: DELEGATE IT — AI THAT DOESN'T JUST ANSWER, IT DOES

> **Everything so far, you drove — you prompted, you asked. An agent takes a goal and does the work itself, step by step. This is the frontier.**

*This is a demo you drive. Real agents are the paid/advanced tier — but they show students where all of this is going, and the free build tools let them try the idea tonight.*

**The end-to-end finale — one goal, done live (18 min).** This single prompt pulls together *everything from today* — a good prompt (Role·Context·Task·Format), grounded in real, cited sources, producing a finished thing you keep. In **Claude Code**:

```
You are my research assistant and presentation designer (ROLE).
I'm a medical student who wants an evidence-based guide to studying
smarter for exams (CONTEXT).
Research the study techniques proven to work — active recall, spaced
repetition, interleaving — from credible sources and cite them, then
turn it into a clean slide presentation (TASK).
Make it a single self-contained HTML deck: 6–8 slides, one idea each,
a sources slide at the end, works offline (FORMAT).
```

Narrate as it works — this is the whole workshop in one run: *"Watch what it's doing: first it researches, finds and cites real sources, then it designs and writes an entire presentation — one step at a time, and I approve each one. I'm not doing any of it."* When it finishes, **open the presentation on screen.** Wait for the noise — they're watching an AI build a presentation, live, *during* a presentation.

> "That's an agent. One prompt — a good prompt, grounded in sources — and it did the whole job end to end: research to finished deck, showing me every step. That is where all five levels have been heading. And even here, at full power, you stay in charge — you approve each move."

**The honest bridge — do not skip:**

> "Claude Code is the paid tool I use for real work. But the *idea* — describe what you want and get it built — is free tonight: **Claude Artifacts, Gemini Canvas.** You've now seen the whole ladder: prompt it well, ground it in real sources, make it reusable, keep your hands on the controls, and hand the whole job to an agent."

**Fallback:** recording `05` (the end-to-end run). **Never skip the finale — play the recording instead.**

---

### `02:28–02:38` — CLOSE

**Everyday wins — quick-fire (3 min), so it's not just for studying:**

> "Beyond studying, this saves you time every day." Draft a polite email to a professor · summarise a 20-page PDF into 10 points · build a study timetable around your exam dates.

**Land it:**

> "Five levels. Prompt it well. Ground it in your own material. Flip it so it examines you. Automate it so you build it once. Verify it, always, because it's medicine. And delegate it — where it's all going.
>
> One thing if you take nothing else: **stop asking it for answers, start asking it to test you.** The exam room doesn't care what the AI knows. It cares what you know.
>
> **AI is your co-pilot. Not your pilot.**"

**The takeaway — no handout.** Tell them plainly:

> "I'm dropping every prompt from today in your class WhatsApp group tonight. Two things before you sleep: set your custom instructions, and have AI quiz you on whatever you're studying this week."

Leave the **four habits** on screen long enough for the room to photograph them.

---

## PART 3 — CONTINGENCIES

| If this happens | Do this |
|---|---|
| **Wifi dies** | Switch to the recordings folder. "This is why you always have a backup — true for your presentations too." Turn it into a point. |
| **A demo produces a boring answer** | Say so out loud. "That's a weak answer — watch what happens when I give it more to work with." Recovering visibly builds *more* trust than a clean run. |
| **A student's clinical prompt gets refused** | Reframe as education: "I'm a medical student practising for an exam." It can happen with dose/diagnosis prompts in the hands-on. |
| **Hands-on stalls the room** | Hands-on is time-boxed. Announce the time, then move on regardless. Don't let 5 stuck people hold 45. |
| **The agent/build runs long or errors** | Keep it small — one clean feature. If it breaks live, switch to recording `07`. Never let the finale die on screen. |
| **Someone challenges you on cheating** | Don't get defensive. "Fair. That's exactly why Verify exists, and why I told you what I did as a student." |
| **Someone asks a deep clinical question** | "You're the doctor in this room, not me." Genuine, and it lands well. |
| **Running late** | Cut in this order: L3 hands-on → L4 hands-on → Demo 1 of L5 (research). **Never cut the build finale.** |
| **Running early** | Take questions on their actual subjects and demo live. Best possible use of spare time. |

---

## PART 4 — THE NIGHT-BEFORE CHECKLIST

- [ ] Sample lecture ready (or Discover-sources topic chosen) for L2/L3/L4
- [ ] NotebookLM tested on it — cited answer + Audio Overview pre-generated (it takes minutes — don't generate live)
- [ ] All 5 recordings captured and in one folder
- [ ] Gem "Study Coach" built once as a rehearsal, then deleted so you can build it live
- [ ] Claude Code finale run once end-to-end — know how long the build actually takes
- [ ] `deck.html` tested full-screen on the projector; arrow keys advance
- [ ] Speakers tested at hall volume
- [ ] This guide open on your second screen / phone (NOT projected)
- [ ] Class WhatsApp group link handy, to drop the prompts at the end
- [ ] Every account logged in, unrelated tabs closed, notifications off
