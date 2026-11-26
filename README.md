# Mobilint Skills

[Agent Skills](https://agentskills.io/) for building on the Mobilint NPU SDK.

## Installing

### Claude Code

Install using the [plugin marketplace](https://code.claude.com/docs/en/plugins/install#add-a-marketplace):

```sh
claude plugin marketplace add mobilint/skills
claude plugin install mobilint@mobilint
```

Or run `/plugin` inside Claude Code.

To get updates automatically, run `/plugin`, open **Marketplaces**, select **mobilint**, and enable auto-update.

### Codex

Install from the Mobilint plugin marketplace:

```sh
codex plugin marketplace add mobilint/skills
codex plugin add mobilint@mobilint
```

### npx skills

Install using the [`npx skills`](https://skills.sh) CLI:

```sh
npx skills add mobilint/skills
```

### Clone / Copy

Clone this repo and copy the skill folders into the appropriate directory for your agent:

| Agent | Skill Directory | Docs |
|-------|-----------------|------|
| Claude Code | `~/.claude/skills/` | [docs](https://code.claude.com/docs/en/skills) |
| OpenCode | `~/.config/opencode/skills/` | [docs](https://opencode.ai/docs/skills/) |
| OpenAI Codex | `~/.codex/skills/` | [docs](https://developers.openai.com/codex/skills/) |

## Updating

Codex updates the plugin automatically. To update manually:

Claude Code:

```sh
claude plugin marketplace update mobilint
claude plugin update mobilint@mobilint
```

Codex:

```sh
codex plugin marketplace upgrade mobilint
```

npx skills:

```sh
npx skills update
```

## Skills

Skills are contextual and auto-loaded based on your conversation. When a request matches a skill's triggers, the agent loads and applies the relevant skill.

| Skill | Useful for |
|-------|------------|
| mobilint-sdk | Answering Mobilint NPU SDK questions from Mobilint's official docs and forum |

## Usage

Example prompts:

```
How do I compile my ONNX model for a Mobilint NPU?
```

```
Which driver and firmware versions does my SDK version need?
```

```
My model fails to load on the device with this error: <log>
```

In Claude Code, `/mobilint:mobilint-sdk` invokes the skill directly.

## License

Apache-2.0. See [LICENSE](LICENSE).
