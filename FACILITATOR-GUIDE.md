# Facilitator Guide — "Stop Asking. Start Building."

**AI as a tool for medical students · RLMC**
Duration: 2 hr 50 min (incl. 10 min break) · Audience: 20–50 MBBS students, mixed years · Devices: phones + some laptops

> **The one sentence this workshop exists to deliver:**
> *You already use AI to get answers. Almost nobody in this room uses it to be examined, to be grounded in their own material, or to build something. That's the gap.*

> **How to run this workshop:** there is no slide deck. **Your screen is the show.** You live-drive the actual tools — NotebookLM, Gemini, Claude, Claude Code — and the students watch you do real things, not slides about them. This document is your private script: keep it open on a second screen, your phone, or a printout. Nothing in here is meant to be projected. Part 2 is a minute-by-minute run sheet; the **bold quoted lines are what you say out loud**, the `code blocks` are what you paste into the tool on screen.

> **You are not the medical expert — and the demos don't ask you to be.** The demos *you drive* use plain, everyday general-knowledge topics anyone in the room can follow and fact-check — this guide uses **the water cycle, the solar system, photosynthesis, compound interest, and the history of the ballpoint pen**. Use them as written, or swap in anything you know cold; you're teaching the *technique*, not the subject. (The document-based demos — Mode 1 and the Gem — stay on **the water cycle** throughout, because they build on the same uploaded notes.) Every *hands-on block* then flips it: students load their **own real course material** — that's where the medical content belongs, supplied by the people who can actually judge it. The medical *framing* stays (it's why this matters to them); only the demo *content* is generic.

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

*This is the **facilitator's demo set** — all on one neutral topic you know well (this guide uses **the water cycle**). Students bring their own real course material for the hands-on parts; you don't need any.*

1. **A short explainer/notes PDF** on your example topic — e.g. the Wikipedia article on the water cycle exported to PDF, or any 5–15 page explainer. *(NotebookLM notebook + the Mode 3 Gem — this is your "lecture notes".)*
2. **A one-page set of practice questions** on the same topic. Don't have one? Generate it with AI the night before and save as PDF. *(NotebookLM notebook — this is your "past paper"; it powers the gap-analysis demo.)*
3. **A second source** on the same topic (another article/chapter PDF). *(NotebookLM notebook — adds depth.)*
   *Items 1–3 become the NotebookLM notebook. Load them the night before, not live.*
