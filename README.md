# build-control

The weekly build budget shared by every project's runner (docs/process.md section 12 in each project).

- budget.json: the weekly limit in tokens, the warning percentage, and an optional override end time. While
  weekly_limit_tokens is null, usage is recorded but nothing is held.
- usage.jsonl: one line per finished build session, appended by the runners. Never edited by hand.

Written by: the runners (usage.jsonl), the chat session and Command Center (budget.json). The week resets Monday
2:00 AM Eastern.
