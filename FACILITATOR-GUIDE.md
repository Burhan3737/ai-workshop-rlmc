# Facilitator Guide — "Stop Asking. Start Building."

**AI as a tool for medical students · RLMC**
Duration: 2 hr 50 min (incl. 10 min break) · Audience: 20–50 MBBS students, mixed years · Devices: phones + some laptops

> **The one sentence this workshop exists to deliver:**
> *You already use AI to get answers. Almost nobody in this room uses it to be examined, to be grounded in their own material, or to build something. That's the gap.*

> **How to run this workshop:** there is no slide deck. **Your screen is the show.** You live-drive the actual tools — NotebookLM, Gemini, Claude, Claude Code — and the students watch you do real things, not slides about them. This document is your private script: keep it open on a second screen, your phone, or a printout. Nothing in here is meant to be projected. Part 2 is a minute-by-minute run sheet; the **bold quoted lines are what you say out loud**, the `code blocks` are what you paste into the tool on screen.

---

## PART 1 — PREP

### A. Accounts you need (all free unless noted)

| Tool | Link | Why | Your account |
|---|---|---|---|
| **NotebookLM** | notebooklm.google.com | Mode 1 — grounded answers with citations | Free Google account |
| **Gemini** | gemini.google.com | Mode 2 voice, Mode 3 Gems | Free Google account |
| **Gemini app (mobile)** | iOS/Android store | Gemini Live voice demo | Same account |
| **Claude** | claude.ai | Mode 3 Projects, Mode 4, free Artifacts | Free tier fine |
| **Claude Code** | claude.com/product/claude-code | **Finale — yours only, paid** | Your existing plan |
| ChatGPT | chatgpt.com | Optional comparison only | Free |

### B. Free-tier limits — memorise these, students will ask

| Tool | Free limit that matters | Consequence for the room |
|---|---|---|
| NotebookLM | 50 sources/notebook · 100 notebooks · 50 chats/day · ~3–5 audio overviews/day | Generous. Safe for hands-on. |
| Gemini | ~30 prompts/day · Gems unlimited (10 files each) · Live voice free on mobile | Safe, but tell them to spend prompts wisely |
| Claude | Projects (5 max) · Artifacts · 20 files/chat · budget resets ~every 5 hrs | Safe. **No Claude Code on free.** |
| **ChatGPT** | **3 file uploads per day** · voice = short daily preview | **Do NOT route file or voice hands-on here.** This is the trap. |
| Gemini Scheduled Actions | **Paid** (AI Plus ~$4.99/mo) | Mention only. Never ask them to follow along. |

> **Rule for the day:** every single thing you ask a student to *do* must work on a free account. Paid tools appear only as *"here's the ceiling"* — clearly labelled, never followed along.

### C. Files to prepare (night before)

1. **One real lecture PDF** — pharmacology or physiology works best, 40+ slides. Ideally an actual RLMC deck.
2. **One past paper** for the same subject.
3. **One textbook chapter** PDF, same topic.
   *These three become the NotebookLM notebook. Load them the night before, not live.*
