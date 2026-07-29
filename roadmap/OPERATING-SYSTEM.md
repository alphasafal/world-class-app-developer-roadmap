# Learning and Building Operating System

## Daily loop (3–5 focused hours)

1. **Frame (10 min):** user-visible outcome, acceptance criteria, constraints and non-goals.
2. **Understand (30–45 min):** official documentation; write a plain-language mental model.
3. **Attempt (60–120 min):** implement the critical part before asking AI for a full solution.
4. **Inspect (20 min):** review every generated diff and explain important functions and tradeoffs.
5. **Verify (30–60 min):** unit first, then integration/E2E; test invalid inputs and degraded states.
6. **Ship (20 min):** README, evidence, limitations, journal and commit.
7. **Teach back (10 min):** explain the architecture without opening the code.

## AI rules

- AI may teach, critique, test and pair-program. It may not replace your ability to explain.
- Write your prediction before requesting code.
- Never accept a generated dependency, security claim or performance claim without verification.
- Every seventh day is a no-AI reconstruction of a critical module.
- Keep an “AI mistakes” section in every journal entry.

## Project structure

Use `projects/day-XXX-short-name/` for focused builds. A later day may extend an earlier product, but it must deliver a distinct tested outcome. Large weekly releases can live in their own repositories and be linked from the journal.

## Git discipline

- Branch: `day-XXX-short-name`
- Commit: `day-XXX: outcome`
- Pull request includes acceptance criteria, screenshots/traces, test commands, risks and self-review.
- Protect `main`; require CI. Never commit secrets.

## Anti-burnout constraint

Do not attempt 18-hour days. Sustainable deliberate practice, sleep, exercise and weekly recovery outperform short bursts. Minimum viable day: one bounded 90-minute build plus evidence. Never fake a completion streak.
