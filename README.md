# AI Project Idea Critic — a Claude Skill

Nishtha Jain · CRN 2315172 · URN 2302627
Built in the additional session, Tue 6 Oct 2026

A Skill that evaluates a project idea instead of praising it. It scores the idea
against a six-point rubric, says plainly whether it is worth building, and hands
back a reshaped stronger version — as a scorecard page rather than a chat reply.

---

## The Skill

```
skill/ai-project-idea-critic/
  SKILL.md                  name, description, and the instructions
  references/rubric.md      the six scoring criteria, read at step 2
```

**What it does.** When someone shares a project idea, the Skill makes Claude:

1. Score it against six criteria — problem, AI necessity, originality,
   feasibility, data availability, portfolio value
2. Give a verdict: **Weak**, **Promising** or **Strong**
3. State what would have to be true for it to be worth building
4. Propose a named, scoped, reshaped version
5. Make the call: **Build / Reshape / Drop**
6. Render all of it as a shareable scorecard artifact
7. **Stop there** — no implementation unless asked

Two guardrails are written into it: *judge the idea, never the person*, and
*the verdict follows the evidence* — a genuinely strong idea gets a strong
verdict. It is an evaluator, not a no-machine.

## Why this one demonstrates well

The homework wants the same prompt run twice, Skill off and Skill on, with a
visible difference.

Default behaviour is the problem this Skill was built for: share an idea and
Claude tends to accept it and start describing how to build it. The Skill
replaces that with a scored judgement and a reshaped alternative.

So the difference is **structural**, not stylistic — a chat reply versus a
scored scorecard page. That reads clearly in a screenshot.

---

## The demo

**Use exactly this prompt, both times. Word for word.**

> I want to build an AI chatbot for my college canteen that answers questions about the menu.

It is deliberately a generic idea, because generic is where the two behaviours
diverge most.

| | Expected |
|---|---|
| **Skill OFF** | Encouragement, then a tech stack and a build plan. No judgement on whether it is worth building. |
| **Skill ON** | Verdict (likely **Weak**), six scores out of 5, what would have to be true, a reshaped version, and Build/Reshape/Drop. Plus the scorecard artifact. |

### Screenshots needed

Save into `evidence/`:

| File | What it shows |
|---|---|
| `01-structure.png` | The Skill's structure — `SKILL.md` and `references/rubric.md` visible, not just a folder name |
| `02-skill-off.png` | The prompt and Claude's answer, Skill disabled |
| `03-skill-on.png` | The same prompt and Claude's answer, Skill enabled |

**The whole demonstration rests on one variable changing.** Same prompt, same
wording, same punctuation. If the two prompts differ, the comparison proves
nothing and it is visible to anyone reading.

Turn the Skill off at Settings → Capabilities → Skills, run the prompt, turn it
back on, run it again in a fresh chat.

---

## Submission

The form asks for a **GitHub repo containing the Skill documentation PDF and the
Skill file**.

```
extra-session-skill/
  README.md                      this file
  skill/ai-project-idea-critic/  the Skill
  evidence/                      the three screenshots
  Skill-Demo-Nishtha-Jain.pdf    the documentation PDF
```

The PDF needs a short explanation, the structure screenshot, and the before and
after screenshots — enough to show how the Skill changes the output.
