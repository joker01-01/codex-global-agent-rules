# Codex Global Agent Rules

A practical global `AGENTS.md` for disciplined Codex work: inspect before editing, stay within scope, prefer the smallest coherent implementation, verify real outcomes, and require explicit authorization for consequential actions.

This is an opinionated working agreement, not a prompt claiming to fit every team. Project-level `AGENTS.md` files remain more specific and take precedence.

## What it covers

- Instruction precedence between global and project rules
- Scope control and safe autonomy
- Evidence-based inspection instead of guessing
- A minimal-implementation decision ladder
- Visible failures instead of silent fallbacks
- Focused verification and clear stopping conditions
- Subagent coordination boundaries
- Git and destructive-action safeguards
- Concise, factual communication
- Rules for maintaining the instruction file itself

## Install for Codex

Back up any existing global rules, then place [`AGENTS.md`](./AGENTS.md) at:

```text
~/.codex/AGENTS.md
```

Review and adapt the rules before using them. Keep repository-specific language, commands, frameworks, and policies in each project's own `AGENTS.md`.

## Minimal implementation ladder

After understanding the task and tracing the affected flow, the agent should choose the first option that fully satisfies the requirement:

1. Make no code change when the outcome already exists.
2. Reuse an existing project helper or pattern.
3. Use the standard library.
4. Use a native platform capability.
5. Use an already-installed dependency.
6. Make the smallest clear local change.
7. Only then add new code or a new dependency.

The goal is not code golf. Readability, relevant edge cases, validation, safety, and the user's explicit requirements still win.

## License

[MIT](./LICENSE)
