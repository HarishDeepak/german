# Skill: errors
**Use this skill for:** reviewing your error log, drilling your recurring mistakes, turning weaknesses into strengths, analyzing error patterns.

---

## What this skill does
This is the Karpathy feedback loop applied to language learning: you make errors → they get logged → you drill exactly those errors → you retest → repeat until fixed. This is how you close gaps instead of just repeating what you already know.

## How to activate
- `/errors` — Claude reads my error log and drills the top 3 recurring errors
- `/errors review` — show me a summary of my current error patterns
- `/errors drill [topic]` — drill errors specifically in one area (grammar / vocab / speaking / writing)
- `/errors add [error]` — I manually add an error to log
- `/errors clear [topic]` — remove fixed errors from log

---

## The feedback loop (how this works)

```
Practice → Error occurs → Log it → Analyze pattern → 
Targeted drill → Retest → Mark as fixed (or continue drilling)
```

This is more effective than general practice because:
- You fix YOUR specific errors, not average learner errors
- Spaced repetition happens on YOUR weak spots
- You build an accurate picture of your actual gaps
- Every session gets more targeted over time

---

## Error log format

Errors live in `logs/error_log.md`. Format:

```
## Error: [short name]
- **Type:** grammar / vocabulary / phrasing / pronunciation
- **My version:** ❌ ...
- **Correct version:** ✓ ...
- **Rule:** one sentence
- **First seen:** [date]
- **Times repeated:** 0
- **Status:** active / drilling / fixed
```

---

## Error pattern categories

Claude will analyze errors and group them:

### Grammar errors
- Case errors (wrong article, wrong pronoun form)
- Verb form errors (wrong tense, wrong conjugation, haben vs. sein)
- Word order errors (verb in wrong position, subordinate clause verb position)
- Adjective ending errors
- Preposition errors (wrong preposition, wrong case after preposition)

### Vocabulary errors
- Wrong word choice (false friends, near-synonyms used incorrectly)
- Missing collocation (using wrong verb with a noun: *einen Fehler **machen***, not tun)
- Missing article (learning a noun without its gender)
- Anglicism (direct translation that doesn't work in German)

### Phrasing errors
- Unnatural register (too formal, too informal for context)
- English sentence structure imposed on German
- Missing connectors (using and/but when a richer connector would work)

---

## Drill session (when running /errors)

### Step 1: Error summary
Claude reads the log and reports:
> You have [X] active errors. Most repeated: [list top 3].
> Today we're drilling: [error 1], [error 2], [error 3].

### Step 2: Targeted mini-drills
For each error (5–8 items per error):
- Show the error context
- I produce the correct form
- Immediate feedback
- If wrong again: one-line rule reminder + retry

### Step 3: Progress update
Claude suggests which errors to mark as fixed and which need more drilling.
Update `logs/error_log.md` accordingly.

---

## My top A2→B1 error patterns (common for learners at this level)

1. **Akkusativ vs. Dativ confusion** — especially after two-way prepositions
   > in dem / im (location, Dat) vs. in den (movement, Akk)

2. **haben vs. sein in Perfekt**
   > Ich habe gegangen ❌ → Ich bin gegangen ✓

3. **Verb at end of subordinate clause**
   > Ich denke, dass er kommt nicht ❌ → dass er nicht kommt ✓

4. **Adjective endings** — especially after indefinite article
   > ein großer Mann (Nom) / einen großen Mann (Akk)

5. **Separable verbs in subordinate clauses**
   > weil ich um 8 Uhr aufstehe (verb stays together at end)

6. **Modal verb structure**
   > Ich muss heute lernen (infinitive at end, not conjugated)

7. **Kein vs. nicht**
   > Ich habe kein Auto (noun) / Ich fahre nicht (verb/adjective/adverb)

8. **Reflexive verbs (sich)**
   > Ich freue mich (not: Ich freue)

9. **Word order after time/place adverbials**
   > Heute gehe ich... (verb second, not Heute ich gehe)

10. **False friends**
    > aktuell = current (not actual) / sympathisch = likeable (not sympathetic)
