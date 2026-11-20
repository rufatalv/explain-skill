# explain

An [Agent Skill](https://agentskills.io) that explains code, a flow, a task or a concept in ASD-STE100 (Simplified Technical English) style. The layout is for readers with ADHD: TL;DR first, short active sentences, bullets and tables.

It works with any agent that supports Agent Skills, for example Claude Code, Codex, Cursor and Gemini CLI.

## Install

```sh
npx skills add rufatalv/explain-skill
```

- The CLI asks which agents to install the skill for.
- Add `-g` to install it for your user, not only for the current project.
- Add `-a <agent>` to pick the agents without the prompt.

## Use

- Type `/explain <what to explain>` if your agent supports slash commands.
- Or ask your agent to "explain" or "walk me through" something.

See [skills/explain/SKILL.md](skills/explain/SKILL.md) for the full rules.

## License

[MIT](LICENSE)
