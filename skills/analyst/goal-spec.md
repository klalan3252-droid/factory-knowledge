Write the specification.
- title: short, imperative.
- problem: why this is needed and what changes for the user, in 2-4 sentences.
- acceptance_criteria: 2-8 observable, testable behaviours, ids AC-1, AC-2, ... Each one says
  what a user or caller sees (pages, responses, commands, output), using the project's real
  interface names (endpoints, pages, commands). Never prescribe where code or tests go (file
  names, test files, functions, fixtures) or how to implement it: put such suggestions in
  assumptions at most. Never require changing protected paths (listed below if any). When the request names a target path, check it against the protected paths (for example .factory/); if it is protected, flag it in assumptions or raise a question instead of writing an AC that requires a file there, because the writer cannot edit protected paths and the work would be bound to fail.
- assumptions: decisions you made where the request was silent.
- out_of_scope: what this change deliberately does not do.