4. **A simple one-page outline** of the topic's subtopics. *(Mode 3, Demo 2 — you upload this into the "Topic Tutor" Gem live; it stands in for a syllabus.)*
5. **A photo of some handwritten notes** on your phone (messy is better — it's more impressive). Any subject. *(Mode 3, Demo 3.)*
6. **A photo of any diagram, chart, or figure** you can talk about — a graph, a labelled diagram, an infographic. *(Mode 3, Demo 3 — you'll ask the AI to "read" it.)*
7. **2–3 labelled images** — *only if you might pick the image-quiz finale (Target B)*; any images with labels (flags, landmarks, logos — anything). You upload these into the app you build. The other two finale targets need no files.

### D. Recordings to capture (night before) — NON-NEGOTIABLE

Wifi in a lecture hall is not a dependency you bet a workshop on. Screen-record every demo below and keep them in one folder on your laptop. *(Numbered `02`–`08` to match the run-sheet fallbacks — there is no `01`; the old opening broken-demo was cut, and its fabrication point now lives in Mode 4 / recording `07`.)*

- [ ] `02` — NotebookLM cited answer
- [ ] `03` — NotebookLM Audio Overview playing
- [ ] `04` — viva examiner exchange
- [ ] `05` — Gemini Live role-play + debrief
- [ ] `06` — Gem being built + used
- [ ] `07` — fake citation being caught
- [ ] `08` — **Claude Code building the app, start to finish**

`08` is the most important recording you will make. If the finale fails live, the workshop's closing moment fails with it.

### E. The Mode 4 fake-citation demo — capture this in advance

**You cannot rely on a model failing on cue** — *especially* now that even the free models are strong. That's exactly why the fabrication you show in **Mode 4 (Verify)** is prepared the night before, not gambled on live. Fish for a good failure, screenshot it and capture recording `07`, and have it ready.

What still reliably breaks — even on a good, current model — try these with web search **off**:

```
List 5 peer-reviewed papers, with DOIs, on the cultural history of coffee.
```

```
Quote the exact wording of clause 4.2 of the ISO 9001 standard,
word for word.
```

Then check the DOIs at doi.org. Screenshot one that resolves to nothing. **That's your Mode 4 payoff** — see the run sheet at `02:00–02:20`.

### F. Room setup

- [ ] Laptop + HDMI tested, screen mirroring confirmed
- [ ] **Speakers tested and loud** — two demos are audio (Audio Overview, Gemini Live)
- [ ] **A handheld mic (or the room mic) tested** — Mode 2 puts a student volunteer on the mic for the viva and the Gemini Live role-play; the whole room must hear them
- [ ] Know you'll need **two student volunteers in Mode 2** (the viva examinee + someone for the live role-play/interview) — recruit them on the spot; nothing to pre-arrange, just don't be caught off guard
- [ ] Phone screen-mirroring working (for the Gemini Live role-play demo) — or hold the phone to a mic
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

> "Twinkle, twinkle, little…"

The room shouts **"STAR."** Do two or three more:

> "Better late than…" → *never*
> "Salt and…" → *pepper*
> "Once upon a…" → *time*

*(A medical room warms up even faster to medical stems — "the patient presented with chest…" → PAIN. Use those instead if you're comfortable; the point is identical.)*

**Say the line:**
> "Notice you all said the same word. Nobody looked anything up. You just knew what usually comes next. Hold onto that — you just did exactly what the AI does."

**Round 2 — the fork (3 min).** Now a stem with more than one good answer:

> "I walked into the kitchen and picked up the…"

You'll hear *kettle, cup, knife, phone, spoon.* **Say the line:**
> "See what happened? It's not one answer — it's a spread of likely ones, each with a probability. The AI keeps a list exactly like that, then picks one. Change which one it picks and you get a slightly different sentence every time. That's why it never answers the same way twice."

**Round 3 — the reveal (4 min).** Call back to their "What is AI?" answers from the top, then land what they just proved:

> "At the start I asked what AI is. Some of you said a robot, a brain, something that knows everything. Here's the honest answer: it's none of those. That is *all* a large language model does — it read basically the whole internet, every textbook, every paper, every forum, and all it learned was: given the words so far, what word probably comes next. Then it does that again. And again. One word at a time, faster than you can read. There is no fact-box inside it. No library it looks things up in. It's the most powerful autocomplete ever built."

**Then the trap that makes the rest of the day matter (3 min):**

> "So watch what happens when I ask it for a reference. It has never seen your exact paper — but it has seen *thousands* of references. So it predicts what a reference should *look like*: a plausible author, a real-sounding journal, a DOI in the right format. It's not lying to you. It literally cannot tell the difference between a real citation and a citation-shaped sentence. It's just finishing the pattern."

> "And here's the thing — these models have got *very* good. The free one in your pocket is genuinely impressive. But 'impressive' and 'trustworthy' are different words. A confident, perfectly-formatted answer and a *true* answer look identical, and the machine can't tell them apart. I'm going to prove that to you live later, in the part on verifying — hold the thought until then."

> "In your field, a confident wrong answer isn't a typo. It's a patient. So everything I show you now is really about one thing: how to steer this thing toward true, and how to catch it when it isn't."

**Frame the session.** Four shifts, then we build something.

`GROUND IT → FLIP IT → AUTOMATE IT → VERIFY IT → BUILD IT`

> *But first — the one skill sitting under all of them.*

---
// Moreover prompting is the foundation of every agent/llm we talk with, its what forms the basis of hwo we communcicate wiht an llm model and that the only skill we need tod evleop right mow (basically note for me here I might give a small speech or create this a discussion point) 
### FOUNDATION — bad prompt vs good prompt (≈8 min, just before Mode 1)

> **This is not a fifth mode — it's what makes the other four work.** Every mode below is just a *good* prompt pointed at a job. So before the tools, one skill: how to actually talk to it.

*This adds ~8 min. The timestamps below don't include it — either shift them all back ~8 min, or buy the time back from a later hands-on (see Contingencies). Don't cut this.*

**Show the difference live, same topic, side by side.**

**The bad prompt** — type it, let the vague answer land:

```
tell me about the water cycle
```

> "Technically correct. Totally useless — a wall of text, because I gave it nothing to aim at."

**The good prompt** — same topic, four things added:

```
You are a tutor for a student revising for an exam (ROLE).
I keep mixing up the stages of the water cycle (CONTEXT).
Explain it in 5 simple steps, then give me 3 quick questions to test
myself (TASK). Keep it under 200 words, no jargon (FORMAT).
```

> "Same model, same topic. The only thing that changed is I told it *who to be, what I need, what to do, and what shape to hand back*. That's the whole skill."

**The takeaway — put it on screen and tell them to photograph it:**

```
A good prompt has four parts:
ROLE    — who it should be       ("you are a tutor…")
CONTEXT — your situation         ("I'm revising and I keep mixing up…")
TASK    — what to actually do    ("explain, then quiz me")
FORMAT  — the shape to hand back ("5 steps, under 200 words, no jargon")
```

> "You'll see all four in every prompt I use for the rest of today. Watch for them."

---

//before starting this section i need to present them a summary of what we would be discussing today (i.e a plan for today)
### `00:20–00:50` — MODE 1: GROUND IT

> **Stop asking what it remembers. Make it read what you gave it.**

**Go to:** notebooklm.google.com (notebook pre-loaded from prep step C)

**Demo 1 — the citation (5 min).** Ask your notebook:

```
Using only my sources, give me a one-page high-yield summary of
the water cycle for revision. Cite the slide or page number for
every claim.
```

Click a citation. It jumps to the exact slide. **Say the line:**
> "It's not remembering. It's reading. And it's showing you where it got it."

**Demo 2 — the refusal (3 min).** Ask something deliberately outside the sources.

```
What do my notes say about the French Revolution?
```

It says it isn't in your sources. **Say the line:**
> "It just said 'I don't know.' Your chatbot almost never does that. That's the whole difference."

**Demo 3 — the gap analysis (5 min).** This is the one they'll actually use tonight:

```
Compare my notes against the practice questions. What comes up in
the questions that my notes do NOT cover? List it as a revision
checklist.
```

**Demo 4 — Audio Overview (7 min).** Generate it, then **play it out loud.** Customise first:

```
Focus on the water cycle. Explain it at the level of a student
revising for an exam. Emphasise the points most likely to be tested.
```

> "That's your commute. That's the queue at the canteen. Your lecture deck is now a podcast."

**HANDS-ON (10 min).** Everyone opens notebooklm.google.com and uploads **one of their own real lecture PDFs** — this is where the medical content comes in, theirs not yours — asks one question, hits Generate Audio Overview.
*Walk the room. Expect: file too large, wrong Google account, unsupported format. Nobody is stuck for more than 2 min — pair them up.*

**Fallback:** recordings `02`, `03`.

---

### `00:50–01:20` — MODE 2: FLIP IT

> **It shouldn't answer your questions. It should ask you questions.**

**Demo 1 — the viva examiner (10 min). Get a volunteer on the mic.**

Paste into Claude or Gemini:

```
You are a tough oral examiner for my course. Examine me on
the solar system.

Rules:
- Ask ONE question at a time, then wait for my answer.
- Never give me the answer.
- If I'm vague or wrong, probe deeper the way a real examiner does.
- Escalate difficulty as I do well.

After 8 questions, stop and give me: my score out of 10, the two
gaps that would have failed me, and exactly what to revise tonight.
```

Ask the volunteer what they're studying and swap the topic in — let them squirm a little on their own subject. It's more memorable than a smooth run.

**Demo 2 — the live role-play partner (12 min). THE MOMENT OF THE WORKSHOP.**

Open **Gemini Live on your phone** (mirrored/held to mic). Voice mode, speak this:

```
You are an interviewer for a university admission (or a job). Stay in
character at all times — never break character.

Ask me realistic questions one at a time and wait for my answer. Be a
little challenging, the way a real interviewer is. Don't coach me
mid-answer.

When I say "END", drop character and tell me: how I came across, my
two weakest answers, and exactly what to improve.
```

Bring a **volunteer** up to be interviewed out loud. Let it run 4–5 min. Then say **END** and read the debrief to the room.

> "You can practise like that every night. For free. Unlimited attempts, and it never gets tired of you."

**Then hand the medical version straight to the room:**
> "Now — medics, your version of this is gold. Swap 'interviewer' for a patient with a hidden condition who only answers what you actually ask, and you've got an endless supply of history-taking and communication practice. Same technique, your subject. That's exactly what tonight's hands-on is about."

**Demo 3 — the Feynman check (5 min).**

```
I'm going to explain photosynthesis to you as if you're the examiner.
Don't correct me while I talk. When I finish, tell me: which parts
I actually understood, which parts I was reciting without
understanding, and the one question an examiner would ask to
expose the gap.
```

> "That last one is the difference between passing and being caught out."

**HANDS-ON (5 min).** Pairs. One person runs a 3-min viva on **a topic from their own course** — their material, their subject.

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
I'm a university student preparing for exams.

When you answer me:
- Explain in clear, simple steps.
- Structure answers as: definition → key points → example →
  common mistakes.
- Tell me how confident you are, and what I should double-check in a
  trusted source.
- If something is region- or context-specific, flag it.
```

> "You write that once. It applies to every conversation you have from now on. Most people never open this screen."

> *To the room:* "In the hands-on you'll write your own. A medic would add: 'use drug names as used in Pakistan, structure answers viva-style, never give a dose without a source.' That's your content — you know what belongs there, I don't."

**Demo 2 — a saved assistant, built live (12 min).** Use **Gemini Gems** (free, unlimited, 10 files each) — gemini.google.com → *Gems* → *New Gem*.

Name: `Topic Tutor — the water cycle`

```
You are my tutor for the water cycle. My notes and outline are in
your files.

Always:
- Answer from my uploaded material where possible; say clearly when
  you're going beyond it.
- End every answer with one follow-up question to check I understood.

If I say "QUIZ ME", stop teaching and examine me instead: one
question at a time, no answers given, 8 questions, then score me.
```

Upload your outline. Use it. **Then close it and reopen it** — show that it remembered everything.

> "That's a tutor that knows your material and your exam format, and it's still there in March. This — a saved, reusable assistant you set up once — is exactly what people mean when they talk about giving an AI a 'skill'."

**This is your "skills" moment — and it's the free, hands-on one:**
> "You'll hear about 'custom GPTs' and 'Claude Skills'. Same idea — a custom AI expert you build once and reuse. But *creating* those needs a paid plan. Gemini Gems does the same job for free. So this is the one you'll actually build tonight."

*Mention only:* Claude Projects does the same thing (free, 5 projects). Claude Skills and custom GPTs are **paid to create** — on free you can only run ones others made. Scheduled recurring quizzes are **paid** too — don't follow along.

**Demo 3 — your phone camera is an input (5 min).** Photograph your messiest handwritten notes:

```
Convert these handwritten notes into clean structured notes.
Flag anything you couldn't read clearly rather than guessing it.
```

Then the diagram/chart image:

```
Walk me through reading this figure step by step, the way I'd need
to explain it to someone else. Don't just tell me the answer — teach
me the method.
```

> "Note what I asked for. Not the answer — the *method*. Ask for the answer and you learn nothing."

**HANDS-ON (6 min).** Set custom instructions (everyone) — **with their own subject and exam** — then build one Gem / "skill" on their own material if there's time.

**Fallback:** recording `06`.

---

### `02:00–02:20` — MODE 4: VERIFY IT

> **How not to get burned. This is the part that matters most in your profession.**

**The three failure modes that matter — and land hardest in medicine:**

1. **Outdated information** — training data has a cutoff; facts, prices, and guidelines all move.
2. **Fabricated citations** — papers, quotes, and references that don't exist, with real-looking details.
3. **Context mismatch** — advice written for another country, system, or year that doesn't apply to yours. *For medics: US/UK guidance ≠ Pakistani practice, local drug availability, resistance patterns — they've never thought about it.*

**Demo — catch a fake citation live (7 min).** Play recording `07`, or run it live:

```
Give me 5 peer-reviewed references, with DOIs, on the history of
the ballpoint pen.
```

Take one DOI → doi.org → nothing. Or Google Scholar → no such paper.

> "Remember what I promised during the word game at the start — that I'd prove this to you live? Here it is. It's not looking up a paper — it's predicting what a paper should *look* like. That paper does not exist. It doesn't matter how good the model is; this is baked into how it works. And if that citation goes into your research project, it's your name on it, not the AI's."

**The four habits (8 min)** — type these into whatever tool is on screen, big, and tell the room to photograph it. This is the one thing worth them having in their camera roll:

```
1. "Cite it, or tell me you can't."
2. "What would change this answer?"
3. "What's the strongest argument against what you just told me?"
4. "Which fact here is most likely to be out of date?"
```

Plus the hard rule: **never accept a number — a dose, a date, a statistic — without a source you can open.**

**Ethics, 3 minutes, no sermon (5 min).** Be blunt and be honest:

> "I'm not going to tell you not to use it for assignments. I did. But your vivas are oral, in person, in front of a consultant who will ask you the follow-up question. If the AI learned it and you didn't, you find that out in the worst possible room. Use it to *get examined*, not to get finished."

---

### `02:20–02:45` — FINALE: BUILD IT

> **You are not limited to what someone else built for you.**

**Pick your target on the day** based on the break-time conversations:

| Target | Good for | Prompt |
|---|---|---|
| **Flashcard / quiz app** | any room — safest default | See A below |
| **Image-label quiz trainer** | visual subjects | See B below |
| **Study-timer app** | simplest build, still a "wow" | See C below |

Open **Claude Code**. Narrate what you're doing as you type — they've never seen an engineer work.

**A — Flashcard quiz app**
```
Build a single-page web app: a flashcard quiz trainer. Let me type in
a list of question/answer pairs. It then quizzes me one at a time,
hides the answer until I click, tracks my score, and at the end
re-shows only the ones I got wrong. Clean, mobile-friendly, works
offline in a single file.
```

**B — Image-label quiz trainer**
```
Build a single-page web app for image-label quiz practice. I upload
images and add a label for each. It then quizzes me one image at a
time with a 30-second timer, hides the label until I answer, tracks
my score, and at the end re-shows only the ones I got wrong.
Mobile-friendly, single file, works offline.
```

**C — Study-timer app**
```
Build a single-page study-timer web app. Let me set a focus length
and a break length, then run a countdown that switches between focus
and break automatically and counts how many focus sessions I've done
today. Clean, mobile-friendly, works offline in a single file.
```

> **Whichever you pick, keep it to one clean feature that visibly works** — a small app that runs beats an ambitious one that half-breaks live.

**Then share the link and let it open on their phones in the room.** That immediacy *is* the wow. Wait for the noise.

**Then the honest bridge — do not skip this:**

> "I built you a generic one so you could see it's possible. But you know your field — you could build the OSCE checklist, the drug-dose trainer, the anatomy spotting deck. I couldn't; I don't know what goes in them. You do."

> "That's Claude Code — the paid tool I use for real work, and I'm not pretending you'll all buy it tomorrow. But the *idea* — describing what you want and getting working software — is free. Claude Artifacts. Gemini Canvas. Tonight, on a free account."

> "You just watched someone who has never opened your syllabus build a working study tool in four minutes. You know exactly what you need. That's the part I can't do."

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
| **A student's clinical prompt gets refused** | Reframe as education: "I'm a medical student practising for an exam." Have this ready — it can happen with dose/diagnosis prompts in the hands-on. |
| **Hands-on stalls the room** | Hands-on is optional and time-boxed. Announce the time, then move on regardless. Don't let 5 stuck people hold 45. |
| **Someone challenges you on cheating** | Don't get defensive. "Fair. That's exactly why Mode 4 exists and why I told you what I did as a student." |
| **Someone asks a deep clinical question** | "You're the doctor in this room, not me." Genuine, and it lands well. |
| **Running late** | Cut in this order: Mode 2 hands-on → Mode 3 hands-on → Mode 1 Demo 3 → Feynman check. **Never cut the finale.** |
| **Running early** | Take questions on their actual subjects and demo live. Best possible use of spare time. |

---

## PART 4 — THE NIGHT-BEFORE CHECKLIST

- [ ] NotebookLM notebook built with 3 sources on your example topic, tested
- [ ] Audio Overview pre-generated (it takes minutes — do not generate live)
- [ ] All 7 recordings (`02`–`08`) captured and in one folder
- [ ] Mode 4 fake-citation prepared: a fabricated DOI captured (screenshot + recording `07`) and verified as fake at doi.org
- [ ] Gem built once as a rehearsal, then deleted so you can build it live
- [ ] Claude Code finale run once end-to-end — know how long it actually takes
- [ ] Handwritten-notes photo + a diagram/chart image on phone
- [ ] Speakers tested at hall volume
- [ ] Phone mirroring tested
- [ ] This guide open on your second screen / phone (NOT projected)
- [ ] Class WhatsApp group link handy, so you can drop the prompts at the end
- [ ] Every account logged in, unrelated tabs closed, notifications off
