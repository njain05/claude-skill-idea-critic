# Extra session — Creating a Skill

Nishtha Jain · CRN 2315172 · URN 2302627 · Additional session, Tue 6 Oct 2026

> An **extra class**, outside the numbered run. Session 8 proper was the
> third-party API session on Tue 22 Sep — that work is in `session8-weather/`.

---

## The homework

Create a simple Skill and demonstrate its use case. Upload a PDF to your GitHub
repo and share the URL.

The PDF must contain:

1. A short description of the Skill and what it does
2. A screenshot of the Skill's structure
3. **Screenshots comparing the output for the same prompt with the Skill turned
   OFF versus turned ON**

> *"The PDF should clearly demonstrate how the Skill improves or changes the
> output."*

## The whole grade is in the comparison

Points 1 and 2 are description. Point 3 is the evidence, and it only works if
**one variable changes**. Same prompt, same wording, same typos, run twice —
once with the Skill off, once on. If the prompt differs even slightly between
the two screenshots, the comparison proves nothing and the marker can see it.

So the Skill has to be chosen for a task where the *off* answer is visibly
inadequate. A Skill that makes a good answer slightly better photographs badly.

## Choosing a Skill worth demonstrating

The ones that show a stark before/after are those encoding knowledge Claude
cannot guess:

- **A house style or format** — without it, generic structure; with it, your
  exact sections, headings and tone, every time.
- **A checklist or review standard** — without it, vague praise; with it, the
  same specific checks every run.
- **Domain rules** — without it, a plausible answer that breaks a rule; with it,
  the rule held.

The sharpest demo is a prompt where the off version is *confidently wrong* in a
way the on version fixes.

### From your own work

Three things already in this folder's neighbourhood would make honest Skills,
because the rules are real and already written down:

| Skill | Would encode | Off vs on |
|---|---|---|
| **Business card → bot** | The Session 10 structure: facts, rules, never-do, priority enquiries | Off: a vague chatbot brief. On: a card the kit can actually consume. |
| **Client fact discipline** | Your Panwar rules — never invent a fact, mark gaps `TODO: confirm with client`, never publish a masked GST or a proxy phone number | Off: invented MOQs and lead times. On: visible TODOs where the data is missing. |
| **Prompt log entry** | The `prompt.md` format — verbatim prompt, what it produced, honest assessment, time estimate vs actual | Off: a tidy summary. On: the real prompt with its typos and a note on what didn't work. |

The second one has the best demo: ask for a supplier page for a business with
gaps in its public data. Without the Skill you get confident invented numbers.
With it, you get `TODO: confirm with client`. That difference is obvious in a
screenshot and it's a real lesson, not a formatting trick.

## Structure of a Skill

```
skill-name/
  SKILL.md        name, description, and the instructions
  (optional)      reference files the skill tells Claude to read
```

The `description` is what decides whether the Skill fires at all — it has to
name the situations that should trigger it, in the words you'd actually use.

## What goes in this folder

```
extra-session-skill/
  README.md           this file
  skill/              the Skill itself
  evidence/           the off and on screenshots
  Skill-Demo.pdf        the submission
```

## Before you submit

- Same prompt in both screenshots, word for word
- The structure screenshot shows `SKILL.md`, not just a folder name
- The difference is visible without reading closely
- PDF in the repo, and the URL shared
