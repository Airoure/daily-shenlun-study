---
name: daily-shenlun-study
description: Daily Shenlun practice workflow for Chinese civil-service application essay preparation. Use when the user wants daily Shenlun study, current-affairs material collection, configurable official source selection, material-to-question conversion, timed answer practice, answer review, scoring feedback, weak-point tracking, durable study records, or next-day Shenlun planning. Also use when the user says to start today's Shenlun practice, collect the latest Shenlun materials, review a Shenlun answer, or continue prior Shenlun study.
---

# Daily Shenlun Study

Use Chinese by default for replies, comments, questions, feedback, and records.

## Core Contract

Run one daily Shenlun loop:

1. Continue from the learner's latest record.
2. Collect current material from configured sources.
3. Select one theme and one practice task.
4. Let the learner answer before showing the reference answer.
5. Review the answer with concrete scoring feedback.
6. Persist today's record and next session.

Do not default to user-provided materials. The default behavior is to collect current material from configured sources. If web access is unavailable, say so and either use cached/user-provided material or ask whether to continue with generated drill material.

## Configurable Sources

Read `references/sources.md` before collecting material. Treat that file as the source configuration and selection guide.

Default source pool:

- State Council policy document library
- China Government Network policy interpretation
- People's Daily Renmin Shiping
- Banyuetan
- National Bureau of Statistics
- Ministry of Agriculture and Rural Affairs rural revitalization and governance cases

Use only enabled sources unless the user explicitly asks to add another source. If the user asks to change the source set, update the session behavior from their instruction; only edit `references/sources.md` when asked to permanently change the skill.

## Daily Collection Rules

Collect 3-5 items per session:

1. One policy item.
2. One commentary item.
3. One grassroots or rural governance case.
4. One data item when useful.
5. One optional local practice item only if it improves the theme.

Prefer items from the last 30 days. If too little relevant material exists, expand to the last 90 days and state that expansion. Always cite source links for collected current material.

Reject material that is:

- mostly ceremonial or meeting-only with no policy, problem, case, or data;
- too broad to support a focused practice question;
- from an unreliable repost when an official or primary source is available.

## Material Processing

For each candidate item, extract:

- theme;
- policy keywords;
- public problem;
- causes or constraints;
- measures or mechanisms;
- data or factual evidence;
- reusable Shenlun expression;
- suitable question type.

Then choose one daily theme. Do not overwhelm the learner with all collected material.

Daily output before practice should be compact:

```text
Today theme: ...
Sources: ...
Material summary: ...
Keywords: ...
Question type: ...
Practice question: ...
Answer requirement: ... Chinese characters, suggested ... minutes
```

Do not provide the model answer before the learner answers unless the user explicitly asks for explanation mode.

## Practice Modes

Choose the smallest useful mode:

- 20 minutes: point extraction or answer outline.
- 45-60 minutes: one short answer plus review.
- 90 minutes: one full answer, review, and targeted rewrite.

Supported question types:

- summary and categorization
- comprehensive analysis
- countermeasure proposal
- official document writing
- argumentative essay

When no learning record exists, assume a 45-60 minute general Shenlun session unless the user states a different time.

## Review Standard

Read `references/rubrics.md` when reviewing an answer or producing a scoring explanation.

Review with this Chinese structure:

```text
Score band: ...
Core judgment: ...

Main deductions:
- ...

Priority revisions:
1. ...
2. ...

Minimal revision based on the learner's answer:
...

Reference answer:
...

Next step:
...
```

Use approximate practice scores only. Do not claim official scoring certainty.

## Study Record

Persist progress after every meaningful session. Use `assets/daily-record-template.md` as the structure.

Search for an existing record before starting from scratch:

1. Known Obsidian or study directories from conversation context.
2. Current workspace Markdown files.
3. Files whose names or headings include `shenlun`, `daily study`, `practice record`, or Chinese equivalents for Shenlun and study/practice records.

If no record exists, create `shenlun-daily-record.md` in the current workspace unless the user names another path. If writing outside the permitted workspace is required, request permission.

Record these fields every day:

- date;
- selected sources and links;
- theme;
- question type;
- task;
- learner answer summary;
- score band;
- main weak point;
- reusable method or expression;
- next session.

Make `Next session` specific, for example: `rewrite the second countermeasure paragraph in 180 Chinese characters`, not `keep practicing`.

## Teaching Rules

- Keep interaction exam-oriented and concrete.
- Ask for learner output early.
- Teach only the rule needed for today's mistake.
- Give one focused next task, not a full curriculum.
- Distinguish source-backed facts from inference.
- Avoid fabricated official questions, official model answers, or policy facts.
