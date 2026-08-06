# Demo Outputs — Offline Backup Pack

> **What this is:** a ready-to-show fallback for every live demo in the workshop, on the running topic of **photosynthesis**.
> **When to use it:** if wifi, login, or a tool fails on the day, read the "EXAMPLE OUTPUT (backup)" aloud or screen-share it instead of running the tool live.
> **How it's laid out:** one section per level, in run order. Each has the exact prompt (in a code block) and the output the AI would realistically return.

**Jump to:** [L1 Prompt it](#l1--prompt-it) · [L2 Ground it](#l2--ground-it-notebooklm) · [L3 Flip it](#l3--flip-it) · [L4 Automate it](#l4--automate-it) · [Verify](#verify) · [L5 Delegate it](#l5--delegate-it-agent)

---

## L1 — Prompt it

### (i) The lazy prompt

```
what is photosynthesis
```

*Note: returns a vague, undirected wall of text — a textbook dump with no structure, no analogy, no way to test yourself. Technically correct, practically useless. Don't read it out; just describe it.*

### (ii) The good prompt (biology-tutor RCTF)

```
You are a biology tutor (ROLE).
I'm revising for an exam and keep mixing up the light and dark
reactions of photosynthesis (CONTEXT).
Explain it in 5 simple steps with one everyday analogy, then ask
me 3 questions to test myself (TASK).
Keep it under 200 words, no jargon (FORMAT).
```

**EXAMPLE OUTPUT (backup)**

No problem — this mix-up is really common. Here it is in 5 steps:

1. **Light gets caught.** In the leaf, green chlorophyll absorbs sunlight. This is the start of the *light reactions*.
2. **Water is split.** That captured light energy splits water into hydrogen and oxygen. The oxygen leaves the leaf — that's the air we breathe out of the plant.
3. **Energy is packaged.** The light reactions store the energy in two carrier molecules (ATP and NADPH). Think of these as charged batteries.
4. **Sugar is built.** Now the *dark reactions* (the Calvin cycle) take over. They don't need light directly — they use those charged batteries to grab carbon dioxide from the air and build it into sugar.
5. **Fuel is ready.** The sugar (glucose) is the plant's food and stored energy.

**Everyday analogy:** the light reactions are like **charging your phone battery** during the day; the dark reactions are like **using that battery to run an app** — you can do it anytime, even after the sun's gone, as long as the battery is charged.

**Test yourself:**
1. Which reactions release oxygen — light or dark?
2. What are the two "charged batteries" the light reactions produce?
3. Where does the carbon in the new sugar come from?

*(Word count ~180.)*

---

## L2 — Ground it (NotebookLM)

### The cited-summary prompt

```
You are my study tutor (ROLE). Using only the sources I gave you
(CONTEXT), write a one-page high-yield summary of this lecture (TASK).
Cite the slide or page number for every point (FORMAT).
```

**EXAMPLE OUTPUT (backup)**

*(In NotebookLM the little numbers below are clickable — each jumps to the exact source passage. On the day, click one to show it isn't remembering, it's reading.)*

# Photosynthesis — High-Yield Summary

**The one-line definition.** Photosynthesis is the process by which green plants, algae, and some bacteria convert light energy, water, and carbon dioxide into glucose (chemical energy) and oxygen [1].

**Overall equation.** 6 CO₂ + 6 H₂O + light energy → C₆H₁₂O₆ + 6 O₂ [1][2].

**Where it happens.** In the **chloroplasts**, mostly in leaf cells. The green pigment **chlorophyll**, held in the chloroplast, absorbs light — mainly red and blue wavelengths, reflecting green [1].

**Two stages — don't mix them up:**

- **Light-dependent reactions** — occur in the **thylakoid membranes**. Light energy splits water (photolysis), releasing **oxygen** as a by-product, and stores energy as **ATP** and **NADPH** [2].
- **Light-independent reactions (Calvin cycle)** — occur in the **stroma**. They use the ATP and NADPH to "fix" carbon dioxide into **glucose**. No direct light needed, but they depend on the products of the light stage [1][2].

**Why it matters.** Photosynthesis is the base of nearly all food chains and the source of atmospheric oxygen [1].

**Factors that affect the rate.** Light intensity, carbon dioxide concentration, and temperature. Each can become the limiting factor if in short supply [2].

**Common exam trap.** Oxygen comes from **water**, not from carbon dioxide. The carbon in glucose comes from **CO₂** [2].

---
**Sources**
1. Britannica, "Photosynthesis" — britannica.com/science/photosynthesis
2. Khan Academy, "Introduction to photosynthesis"

> **Audio Overview (can't be pre-written — describe it):** Two AI hosts chat like a podcast — one plays the curious student, the other the tutor. They walk through the same lecture conversationally ("So wait, the oxygen actually comes from the *water*?" — "Right, that trips everyone up..."), swapping the two stages back and forth until it clicks. Roughly 6–8 minutes, sounds like two real people, built entirely from the uploaded source.

---

## L3 — Flip it

### The examiner prompt

```
You are a tough examiner (ROLE). Examine me on this lecture (CONTEXT).
Ask one question at a time, wait for my answer, never give it to me,
and probe deeper if I'm vague (TASK). After 8 questions, score me out
of 10 and name the two things to revise tonight (FORMAT).
```

**EXAMPLE OUTPUT (backup)** — *a realistic quiz transcript. Read the examiner lines; the "Student" lines are the answers you'd type back.*

**Examiner:** Right, let's begin. Question 1 of 8. In one sentence, what is photosynthesis?

**Student:** It's how plants make food using sunlight.

**Examiner:** Acceptable, but loose. "Make food" — food from *what raw materials*? Name them.

**Student:** Carbon dioxide and water.

**Examiner:** Good. Question 2. Where in the plant cell does photosynthesis take place?

**Student:** In the chloroplast.

**Examiner:** Correct. Question 3. Photosynthesis has two stages. Name them.

**Student:** The light reactions and the dark reactions.

**Examiner:** Fine — the second is also called the light-independent reactions, or the Calvin cycle. Remember that, examiners use both names. Question 4. In which stage is oxygen released?

**Student:** The dark reactions.

**Examiner:** No — and think carefully before I move on. Oxygen comes from splitting a molecule. Which molecule, and in which stage?

**Student:** Oh — water is split, in the light reactions.

**Examiner:** Correct. That's the single most common error on this topic, so good that you caught it. Question 5. The light reactions produce two energy-carrying molecules used later. Name them.

**Student:** ATP and... NADPH?

**Examiner:** Yes. Question 6. Where does the carbon in the newly made glucose come from?

**Student:** From carbon dioxide in the air.

**Examiner:** Correct. Question 7. The Calvin cycle is called "light-independent." Does that mean it can run indefinitely in the dark? Explain.

**Student:** Yes, because it doesn't need light.

**Examiner:** Careful — that's half right and half wrong. It doesn't use light *directly*, but what does it depend on that only the light stage can supply?

**Student:** The ATP and NADPH — so it stops once those run out in the dark.

**Examiner:** Exactly. It's "independent" of light but not independent of the light *reactions*. Question 8, last one. Name two factors that limit the rate of photosynthesis.

**Student:** Light intensity and temperature.

**Examiner:** Good. Carbon dioxide concentration is the common third.

---
**Score: 7 / 10.** Solid grasp of the raw materials, the location, and the two energy carriers. You lost marks on the two conceptual traps — where oxygen is released, and what "light-independent" really means.

**Revise tonight:**
1. **Oxygen comes from water (photolysis) in the light reactions** — not from CO₂, not in the dark reactions.
2. **"Light-independent" ≠ "runs forever in the dark"** — the Calvin cycle depends on ATP and NADPH from the light stage.

---

## L4 — Automate it

### (i) Custom instructions

```
I'm a university student preparing for exams (CONTEXT).
Act as my study tutor (ROLE).

When you answer: explain in clear simple steps, tell me your
confidence, and flag anything I should double-check or that's
region-specific (TASK).
Structure every answer as: definition → key points → example →
common mistakes (FORMAT).
```

**Example question:** "Explain the Calvin cycle."

**EXAMPLE OUTPUT (backup)** — *notice it follows the saved format automatically, without being told each time.*

**Definition.** The Calvin cycle is the light-independent stage of photosynthesis, taking place in the stroma of the chloroplast, where carbon dioxide is converted into glucose using the ATP and NADPH made in the light reactions.

**Key points.**
- It runs in three phases: **carbon fixation** (CO₂ is attached to a 5-carbon molecule, RuBP, by the enzyme **rubisco**), **reduction** (ATP and NADPH convert the result into a 3-carbon sugar, G3P), and **regeneration** (most G3P is recycled to remake RuBP so the cycle can continue).
- It does **not** use light directly, but it stops once the ATP and NADPH from the light reactions run out.
- For every one glucose molecule, the cycle must turn several times and fix six molecules of CO₂.

**Example.** Think of a small factory: trucks (CO₂) arrive, rubisco is the loading dock that clips each delivery onto a frame (RuBP), and the "charged batteries" (ATP/NADPH) power the assembly line that builds the sugar — while quietly rebuilding the frames so the next trucks have somewhere to dock.

**Common mistakes.**
- Calling it the "dark reactions" and assuming it needs darkness — it just doesn't need light *directly*.
- Forgetting it depends entirely on the light stage's products.
- Thinking one turn makes one glucose — it takes several turns.

*Confidence: high — this is standard, stable textbook biology. Nothing here is region-specific, so nothing to double-check for your exam board beyond confirming whether they want the enzyme "rubisco" named.*

### (ii) The "Study Coach" Gem

*Gem name:* `Study Coach` — loaded with the photosynthesis lecture, built once from this prompt:

```
You are my study tutor (ROLE). My lecture notes are in your files
(CONTEXT). Teach from my material and end every answer with one
follow-up question to check I understood (TASK).
If I say "QUIZ ME", examine me instead: one question at a time, no
answers, 8 questions, then score me (FORMAT).
```

**EXAMPLE OUTPUT (backup)** — *short transcript: it teaches, then the user types QUIZ ME and it flips to examiner mode.*

**You:** Can you explain why oxygen is a by-product of photosynthesis?

**Study Coach:** From your lecture: during the **light reactions**, the energy from sunlight is used to split water molecules — this is called photolysis. Water (H₂O) breaks into hydrogen and oxygen. The hydrogen is kept and used to make NADPH, but the oxygen isn't needed, so the plant releases it. That's the oxygen we breathe. So oxygen is a *waste product* of splitting water — nothing to do with the carbon dioxide.

*Quick check: in which stage of photosynthesis is that oxygen released — the light reactions or the Calvin cycle?*

**You:** The light reactions.

**Study Coach:** Exactly right. Want to move on to how the Calvin cycle uses the products of that stage?

**You:** QUIZ ME

**Study Coach:** Switching to examiner mode. No answers from me — I'll score you at the end. Question 1 of 8: Write the overall word equation for photosynthesis.

**You:** Carbon dioxide plus water, using light, makes glucose plus oxygen.

**Study Coach:** Noted. Question 2 of 8: Name the green pigment that absorbs light, and say which colours of light it absorbs best.

*(...continues one question at a time, no answers given, through Q8, then scores out of 10 — exactly like the L3 examiner.)*

---

## Verify

### An invented detail, and a habit that catches it

**Ask the AI:** "How efficient is photosynthesis at converting sunlight into chemical energy?"

**AI answers (confidently):**

> "Photosynthesis is remarkably efficient — most crop plants convert about **28% of the sunlight** that hits them into chemical energy, which is why plants are such effective solar collectors."

That number is **invented**. It sounds authoritative and precise, which is exactly the danger. In reality the theoretical maximum is roughly 11%, and most real crops manage only about **1–2%**. The AI predicted a plausible-sounding figure, not a true one.

**Habit 1 catches it — "Cite it, or tell me you can't."**

> **You:** Cite it, or tell me you can't.
>
> **AI:** I can't cite a reliable source for "28%." On checking, that figure appears to be incorrect — the commonly cited real-world efficiency of photosynthesis in crop plants is around 1–2%, with a theoretical maximum near 11%. I shouldn't have stated 28% as fact.

One question turned a confident fabrication into a corrected, sourced answer. That is the entire point of Verify: **never accept a number — a dose, a date, a statistic — without a source you can open.**

### The four habits (verbatim from the deck)

```
1. "Cite it, or tell me you can't."
2. "What would change this answer?"
3. "What's the strongest argument against what you just told me?"
4. "Which fact here is most likely to be out of date?"
```

---

## L5 — Delegate it (agent)

### The research prompt

```
You are my research assistant (ROLE). I want to know what actually
improves exam performance (CONTEXT). Research the main proven study
techniques (TASK) and write me a one-page summary with sources (FORMAT).
```

**EXAMPLE OUTPUT (backup)** — *what the agent would produce after breaking the goal into steps, gathering, and writing.*

# What Actually Improves Exam Performance — A One-Page Summary

The research on learning is unusually clear: a handful of techniques consistently outperform the ones most students actually use (rereading and highlighting). Here are the proven ones.

**1. Active recall (retrieval practice).** Testing yourself — pulling information out of memory rather than reading it back in — is the single best-evidenced technique. Every act of recall strengthens the memory. Use flashcards, past papers, or simply closing the book and writing down what you remember [1][2].

**2. Spaced repetition.** Spread your study of a topic over increasing intervals (a day, then a few days, then a week) instead of cramming it all at once. The small "effort" of nearly-forgetting and then recalling is what builds durable memory [1][3].

**3. Interleaving.** Mix different topics or problem types in one session rather than doing one type in a block. It feels harder and slower, but it trains you to *choose* the right method — which is what exams actually test [1][2].

**4. Elaboration.** Ask "why" and "how" and connect new material to what you already know. Explaining a concept in your own words, or teaching it to someone else, exposes the gaps that rereading hides [2][3].

**5. Concrete examples & dual coding.** Pair abstract ideas with concrete examples, and combine words with diagrams. Two routes into memory are stronger than one [2].

**What to drop:** rereading notes and highlighting feel productive but produce weak, short-lived learning. They create an illusion of fluency — you recognise the material without being able to recall it [1][2].

**The one-line takeaway:** don't study by *re-reading*; study by *retrieving* — test yourself, space it out, and mix it up.

---
**Sources**
1. Dunlosky et al. (2013), "Improving Students' Learning With Effective Learning Techniques," *Psychological Science in the Public Interest*.
2. Weinstein, Madan & Sumeracki (2018), "Teaching the science of learning," *Cognitive Research: Principles and Implications*.
3. Roediger & Karpicke (2006), "Test-Enhanced Learning," *Psychological Science*.

> **Companion build:** the flashcard quiz app from Level 5's build demo is delivered separately as a standalone HTML file — reference it here as the tool that puts technique #1 (active recall) into practice. No need to rebuild it from this pack.
