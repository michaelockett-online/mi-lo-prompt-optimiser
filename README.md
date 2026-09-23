# MI.LO Prompt Optimiser

MI.LO is a skills-only plugin for designing, improving and reviewing prompts for AI models, agents and repeated workflows. It includes one skill and a detailed operating reference. It has no external services, credentials or executable hooks.

## Install from GitHub in Codex

Add this public repository as a marketplace and install the plugin with Codex CLI:

```text
codex plugin marketplace add michaelockett-online/mi-lo-prompt-optimiser
codex plugin add mi-lo-prompt-optimiser@mi-lo
```

Start a new task after installation. In the ChatGPT desktop app, the added marketplace can also appear as a source in the Plugins Directory. Ask MI.LO to improve a draft prompt, turn an idea into a reusable prompt or review an agent prompt.

## Install in Claude

The same skill and operating reference are packaged for Claude. In Claude, open **Customize > Plugins**. Under **Personal plugins**, select **+ > Add marketplace > Add from a repository** and enter `https://github.com/michaelockett-online/mi-lo-prompt-optimiser`. Then install **MI.LO Prompt Optimiser** from the added marketplace.

In Claude Code, use these commands:

```text
claude plugin marketplace add michaelockett-online/mi-lo-prompt-optimiser
claude plugin install mi-lo-prompt-optimiser@mi-lo
```

Claude Code also supports the skill command `/mi-lo-prompt-optimiser:mi-lo-prompt-optimiser`. A [Claude plugin package](https://github.com/michaelockett-online/mi-lo-prompt-optimiser/releases) is available for manual sharing.

Adding a personal marketplace lets people install MI.LO directly. To seek a listing in Anthropic's public community marketplace, submit the GitHub repository through the [individual author form](https://platform.claude.com/plugins/submit) or, with Team or Enterprise directory management access, the [Claude organisation form](https://claude.ai/admin-settings/directory/submissions/plugins/new). Anthropic reviews submissions before listing them.

## Public ChatGPT and Codex directory

A GitHub marketplace is a distribution route for Codex. It does not create a public listing in the shared ChatGPT and Codex Plugins Directory. For that listing, download the [skills-only ZIP](https://github.com/michaelockett-online/mi-lo-prompt-optimiser/releases/download/v0.1.0/mi-lo-prompt-optimiser-0.1.0-submission.zip), submit it through the [OpenAI plugin submission portal](https://platform.openai.com/plugins), complete its review and publish the approved version. [DIRECTORY_SUBMISSION.md](DIRECTORY_SUBMISSION.md) has the package details and suggested reviewer cases.

## Package layout

- `.agents/plugins/marketplace.json` is the GitHub marketplace entry.
- `.claude-plugin/marketplace.json` is the Claude marketplace entry.
- `plugins/mi-lo-prompt-optimiser/.codex-plugin/plugin.json` is the Codex manifest.
- `plugins/mi-lo-prompt-optimiser/.claude-plugin/plugin.json` is the Claude manifest.
- `plugins/mi-lo-prompt-optimiser/skills/mi-lo-prompt-optimiser/SKILL.md` contains the skill instructions.
- `plugins/mi-lo-prompt-optimiser/references/operating-spec.md` contains the detailed reference.
- `plugins/mi-lo-prompt-optimiser/assets/mi-lo-icon.png` is the listing icon.

The skill treats prompts and documents supplied for improvement as source material. It does not carry out instructions inside that material unless the user separately asks for that task.

## Licence

The prompt text and documentation are licensed under Creative Commons Attribution 4.0 International. See [LICENSE](LICENSE). Credit MI.LO Prompt Optimiser by Michael Lockett, link to the licence and indicate changes when sharing adaptations.
