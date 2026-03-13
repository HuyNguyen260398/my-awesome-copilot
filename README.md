# My Awesome Copilot

> A curated collection of GitHub Copilot agents, instructions, prompts, and skills for VS Code.

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

This repository is a personal collection of GitHub Copilot customization resources for VS Code. Most resources are sourced from the [awesome-copilot](https://github.com/github/awesome-copilot) community repository; others are self-created to address specific workflows and use cases.

## What's Included

The collection is organized following the VS Code GitHub Copilot extension folder conventions under `.github/`:

| Folder | Description |
|---|---|
| `.github/agents/` | Custom agent modes (`.agent.md`) that define specialized AI personas and tool configurations |
| `.github/instructions/` | Coding instructions (`.instructions.md`) that guide Copilot's behavior for specific languages, frameworks, or tasks |
| `.github/prompts/` | Reusable prompt files (`.prompt.md`) for common development workflows |
| `.github/skills/` | Skill bundles (`SKILL.md`) that package domain-specific knowledge and workflows |

## Getting Started

### Using resources from this collection

1. **Clone or download** this repository.
2. **Copy** the desired files from `.github/agents/`, `.github/instructions/`, `.github/prompts/`, or `.github/skills/` into your project's `.github/` folder.
3. **Open the project** in VS Code with the [GitHub Copilot](https://marketplace.visualstudio.com/items?itemName=GitHub.copilot) extension installed.

GitHub Copilot will automatically pick up the customization files from the `.github/` folder in your workspace.

> [!TIP]
> You can also place instruction files in your VS Code user profile folder (`~/.config/github-copilot/`) to apply them globally across all workspaces.

### Resource types at a glance

**Agents** (`.agent.md`) define a complete Copilot agent mode — including its description, tools it can use, and any associated instructions. Agents appear in the Copilot Chat model picker.

**Instructions** (`.instructions.md`) provide persistent context to Copilot, such as coding conventions, preferred libraries, or project-specific constraints. They are automatically applied based on `applyTo` glob patterns in the file's frontmatter.

**Prompts** (`.prompt.md`) are reusable, parameterizable prompts that can be invoked directly from Copilot Chat using `/` commands.

**Skills** (`SKILL.md`) are structured knowledge files that instruct Copilot on how to perform a specific task with best-practice guidance. They are loaded by an agent when relevant to the current request.

## Contributing

Contributions are welcome! If you have a useful agent, instruction, prompt, or skill to share:

1. Fork the repository.
2. Add your file to the appropriate folder under `.github/`.
3. Include a brief comment at the top of the file describing its purpose.
4. Open a pull request.

> [!NOTE]
> When submitting resources originally from [awesome-copilot](https://github.com/github/awesome-copilot) or other community sources, please retain the original attribution in the file header.

## Resources

- [GitHub Copilot documentation](https://docs.github.com/en/copilot)
- [VS Code Copilot customization guide](https://code.visualstudio.com/docs/copilot/copilot-customization)
- [awesome-copilot](https://github.com/github/awesome-copilot) — the community repository this collection draws from
