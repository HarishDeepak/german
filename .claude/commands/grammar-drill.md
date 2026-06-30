# Skill: grammar-drill
**Use this skill for:** drilling one specific grammar topic, understanding a rule, fixing a recurring mistake, working through a grammar chapter.

---

## What this skill does
Runs a focused grammar session on exactly one topic. Explains the rule concisely, gives examples, then drills me with exercises until I get it right. Tracks errors for the error log.

## How to activate
Say `/grammar-drill` followed by the topic. Examples:
- `/grammar-drill Dativ` — practice Dativ case and articles
- `/grammar-drill Adjektivdeklination` — all three adjective ending tables
- `/grammar-drill Perfekt` — Perfekt formation, haben vs. sein
- `/grammar-drill Wortstellung` — word order in main and subordinate clauses
- `/grammar-drill Konjunktiv II` — würde + Infinitiv, wäre, hätte
- `/grammar-drill` — Claude picks the topic with most errors in my log

---

## Session structure

### Step 1: Rule (max 5 lines)
State the rule as briefly as possible. A table if helpful. No paragraphs.

### Step 2: Examples (3–5)
Show the rule in real sentences. Always include a wrong version with correction.

### Step 3: Drill (10–20 items)
Mix of:
- **Gap fill** — complete the sentence with the correct form
- **Transform** — rewrite the sentence using the target structure
- **Error correction** — find and fix my mistake
- **Translation** — short English sentence → German

I answer. Claude corrects immediately. When I make an error, Claude explains it in one sentence, then gives a retry.

### Step 4: Production (2–3 items)
I write 2–3 original sentences using the structure. Claude corrects and rates them.

### Step 5: Summary card
At the end, Claude writes a mini reference card I can paste into `notes/grammar_notes.md`:
```
## [Topic] — Quick Reference
Rule: ...
Pattern: ...
Example: ...
Watch out for: ...
```

---

## Grammar topic list (A2 → B1, priority order)

### Must master first (A2 foundations)
1. Articles in all 4 cases (der/die/das/ein/eine — all 4 cases)
2. Personal pronouns in all cases
3. Present tense regular and irregular verbs
4. Modal verbs (können, müssen, wollen, sollen, dürfen, mögen)
5. Perfekt — haben vs. sein, participle formation
6. Präteritum of sein, haben, modal verbs
7. Separable verbs (trennbare Verben)
8. Negation: nicht vs. kein
9. Basic word order (V2 rule, questions)
10. Basic subordinate clauses: weil, dass, wenn

### Core B1 targets
11. Dativ case — prepositions, indirect object
12. Genitive case — basic recognition and use
13. Two-way prepositions (Wechselpräpositionen): in, an, auf, über, unter, vor, hinter, neben, zwischen
14. Adjective endings — attributive (all 3 declension types)
15. Adjective endings — after indefinite article
16. Relative clauses (Relativsätze)
17. Reflexive verbs (reflexive Verben)
18. Passive voice (werden-Passiv, present and past)
19. Konjunktiv II — würde + Inf, wäre, hätte, könnte, müsste
20. Infinitive constructions: zu + Inf, um…zu, ohne…zu, statt…zu
21. Futur I (werden + Infinitiv)
22. da- and wo-compounds (damit, worüber, etc.)
23. Extended subordinate clauses: obwohl, als, sobald, damit, falls
24. Nominalisierung (turning verbs into nouns)

---

## Drill format examples

**Gap fill:**
> Ich gehe __ (der) Supermarkt. → *in den* Supermarkt (Akkusativ, Bewegung)

**Error correction:**
> ❌ Er hat gestern nach Hause gegangen.
> ✓ Er ist gestern nach Hause gegangen.
> 📌 gehen → sein im Perfekt (Bewegung)

**Transform:**
> Rewrite using *obwohl*:
> Er ist müde. Er arbeitet weiter.
> → Obwohl er müde ist, arbeitet er weiter.

**Translation:**
> "She would like a coffee, please."
> → Sie hätte gern einen Kaffee, bitte. / Ich möchte einen Kaffee, bitte.

---

## Quick reference: Cases overview

| Case | Question | Definite (m/f/n/pl) | Use for |
|------|----------|---------------------|---------|
| Nominativ | Wer? Was? | der / die / das / die | Subject |
| Akkusativ | Wen? Was? | den / die / das / die | Direct object, direction |
| Dativ | Wem? | dem / der / dem / den+n | Indirect object, location |
| Genitiv | Wessen? | des+s / der / des+s / der | Possession |

---

## Adjective ending quick reference

### After definite article (der/die/das)
| | m | f | n | pl |
|--|--|--|--|--|
| Nom | -e | -e | -e | -en |
| Akk | -en | -e | -e | -en |
| Dat | -en | -en | -en | -en |
| Gen | -en | -en | -en | -en |

### After indefinite article (ein/eine/ein)
| | m | f | n | pl |
|--|--|--|--|--|
| Nom | -er | -e | -es | -en |
| Akk | -en | -e | -es | -en |
| Dat | -en | -en | -en | -en |
| Gen | -en | -en | -en | -en |

### No article (kein article)
| | m | f | n | pl |
|--|--|--|--|--|
| Nom | -er | -e | -es | -e |
| Akk | -en | -e | -es | -e |
| Dat | -em | -er | -em | -en |
| Gen | -en | -er | -en | -er |
