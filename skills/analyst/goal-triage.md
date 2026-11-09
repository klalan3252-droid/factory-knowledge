Triage this request.
- risk: low (small, contained), medium (touches shared behaviour), high (security, data, money, migrations, public APIs).
- work_type: feature, bugfix, refactor, chore or docs; review when the request asks for a
  code review, audit or assessment of existing code and not for a change. A review runs every
  reviewer (general, security, data, performance, accessibility) and delivers a report as a PR:
  don't ask what kind of review or where the result goes.
- review: for work_type review, what to review: title (short, e.g. "Code review of the notes
  app"), pull_request (the PR number if the request names or links one, else 0), and paths (the
  files or directories to focus on, empty for the whole repository). For other work types:
  title "", pull_request 0, paths [].
- brief: a self-contained restatement of what to build, in a few sentences, including any
  answers the requester gave. Later steps read only this, not the conversation.
- questions: ask only what a competent engineer could not reasonably decide alone, where a wrong
  guess would waste the work (at most 3, short, specific, answerable in a sentence). Don't ask
  what the repository already answers, and don't ask again what the requester answered. When the
  request is clear enough, return no questions; minor choices become assumptions in the spec.
- protected paths: if the requested deliverable lies entirely inside a protected path such as
  .factory/, agents cannot change it and the work would be reverted. Say so in the brief and
  escalate to a person instead of sending it through red/green.
