# Reading data model

Use plain UTF-8 Markdown so the archive stays portable and user-editable.

## Layout

```text
read-mentor-data/
├── profile.md
├── index.md
├── reviews.md
└── books/
    └── <short-title>/
        ├── overview.md
        ├── concepts.md
        └── sessions.md
```

Create `profile.md` with the user's reading goals, interests, preferred difficulty, and only explicitly known reading history. Use `index.md` as a concise book list with status and last session date. Use `reviews.md` as the single review queue.

## Book overview

Include title, author, edition/translation if known, status, start/finish dates, user's purpose, pre-reading knowledge, central question, one-sentence thesis in the user's own words, argument skeleton, and unresolved questions. Mark unknown metadata as unknown rather than guessing.

## Concepts

For each concept store:

- name and the user's formulation;
- status: `new | fragile | developing | durable`;
- evidence: dated retrieval, explanation, example, counterexample, comparison, or transfer;
- misconception or uncertainty;
- links to other books/concepts, each labeled `user-observed`, `text-explicit`, or `mentor-inferred`;
- next test.

Do not promote to `durable` without at least one delayed, unaided retrieval and one explanation or transfer example.

## Sessions

Append a dated section containing mode, portion read, user's raw answer, mentor diagnosis, hint/explanation given, corrected restatement, concepts updated, and next action. Preserve meaning and label paraphrases; never present a polished mentor rewrite as the user's answer.

## Review queue

Use a Markdown table:

```markdown
| due | book | concept | prompt | interval | last_result |
|---|---|---|---|---:|---|
| 2026-08-16 | 论持久战 | 三阶段 | 不看笔记解释为何相持阶段是枢纽 | 1 | new |
```

Keep prompts generative. Avoid answers embedded in the question. When multiple reviews are overdue, choose up to three by fragility and importance rather than dumping the entire queue.
