# The Science Behind This System

This system is built on five research-backed methods. Understanding them helps you use the system correctly.

---

## 1. The Karpathy Feedback Loop — "Measure → Fix → Repeat"

Andrej Karpathy (AI researcher) describes effective learning as a tight feedback loop:

```
Practice → Measure output → Analyze failures → Fix specifically → Re-test → Repeat
```

Applied to German learning:
- **Practice** — speak, write, drill
- **Measure** — every error gets logged in `error_log.md`
- **Analyze** — `/errors review` finds your pattern (e.g., always wrong on Dativ)
- **Fix specifically** — `/grammar-drill Dativ` targets exactly that
- **Re-test** — next `/errors` session checks if it's gone
- **Repeat** — until the error disappears from your log

**Why this matters:** Most learners repeat what they're good at. This system forces you to drill what you're bad at. That's where the progress happens.

---

## 2. Active Recall + Spaced Repetition — "Retrieve, don't review"

Research finding (Roediger & Karpicke, 2008): Testing yourself is far more effective than re-reading.

- **Active recall** = producing the answer from memory (not recognizing it)
- **Spaced repetition** = reviewing at increasing intervals (not in one block)

Applied here:
- `/vocab` never shows you a word and says "remember this" — it makes you retrieve it under pressure
- Words you miss get drilled again immediately AND flagged for next session
- Grammar topics rotate back every few days, not revisited once in a long block

**Rule:** If you're reading German notes without producing anything, you're not learning — you're just feeling like you're learning.

---

## 3. Swain's Output Hypothesis — "You must produce, not just consume"

Merrill Swain found that French immersion students who received enormous amounts of input still couldn't produce French accurately.

Why: Consuming input uses passive processing. **Speaking and writing force you to notice gaps** in your knowledge that you didn't know you had.

Applied here:
- At least 50% of your study time must be production: speaking, writing, drilling gaps
- `/speak` forces you to produce German under pressure
- `/write` makes you construct full texts — you can't fake it with passive vocabulary

**The feeling you want:** That uncomfortable feeling of searching for a word, getting a case wrong, then being corrected. That's learning.

---

## 4. Krashen's i+1 — "Just above your level"

Stephen Krashen: you acquire language when the input is slightly above your current level (i+1). Too easy = no progress. Too hard = no understanding = no progress either.

Applied here:
- Claude calibrates examples, role-plays, and drills to your A2/B1 level
- When you do `/speak`, Claude uses the B1 vocabulary you need — not simplified A1
- Reading materials are B1 difficulty, not native-speaker journalism
- `/listen resources` recommends content at your exact transition level

**Your current i+1 zone:** You understand simple German and can form sentences. Your i+1 is: longer sentences, more connectors, correct case endings, Konjunktiv II, real-life vocabulary for Germany.

---

## 5. Deliberate Practice (Ericsson) — "Work at your edge"

Anders Ericsson studied experts across fields. The key: **deliberate practice** means:
- Focused on specific weaknesses (not general exposure)
- With immediate feedback
- Just outside your comfort zone
- With the intention to improve, not to perform

Applied here:
- `/errors` drills your specific errors, not general grammar
- `/grammar-drill` focuses on ONE topic per session
- Claude corrects every error (immediate feedback)
- Sessions push you to use structures you can't yet use automatically

**What to avoid:** Doing what feels comfortable. If `/speak` Arzttermin is now easy, move to a harder scenario. If you always do vocabulary and skip grammar, flip it.

---

## How the five methods work together

```
INPUT (i+1)              →  You encounter real German at your level
     ↓
OUTPUT (Swain)           →  You try to produce it
     ↓
ERROR (Karpathy loop)    →  You make mistakes, they get logged
     ↓
DRILL (Deliberate practice) → You specifically fix those errors
     ↓
SPACING (Spaced recall)  →  Errors reviewed again in 3–7 days
     ↓
FIXED                    →  Error disappears from log. Next target.
```

This is the whole system. Every skill in this project serves one of these five steps.

---

## Recommended external tools (complement this system)

| Tool | Purpose | Free? |
|------|---------|-------|
| **Anki** | Spaced repetition flashcards for vocabulary | Yes |
| **Slow German (podcast)** | Comprehensible input at A2–B1 | Yes |
| **DW Nicos Weg** | Structured A1–B1 video course | Yes |
| **Deutsche Welle Nachrichten** | Slow news for B1 listening | Yes |
| **Tandem / HelloTalk** | Language exchange partners (speaking) | Free tier |
| **Goethe practice tests** | Official B1 sample exams | Yes |
| **italki** | Paid tutors for real speaking practice | Paid |
| **ChatGPT / Gemini Voice** | Spoken conversation practice (audio) | Paid tier |

### On speaking with AI voice tools
Claude Code is text-based. For **actual spoken conversation practice with voice feedback**, use:
- **ChatGPT Voice Mode** (best for language learning among AI voice tools — understands prompt instructions about language practice)
- **Gemini Live** — free, works in German, 45+ languages
- **claude.ai** (the web app, not this CLI) — has voice mode

Use this system (Claude Code) for: structured drills, grammar, error tracking, writing, role-play in text.
Use a voice AI tool alongside it for: actual pronunciation, speaking flow, real-time spoken conversation.

NotebookLM is useful for: uploading your grammar book or notes and asking questions about them — but it doesn't drill you interactively.
