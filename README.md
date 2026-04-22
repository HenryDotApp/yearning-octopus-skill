# Yearning Octopus Skill

An interactive, multi-session process to help you figure out what you actually want out of life. Your AI agent plays a direct, relentless, skeptical interrogator — not a cheerleader and not a therapist — and walks you through Tim Urban's framework from ["How to Pick a Career (That Actually Fits You)"](https://waitbutwhy.com/2018/04/picking-career.html).

You have a Yearning Octopus inside you. This skill helps you map it, evict the impostor desires that someone else installed, visit Denial Prison for the parts of yourself you've locked away, rank what actually matters, then find the overlap between what you want and what's achievable.

This will be uncomfortable. That's how you know it's working.

## What it does

- **Phase 1 — Audit the Want Box**: surface all five tentacles (Personal, Social, Lifestyle, Moral, Practical), run the Why Game on each yearning to catch impostors, visit Denial Prison, then build a hierarchy (NN Bowl → Top → Middle → Bottom → Trash).
- **Phase 2 — Audit the Reality Box**: challenge inherited beliefs about what's possible, then honestly assess personal potential (Pace × Persistence).
- **Phase 3 — Find the Option Pool**: the overlap between the two boxes. Written in light pencil, as a hypothesis to test by living it.

Progress is saved to a local file (default `./life-compass-progress.md`) so you can resume across sessions.

## Install

Pick the agent you use. Each one reads `SKILL.md` from its own skills directory — cloning the repo into that directory is enough.

### Claude Code

```bash
mkdir -p ~/.claude/skills
git clone https://github.com/HenryDotApp/yearning-octopus-skill ~/.claude/skills/life-compass
```

Invoke by asking for the life compass, or with `/life-compass`.

### Claude.ai

Upload `SKILL.md` as a custom skill in your Claude.ai settings.

### OpenAI Codex CLI

```bash
mkdir -p ~/.codex/skills
git clone https://github.com/HenryDotApp/yearning-octopus-skill ~/.codex/skills/life-compass
```

Codex auto-discovers skills in `~/.codex/skills/`. Invoke by asking for the life compass.

### Cursor

```bash
mkdir -p ~/.cursor/skills-cursor
git clone https://github.com/HenryDotApp/yearning-octopus-skill ~/.cursor/skills-cursor/life-compass
```

### Any other agent

If your agent doesn't have a native skills system (Aider, Continue, Zed AI, Windsurf, etc.), paste the body of `SKILL.md` into your agent's system prompt, rules file, or project instructions. The skill is a self-contained prompt — it doesn't depend on any agent-specific tooling.

## Usage

Just start a conversation and invoke the skill. The agent will open with a brief framing, then begin Step 1. A full pass takes multiple sessions — don't rush it. If you try to intellectualize, you'll get called on it.

## Credit

The framework is Tim Urban's (Wait But Why). This skill packages it as a facilitator prompt; the ideas, terminology, and structure are his.

## License

MIT.
