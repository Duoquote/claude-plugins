# duoquote's Claude Code plugins

## lead — the Lead output style

Claude Code leads a small team: it does small things itself, sends one builder phase by phase (the next phase to the same agent), uses a reader or two for lookups, and keeps the queue in its task list so nothing is lost across compactions. At the first agent of a session it asks which models to use; unanswered, the builder runs on Opus at xhigh and readers on Haiku at xhigh.

Install:

```
claude plugin marketplace add duoquote/claude-plugins
claude plugin install lead@duoquote
```

Then turn it on with `/output-style` → `lead:Lead`, or add `"outputStyle": "lead:Lead"` to `~/.claude/settings.json`. It applies from the next new session.

Update: `claude plugin update lead@duoquote`.