4. **A photo of handwritten notes** on your phone (messy is better — it's more impressive).
5. **A printed/photo ECG or a histology slide image.**

### D. Recordings to capture (night before) — NON-NEGOTIABLE

Wifi in a lecture hall is not a dependency you bet a workshop on. Screen-record every demo below and keep them in one folder on your laptop, named 01–08.

- [ ] `01` — the broken demo (opening)
- [ ] `02` — NotebookLM cited answer
- [ ] `03` — NotebookLM Audio Overview playing
- [ ] `04` — viva examiner exchange
- [ ] `05` — Gemini Live simulated patient
- [ ] `06` — Gem being built + used
- [ ] `07` — fake citation being caught
- [ ] `08` — **Claude Code building the app, start to finish**

`08` is the most important recording you will make. If the finale fails live, the workshop's closing moment fails with it.

### E. The opening "broken demo" — capture this in advance

**You cannot rely on a model failing on cue.** Fish for a good failure the night before, screenshot it, and present the screenshot.

What reliably breaks — try these with web search **off**:

```
List 5 peer-reviewed papers, with DOIs, on [narrow local topic].
```

```
What does the Pakistani national guideline (2024) recommend as
first-line management for [condition]? Quote the exact protocol.
```

Then check the DOIs at doi.org. Screenshot one that resolves to nothing. **That screenshot is your opening.**

### F. Room setup

- [ ] Laptop + HDMI tested, screen mirroring confirmed
- [ ] **Speakers tested and loud** — two demos are audio (Audio Overview, Gemini Live)
- [ ] Phone screen-mirroring working (for the Gemini Live patient demo) — or hold the phone to a mic
- [ ] Recordings folder open in a second window (your fallback if wifi dies)
- [ ] This guide open on a **second screen or your phone** — never mirrored to the projector
- [ ] Browser zoom bumped to ~125% so the back row can read what you type
- [ ] Each tool open in its own tab, in running order: NotebookLM → Gemini → Claude → Claude Code
- [ ] Browser: log into all accounts **before** students arrive, close every unrelated tab
- [ ] Phone on Do Not Disturb if mirroring it

---

## PART 2 — RUN SHEET

### `00:00–00:10` — OPENING: the honest start

**Start with them, not you. Two open questions first — just let them shout answers. This warms the room and hands you the setup for everything that follows.**

**Question 1 — "What is AI?" (2 min).** Take 3–4 answers. Do not correct a single one:

> "Before I show you anything — what actually *is* this thing? If you had to say what AI is, in your own words, what would you say?"

*You'll hear: "a robot", "a computer brain", "ChatGPT", "it knows everything", "the future".* Don't judge, don't correct — just collect them.

> "Hold onto your answer. In ten minutes you'll know exactly which of you were right."

**Question 2 — "How do you actually use it?" (2 min).** Honest answers, no judgement:

> "And right now — how do you actually use it, day to day? Be honest, I'm not marking you."

*You'll hear: assignments, summaries, "explain this topic", making notes.* This is the baseline you're about to expand.

**Now the poll — sharpen the gap. Do not skip it; the whole workshop hangs off the gap it reveals.**

> "Hands up if you've used AI this week."
> *(every hand goes up — wait for it)*
> "Keep it up if you used it for something that wasn't an assignment, a summary, or 'explain this topic to me.'"
> *(almost every hand drops — let the silence sit for a beat)*
> "That's it. That's why we're here."

**Then own your own story.** This is what buys you the room:

> "I'm a software engineer. When I was a student I used AI to finish assignments. That's it. That's all I used it for. I'm not here to lecture you about that — I'm here because I found out afterwards that I was using maybe 5% of it."

> "But before I show you the 5%, we're going to play a game — because you can't use this thing well until you know what it actually is. And almost nobody does."

---

### `00:10–00:20` — HOW IT ACTUALLY WORKS: the next-word game

> **The whole point: an LLM is not a brain and not a search engine. It is a machine that predicts the next word. That's it. Everything else — the genius and the danger — falls out of that one fact.**

*No tools, no wifi, no screen needed. This runs entirely on the room. If the internet is down when you start, start here anyway.*

**Round 1 — the obvious one (2 min).** Say the stem, cut yourself off, and let the room shout the next word:

> "The patient presented with chest…"

The room shouts **"PAIN."** Do two or three more:

> "History of presenting…" → *complaint*
> "Blood… " → *pressure*
> "Wash your…" → *hands*

**Say the line:**
> "Notice you all said the same word. Nobody looked anything up. You just knew what usually comes next. Hold onto that — you just did exactly what the AI does."

**Round 2 — the fork (3 min).** Now a stem with more than one good answer:

> "The doctor picked up the…"

You'll hear *stethoscope, phone, pen, chart, scalpel.* **Say the line:**
> "See what happened? It's not one answer — it's a spread of likely ones, each with a probability. The AI keeps a list exactly like that, then picks one. Change which one it picks and you get a slightly different sentence every time. That's why it never answers the same way twice."

**Round 3 — the reveal (4 min).** Call back to their "What is AI?" answers from the top, then land what they just proved:

> "At the start I asked what AI is. Some of you said a robot, a brain, something that knows everything. Here's the honest answer: it's none of those. That is *all* a large language model does — it read basically the whole internet, every textbook, every paper, every forum, and all it learned was: given the words so far, what word probably comes next. Then it does that again. And again. One word at a time, faster than you can read. There is no fact-box inside it. No library it looks things up in. It's the most powerful autocomplete ever built."

**Then the trap that makes the rest of the day matter (3 min):**

> "So watch what happens when I ask it for a reference. It has never seen your exact paper — but it has seen *thousands* of references. So it predicts what a reference should *look like*: a plausible author, a real-sounding journal, a DOI in the right format. It's not lying to you. It literally cannot tell the difference between a real citation and a citation-shaped sentence. It's just finishing the pattern."

**Now the broken demo — the payoff.** Show screenshot `01`:

> "Here it is doing exactly that. Confident. Well-formatted. Completely fabricated — including the citations. And now you know *why*: you can't ask a next-word-predictor for the truth. You can only make it more likely to land on it — and that's the whole rest of this workshop."

> "In your field, a confident wrong answer isn't a typo. It's a patient. So everything I show you now is really about one thing: how to steer this thing toward true, and how to catch it when it isn't."

**Frame the session.** Four shifts, then we build something.

`GROUND IT → FLIP IT → AUTOMATE IT → VERIFY IT → BUILD IT`

---

### `00:20–00:50` — MODE 1: GROUND IT

> **Stop asking what it remembers. Make it read what you gave it.**

**Go to:** notebooklm.google.com (notebook pre-loaded from prep step C)

**Demo 1 — the citation (5 min).** Ask your notebook:

```
Using only my sources, give me a one-page high-yield summary of
[topic] for a viva. Cite the slide or page number for every claim.
```

Click a citation. It jumps to the exact slide. **Say the line:**
> "It's not remembering. It's reading. And it's showing you where it got it."

**Demo 2 — the refusal (3 min).** Ask something deliberately outside the sources.

```
What does my lecture say about [something not in the deck]?
```

It says it isn't in your sources. **Say the line:**
> "It just said 'I don't know.' Your chatbot almost never does that. That's the whole difference."

**Demo 3 — the gap analysis (5 min).** This is the one they'll actually use tonight:

```
Compare my lecture slides against the past paper. What has been
asked in exams that my lectures do NOT cover? List it as a
revision checklist.
```

**Demo 4 — Audio Overview (7 min).** Generate it, then **play it out loud.** Customise first:

```
Focus on [topic]. Explain at the level of an MBBS student
preparing for a viva. Emphasise the points most likely to be asked.
```

> "That's your commute. That's the queue at the canteen. Your pharmacology deck is now a podcast."

**HANDS-ON (10 min).** Everyone opens notebooklm.google.com, uploads one lecture PDF, asks one question, hits Generate Audio Overview.
*Walk the room. Expect: file too large, wrong Google account, unsupported format. Nobody is stuck for more than 2 min — pair them up.*

**Fallback:** recordings `02`, `03`.

---

### `00:50–01:20` — MODE 2: FLIP IT

> **It shouldn't answer your questions. It should ask you questions.**

**Demo 1 — the viva examiner (10 min). Get a volunteer on the mic.**

Paste into Claude or Gemini:

```
You are an FCPS Part 1 viva examiner. Examine me on [topic].

Rules:
- Ask ONE question at a time, then wait for my answer.
- Never give me the answer.
- If I'm vague or wrong, probe deeper the way a real examiner does.
- Escalate difficulty as I do well.

After 8 questions, stop and give me: my score out of 10, the two
gaps that would have failed me, and exactly what to revise tonight.
```

Let the volunteer squirm a little. It's more memorable than a smooth run.

**Demo 2 — the simulated patient (12 min). THE MOMENT OF THE WORKSHOP.**

Open **Gemini Live on your phone** (mirrored/held to mic). Voice mode, speak this:

```
You are a patient in an outpatient clinic. You have [hidden
diagnosis]. Stay in character at all times — never break character,
never explain anything medically.

Answer only what I actually ask, the way a real, slightly anxious
patient would: vague, sometimes off-topic. Do not volunteer key
symptoms unless I ask a good question.

I am the medical student taking your history. Begin when I greet you.

When I say "END", drop character and tell me: what I missed, what
questions I should have asked, and how my communication came across.
```

Bring a **clinical-year student** up to take the history out loud. Let it run 4–5 min. Then say **END** and read the debrief to the room.

> "You can do that every night. For free. Unlimited patients, unlimited attempts, and it never gets tired of you."

**Demo 3 — the Feynman check (5 min).**

```
I'm going to explain [topic] to you as if you're the examiner.
Don't correct me while I talk. When I finish, tell me: which parts
I actually understood, which parts I was reciting without
understanding, and the one question an examiner would ask to
expose the gap.
```

> "That last one is the difference between passing and being caught out."

**HANDS-ON (5 min).** Pairs. One person runs a 3-min viva on their current block.

**Fallback:** recordings `04`, `05`.

---

### `01:20–01:30` — BREAK

Leave the last Mode 2 result up on screen. Walk the room, answer questions, and — most important — find out what block people are in and what they're stuck on, so you can pick the finale build target during the break.

---

### `01:30–02:00` — MODE 3: AUTOMATE IT

> **My engineer's lens: if you type the same instructions twice, you've already lost.**

**Demo 1 — memory / custom instructions (7 min).** *Everyone does this one, it takes 2 minutes and improves every conversation they have for the rest of the year.*

Claude → Settings → Profile · Gemini → Settings → Saved info · ChatGPT → Settings → Personalization

```
I'm a [3rd] year MBBS student at Rashid Latif Medical College,
Lahore, Pakistan, preparing for [university professionals / FCPS].

When I ask a clinical question:
- Use terminology and drug names as used in Pakistan.
- Flag when a guideline is US/UK-specific and may differ locally.
- Structure answers viva-style: definition → causes → presentation
  → investigation → management.
- Tell me your confidence, and what I must verify in a textbook.
- Never give me a dose without telling me where it came from.
```

> "You write that once. It applies to every conversation you have from now on. Most people never open this screen."

**Demo 2 — a saved assistant, built live (12 min).** Use **Gemini Gems** (free, unlimited, 10 files each) — gemini.google.com → *Gems* → *New Gem*.

Name: `Block Tutor — [current block]`

```
You are my tutor for the [X] block of MBBS at RLMC. My syllabus and
lecture material are in your files.

Always:
- Answer only from my uploaded material where possible; say clearly
  when you're going beyond it.
- Answer in viva structure and use Pakistani clinical context.
- End every answer with one follow-up question to test whether I
  actually understood it.

If I say "QUIZ ME", stop teaching and examine me instead: one
question at a time, no answers given, 8 questions, then score me.
```

Upload the syllabus. Use it. **Then close it and reopen it** — show that it remembered everything.

> "That's a tutor that knows your syllabus, your exam format and your country, and it's still there in March."

*Mention only:* Claude Projects does the same thing (free, 5 projects). Scheduled recurring quizzes exist but are **paid** — don't follow along.

**Demo 3 — your phone camera is an input (5 min).** Photograph your messiest handwritten notes:

```
Convert these handwritten notes into clean structured notes.
Flag anything you couldn't read clearly rather than guessing it.
```

Then the ECG/histology image:

```
Walk me through reading this systematically, step by step, the way
I'd be expected to present it in an OSCE. Don't just give me the
diagnosis — teach me the method.
```

> "Note what I asked for. Not the answer — the *method*. Ask for the answer and you learn nothing."

**HANDS-ON (6 min).** Set custom instructions (everyone), then build one Gem if there's time.

**Fallback:** recording `06`.

---

### `02:00–02:20` — MODE 4: VERIFY IT

> **How not to get burned. This is the part that matters most in your profession.**

**The three failure modes that matter in medicine:**

1. **Outdated guidelines** — training data has a cutoff; guidelines move.
2. **Fabricated citations** — papers that do not exist, with real-looking DOIs.
3. **Region mismatch** — US/UK guidance ≠ Pakistani practice, local drug availability, or local resistance patterns. *This one will bite them and they've never thought about it.*

**Demo — catch a fake citation live (7 min).** Show screenshot `07`, or run it live:

```
Give me 5 peer-reviewed references supporting [claim], with DOIs.
```

Take one DOI → doi.org → nothing. Or Google Scholar → no such paper.

> "Remember the game at the start? This is Round 3, live. It's not looking up a paper — it's predicting what a paper should look like. That paper does not exist. If it goes in your research project, it's your name on it, not the AI's."

**The four habits (8 min)** — type these into whatever tool is on screen, big, and tell the room to photograph it. This is the one thing worth them having in their camera roll:

```
1. "Cite it, or tell me you can't."
2. "What would change this answer?"
3. "What's the strongest argument against what you just told me?"
4. "Which fact here is most likely to be out of date?"
```

Plus the hard rule: **never accept a number — a dose, a cutoff, a lab value — without a source you can open.**

**Ethics, 3 minutes, no sermon (5 min).** Be blunt and be honest:

> "I'm not going to tell you not to use it for assignments. I did. But your vivas are oral, in person, in front of a consultant who will ask you the follow-up question. If the AI learned it and you didn't, you find that out in the worst possible room. Use it to *get examined*, not to get finished."

---

### `02:20–02:45` — FINALE: BUILD IT

> **You are not limited to what someone else built for you.**

**Pick your target on the day** based on the break-time conversations:

| Target | Best when the room is | Prompt |
|---|---|---|
| **OSCE checklist app** | Mostly clinical years | See A below |
| **Spotting/flashcard trainer** | Mostly 1st–2nd year | See B below |
| **Dose calculator** | Mixed, wants high wow | See C below — **disclaimer required** |

Open **Claude Code**. Narrate what you're doing as you type — they've never seen an engineer work.

**A — OSCE checklist**
```
Build a single-page web app: an OSCE examination checklist trainer
for medical students. Let me pick a station (cardiovascular exam,
respiratory exam, abdominal exam). Show the steps as tickable items
grouped into intro / exposure / inspection / palpation / percussion
/ auscultation / closing. Track a score as I tick, run a timer, and
at the end show which steps I missed. Clean, mobile-friendly,
works offline in a single file.
```

**B — Spotting trainer**
```
Build a single-page web app for anatomy spotting practice. I upload
images and add a label for each. It then quizzes me one image at a
time with a 30-second timer per image, hides the label until I
answer, tracks my score, and at the end re-shows only the ones I got
wrong. Mobile-friendly, single file, works offline.
```

**C — Dose calculator**
```
Build a single-page paediatric weight-based dose calculator for
teaching purposes. Input: weight, drug from a small preset list,
mg/kg. Output: dose per administration and per day, with the
calculation shown step by step so a student learns the method.
Display a permanent prominent banner: "TEACHING DEMO ONLY — NEVER
USE FOR PATIENT CARE." Mobile-friendly, single file.
```

> **If you build C, say the disclaimer out loud, twice.** You are in a room of future prescribers.

**Then share the link and let it open on their phones in the room.** That immediacy *is* the wow. Wait for the noise.

**Then the honest bridge — do not skip this:**

> "That's Claude Code. It's the paid tool I use for actual work, and I'm not pretending you're all going to buy it tomorrow. But this idea — describing what you want and getting working software — that part is free. Claude Artifacts. Gemini Canvas. Tonight, on a free account."

> "You just watched a person who has never opened your anatomy syllabus build you a study tool in four minutes. You know exactly what you need. That's the part I can't do."

**Fallback:** recording `08`. **Never skip the finale — play the recording instead.**

---

### `02:45–02:50` — CLOSE

Land it:

> "Four shifts. Ground it in your own material. Flip it so it examines you instead of answering you. Automate it so you set it up once. Verify it, always, because it's medicine.
>
> If you take one thing: **stop asking it for answers, start asking it to test you.** The exam room doesn't care what the AI knows. It cares what you know."

**The takeaway — no handout to hand out.** Tell them plainly:

> "I'm not giving you a sheet. I'm dropping every prompt from today in your class WhatsApp group tonight. Two things I want you to actually do before you sleep: set your custom instructions, and run one viva on whatever you're studying this week."

Then leave the **Mode 4 four-habits** on screen (retype them into whatever tool is open) long enough for the room to photograph it — that's the one thing worth them having in their own camera roll.

> *Optional:* if you'd rather give them something clickable, there's a prompt-copy page that carries every prompt from today, tap-to-copy — `https://claude.ai/code/artifact/ba687e33-6900-4dd7-a6d9-b8fc23e3a49e`. Drop it in the group instead of retyping. It's private until you share it from the page's share menu, so open it up first.

---

## PART 3 — CONTINGENCIES

| If this happens | Do this |
|---|---|
| **Wifi dies** | Switch to recordings folder. Say: "This is why you always have a backup — and that's true for your presentations too." Turn it into a point. |
| **Demo produces a boring answer** | Say so out loud. "That's a weak answer — watch what happens when I give it more to work with." Recovering visibly builds *more* trust than a clean run. |
| **Model refuses a clinical prompt** | Reframe as education: "I'm a medical student practising for an exam." Have this ready — it happens with dose/diagnosis prompts. |
| **Hands-on stalls the room** | Hands-on is optional and time-boxed. Announce the time, then move on regardless. Don't let 5 stuck people hold 45. |
| **Someone challenges you on cheating** | Don't get defensive. "Fair. That's exactly why Mode 4 exists and why I told you what I did as a student." |
| **Someone asks a deep clinical question** | "You're the doctor in this room, not me." Genuine, and it lands well. |
| **Running late** | Cut in this order: Mode 2 hands-on → Mode 3 hands-on → Mode 1 Demo 3 → Feynman check. **Never cut the finale.** |
| **Running early** | Take questions on their actual subjects and demo live. Best possible use of spare time. |

---

## PART 4 — THE NIGHT-BEFORE CHECKLIST

- [ ] NotebookLM notebook built with 3 real sources, tested
- [ ] Audio Overview pre-generated (it takes minutes — do not generate live)
- [ ] All 8 recordings captured and in one folder
- [ ] Broken-demo screenshot captured and DOI verified as fake
- [ ] Gem built once as a rehearsal, then deleted so you can build it live
- [ ] Claude Code finale run once end-to-end — know how long it actually takes
- [ ] Handwritten-notes photo + ECG/histology image on phone
- [ ] Speakers tested at hall volume
- [ ] Phone mirroring tested
- [ ] This guide open on your second screen / phone (NOT projected)
- [ ] Class WhatsApp group link handy, so you can drop the prompts at the end
- [ ] Every account logged in, unrelated tabs closed, notifications off
