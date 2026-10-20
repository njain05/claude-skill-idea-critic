# Rubric: six criteria

Score each criterion 0-5. Add them for a total out of 30, then map to a verdict:
- **0-13 -> Weak**
- **14-22 -> Promising**
- **23-30 -> Strong**

Give each score a one-line justification grounded in the specific idea, not a
generic sentence. Be willing to give a 1 and willing to give a 5.

## 1. Problem (real pain?)
- 5: a sharp, specific problem a known group feels often and would pay or switch for.
- 3: a real but broad problem many tools already address.
- 1: a vague "wouldn't it be nice" with no clear sufferer.
Folds in: who the target users actually are.

## 2. AI necessity (does it need AI?)
- 5: the core value is impossible or far worse without ML/LLMs.
- 3: AI helps but a non-AI version would still be useful.
- 1: AI is bolted on for buzz; a simple rules/CRUD app would do the same job.
Challenge this hard - most weak ideas fail here.

## 3. Originality (differentiated?)
- 5: a genuinely new angle, or a well-worn space attacked from a fresh direction.
- 3: a familiar idea with one distinguishing twist.
- 1: "an AI chatbot for X" with nothing separating it from dozens of clones.
Folds in: differentiation from existing solutions.

## 4. Feasibility (buildable by this maker?)
- 5: a student could ship a real version in the available time with available skills.
- 3: ambitious; the full version is a stretch but a meaningful slice is reachable.
- 1: needs data, scale, or expertise the maker almost certainly cannot get.

## 5. Data (is the needed data available?)
- 5: the data exists, is accessible, and is legal/ethical to use.
- 3: data is partly available or needs real effort to collect.
- 1: depends on data that is private, tiny, or does not exist.

## 6. Portfolio value (does it prove skill?)
- 5: building it demonstrates real engineering an employer would notice.
- 3: a solid but common portfolio piece.
- 1: a tutorial-level clone that signals little.
Folds in: technical depth.

## Worked example (for calibration)

Idea: "An AI chatbot for college students that answers questions about their
courses, assignments, and exams."
- Problem 2 - broad; students already have syllabi, email, and search.
- AI necessity 2 - mostly retrieval + generation; a good FAQ/search would cover much of it.
- Originality 1 - academic RAG assistants already exist; nothing differentiates this.
- Feasibility 4 - a basic RAG bot is genuinely buildable by a student.
- Data 3 - course material is available but scattered and per-institution.
- Portfolio value 2 - a RAG-over-docs clone is common and signals little depth.
Total 14 -> **Promising** by the numbers, but flag that it sits at the bottom of
that band and is weak on the dimensions that matter most (originality, AI necessity).

Reshaped version to offer: an **Academic Risk & Intervention Assistant** that
joins deadlines, attendance, and performance to flag students at risk and suggest
specific interventions - a sharper problem, real AI justification, and clear
differentiation.
