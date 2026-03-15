# opencode-tools
Because i mix them up all the time...
## Context
### [rtk](https://github.com/rtk-ai/rtk)
CLI proxy that rewrites shell commands and filters their output before it reaches the LLM to save tokens.
```sh
curl -fsSL https://raw.githubusercontent.com/rtk-ai/rtk/refs/heads/master/install.sh | sh
rtk init -g --opencode
```
### [DCP](https://github.com/Opencode-DCP/opencode-dynamic-context-pruning)
Automatically prunes conversation context by summarizing stale messages and deduplicating tool calls.
```jsonc
// opencode.json
{
  "plugin": ["@tarquinen/opencode-dcp@latest"]
}
```
## Workflow
### [Superpowers](https://github.com/obra/superpowers)
Skills framework that enforces structured dev workflows (brainstorming, TDD, plans, code review) automatically.
```
Fetch and follow instructions from https://raw.githubusercontent.com/obra/superpowers/refs/heads/main/.opencode/INSTALL.md
```
## Development
### [DevBrowser](https://github.com/SawyerHood/dev-browser)
Skill to navigate and inspect pages during development.
```sh
git clone https://github.com/sawyerhood/dev-browser /tmp/dev-browser-skill
cp -r /tmp/dev-browser-skill/skills/dev-browser ~/.config/opencode/skills/dev-browser
rm -rf /tmp/dev-browser-skill
cd ~/.config/opencode/skills/dev-browser && npm install
```
### [Svelte](https://github.com/sveltejs/ai-tools)
Svelte 5 documentation lookup, code analysis, and autofixing.
```jsonc
// opencode.json
{
  "plugin": ["@sveltejs/opencode"]
}
```
