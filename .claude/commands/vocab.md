# Skill: vocab
**Use this skill for:** learning new words, drilling vocabulary, testing recall, building personal word lists, thematic vocabulary sessions.

---

## What this skill does
Runs focused vocabulary sessions using active recall, spaced repetition principles, and contextual learning. Never just shows me a list — always makes me retrieve words from memory under pressure.

## How to activate
- `/vocab` — Claude picks a thematic set or drills my personal vocab log
- `/vocab Körper` — vocabulary for body/health topic
- `/vocab test` — test me on words from my vocab_log.md
- `/vocab new 10` — teach me 10 new high-frequency words with drills
- `/vocab Wort [word]` — deep-dive on one word (meaning, forms, collocations, example sentences)
- `/vocab weak` — drill only words I've gotten wrong before

---

## Session structure

### Mode A: Learn new words
1. Present 5–8 words in a thematic group (not random)
2. For each word:
   - German word + article (for nouns) + plural
   - English meaning
   - Example sentence (simple, real-life)
   - One common collocation or phrase
3. After presenting all words: immediate recall drill
4. End with 3 original sentences using words from the set

### Mode B: Active recall drill
I get the English. I produce the German. No peeking.
Format:
> 🔁 **[English word/phrase]** → ?
> (I answer)
> ✓ richtig / ❌ falsch: **[correct form]**

Scoring at the end: X/Y correct. Words I missed → flagged in session summary for `vocab_log.md`.

### Mode C: Context sentences
Claude gives me a sentence with a blank. I fill in the correct word.
> "Ich habe einen ___ beim Arzt." → Termin
> "Das kostet zu ___." → viel

### Mode D: Word deep-dive
For one word I want to master completely:
- All forms (noun: article + plural / verb: all tenses + past participle / adj: comparative)
- Common collocations
- 3 example sentences in ascending difficulty
- Common errors learners make with this word
- Related words (Wortfamilie)

---

## Vocabulary learning rules (based on best methods)
1. **Context beats lists** — always learn words in a sentence
2. **Retrieve, don't review** — I must produce the word, not just read it
3. **Spaced review** — words I miss get drilled again at end of session and flagged for next session
4. **Thematic clustering** — learn 5–8 related words at once, not random words
5. **High frequency first** — always prioritize the most common words

---

## High-frequency word themes (A2 → B1 priority)

### Tier 1 — Core daily (learn first)
- Numbers, time, dates, months, seasons
- Colors, sizes, quantities
- Common verbs: machen, gehen, kommen, haben, sein, werden, brauchen, wissen, kennen, sehen, hören, sagen, fragen, antworten, arbeiten, wohnen, fahren, kaufen, bezahlen, helfen, warten, beginnen, enden
- Common adjectives: groß, klein, alt, neu, gut, schlecht, schön, wichtig, möglich, einfach, schwierig, teuer, billig, schnell, langsam, früh, spät

### Tier 2 — Life in Germany
- Transport: die U-Bahn, der Bus, der Zug, die S-Bahn, das Ticket, die Verspätung, der Anschluss, umsteigen, einsteigen, aussteigen
- Shopping: der Supermarkt, die Kasse, das Angebot, der Rabatt, die Quittung, bezahlen, bar, mit Karte
- Health: der Arzt, die Ärztin, das Rezept, die Apotheke, der Termin, die Krankenkasse, sich krank melden, Schmerzen haben
- Housing: die Wohnung, der Vermieter, die Miete, die Nebenkosten, der Mietvertrag, kündigen, einziehen, ausziehen
- Bureaucracy: das Amt, anmelden, abmelden, das Formular, der Ausweis, die Genehmigung, beantragen, der Bescheid

### Tier 3 — Opinions and connectors (essential for B1 speaking/writing)
- Meinung: meiner Meinung nach, ich finde, ich denke, ich glaube, ich bin der Ansicht
- Connectors: weil, deshalb, deswegen, trotzdem, obwohl, außerdem, jedoch, allerdings, einerseits…andererseits, zum Beispiel, nämlich, schließlich, zwar…aber
- Contrast: aber, sondern, jedoch, trotzdem, obwohl, während
- Addition: und, auch, außerdem, dazu, zudem, darüber hinaus

---

## Vocab log update format
At end of every session, Claude produces a short update block:
```
## Vocab session — [date]
Learned: [word1], [word2], [word3]...
Needs review: [words I missed]
Topic: [theme]
```
I paste this into `logs/vocab_log.md`.

---

## Word forms cheat sheet (nouns)
Always learn nouns as: **Article + Noun (Plural)**
> der Mann (die Männer) — the man
> die Frau (die Frauen) — the woman
> das Kind (die Kinder) — the child

Never learn a noun without its article. Ever.
