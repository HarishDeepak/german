# Skill: weekly-plan
**Use this skill for:** setting up your study week, reviewing progress, balancing all skills, making sure you don't skip weaknesses.

---

## What this skill does
Builds a realistic weekly German study plan based on your available time, current level, recent error log, and B1 exam goals. Reviews your plan mid-week or end-of-week.

## How to activate
- `/weekly-plan` — set up this week's plan
- `/weekly-plan review` — review how this week went and update
- `/weekly-plan short` — set up a plan for a short week (less time available)
- `/weekly-plan exam [date]` — create an exam-focused plan counting down to a date

---

## Weekly plan setup process

When you run `/weekly-plan`, Claude will ask:
1. How many days this week can you study?
2. How much time per session? (15 / 30 / 60 min)
3. Any major gaps from recent sessions or error log?
4. Any specific topics you want to hit?

Then Claude builds a structured week.

---

## Standard weekly template (30 min/day, 5 days)

| Day | Focus | Skill | Goal |
|-----|-------|-------|------|
| Monday | Speaking | `/speak` | Role-play one scenario (Arzt / Bahnhof / Meinung) |
| Tuesday | Grammar | `/grammar-drill [weak topic]` | One grammar topic, full drill cycle |
| Wednesday | Vocabulary | `/vocab` | Learn 8 new words + active recall drill |
| Thursday | Writing | `/write` | One B1-style writing task + correction |
| Friday | Errors + Review | `/errors` | Drill top 3 recurring errors from the week |
| Weekend | Input (listening/reading) | `/listen` | One listening session + comprehension task |

**Rotate speaking as often as possible** — it's your biggest gap.

---

## Minimum viable week (15 min/day, 3 days)

| Day | Focus | What to do |
|-----|-------|-----------|
| Day 1 | Speaking | `/speak` — one scenario, 10 min. Wrap-up 5 min. |
| Day 2 | Grammar | `/grammar-drill` — 1 topic, just the drill phase |
| Day 3 | Errors | `/errors` — 10 min drill, 5 min log update |

This is the floor. Do not skip all three.

---

## Study principles built into the plan

### 1. Output-heavy (Swain's principle)
At least 50% of study time must be PRODUCING German (speaking, writing, drilling).
Pure reading and listening are input — valuable, but not enough alone.

### 2. Deliberate practice (Ericsson)
Every session targets a specific weakness, not just what you're comfortable with.
Comfortable ≠ productive. Work at the edge of your ability.

### 3. Spaced repetition (Ebbinghaus)
Grammar topics and vocab rotate back every 3–7 days, not in one long block.
Distribute, don't cram.

### 4. i+1 (Krashen)
Material should be just above your current level: understandable with effort.
If you understand everything easily, it's too easy.

### 5. Feedback loop (Karpathy pattern)
Every session ends with a logged error or improvement note.
Review errors weekly. Fix them intentionally. Don't ignore patterns.

---

## Weekly session log
At end of each week, write one line per day in `logs/session_log.md`:
```
## Week of [date]
Mon: Speaking — Arzt scenario. Error: Dativ after bei. 
Tue: Grammar — Adjektivdeklination. Score: 8/12.
Wed: Vocab — 8 words: Wohnung theme. 6/8 correct first try.
Thu: Writing — formal email. Errors: register, adjective endings.
Fri: Errors drill — Dativ, Adjektivdeklination, haben/sein Perfekt.
```

---

## Monthly reset
Once per month, run `/weekly-plan review` to:
- See which topics you've drilled most (and which you're avoiding)
- Update the error log (mark fixed errors, add new ones)
- Adjust weekly focus based on actual progress
- Set one concrete goal for the next month
