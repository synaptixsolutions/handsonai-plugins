# Hands-on AI Plugins

AI plugins for builders — agents, skills, and prompts from [handsonai.info](https://handsonai.info).

> [!CAUTION]
> Plugins can execute code and access external services. Review plugin contents before installing. Anthropic does not control what files or software are included in third-party plugins and cannot verify that they work as intended.

## Plugins

| Plugin | Description | Components |
|--------|-------------|------------|
| **business-first-ai** | The Business-First AI Framework — analyze AI opportunities, deconstruct workflows, and build AI-powered workflows | 1 agent, 3 skills |
| **ai-workflow-examples** | Working examples of AI workflows — executive writing, editorial review, research, meeting prep, AI news, and portable prompts | 7 agents, 2 skills, 3 prompts |
| **ai-registry** | Name, document, register, and sync your AI workflows and skills | 5 skills |
| **agentic-coding** | Define requirements before you build — structured Vision Briefs and PRDs with user stories, acceptance criteria, and GitHub issue tracking | 2 skills |

## Installation

### Add the marketplace

Register this marketplace so your tool knows where to find plugins. You only need to do this once.

**Claude Code / Cursor / VS Code:**

```
/plugin marketplace add jamesgray-ai/handsonai-plugins
```

**Cowork:** Click **+** > **Add plugins...** > **Add by URL** and enter `https://github.com/jamesgray-ai/handsonai-plugins.git`

### Install a plugin

```
/plugin install business-first-ai@handsonai-plugins
```

Replace `business-first-ai` with any plugin name from the table above.

## Structure

```
.claude-plugin/
  marketplace.json        # Marketplace manifest
plugins/
  <plugin-name>/
    .claude-plugin/
      plugin.json          # Plugin metadata
    agents/                # Agent definitions (.md)
    skills/                # Skill directories (SKILL.md + references/)
```

## Documentation

- [Plugin Marketplace](https://handsonai.info/use-the-cookbook/build/) — browse plugins with usage examples
- [Using Plugins](https://handsonai.info/use-the-cookbook/build/using-plugins/) — installation, usage, and troubleshooting
- [Plugin Documentation](https://code.claude.com/docs/en/plugins) — official plugin format reference
