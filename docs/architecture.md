# AgentHub architecture

```text
Team members
    |
Discord server / #agenthub
    |
Switch Discord integration
    |
Switch room and shared context
    |
Switch-managed agent session
    |
Codex agent working in the AgentHub directory
```

Switch provides the Discord bridge and agent orchestration. The exact Windows onboarding screens and supported provider choices can vary by release.

A separate custom Discord bot is intentionally omitted because Switch already owns the Discord connection.
