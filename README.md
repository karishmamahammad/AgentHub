# AgentHub — Custom AI teammate for Discord

AgentHub is a hackathon starter for a helpful AI teammate in a Discord room using Switch and a Codex agent.

## Architecture
Discord ↔ Switch Discord integration ↔ Switch room ↔ Codex agent session

Switch handles the Discord connection and agent orchestration. This starter provides project instructions, skills, workflows, and demo prompts. It does not create a separate Discord bot because that would duplicate Switch's integration.

## Setup outline
1. Install Docker Desktop and confirm its WSL 2 backend works.
2. Install Switch Console from https://github.com/sandbox-quantum/switch and follow its current onboarding.
3. Create an agent in Switch Console using Codex as the provider, if available in your installed version.
4. Set the agent's working directory to this extracted AgentHub folder.
5. Connect a private Discord test server/channel through Switch Console.
6. Use `agent/AGENTS.md` as the agent's instructions.
7. Test using `docs/test-prompts.md`.

## Codex CLI (optional development helper)
In PowerShell:
```powershell
npm install -g @openai/codex
codex
```
Sign in when prompted.

## Safety
- Never commit API keys, bot tokens, passwords, or `.env` files.
- Start in a private Discord test server and allowlist trusted users.
- Do not allow unrestricted shell access to a public Discord room.
- Require approval before destructive actions, deployments, purchases, or external messages.
- Review generated code before running it.

## Demo
Show AgentHub explaining a code error, turning a feature request into tasks, reviewing code, and summarizing a team discussion.
