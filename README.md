# opencode-tools
Because i mix them up all the time...

### [netresearch/context7](https://github.com/netresearch/context7-skill)
Fetch up-to-date library documentation via Context7 REST API. Lightweight alternative to Context7 MCP with no persistent context overhead.
```
npx skills add https://github.com/netresearch/context7-skill --skill context7
```
### [DCP](https://github.com/Opencode-DCP/opencode-dynamic-context-pruning)
Automatically prunes conversation context by summarizing stale messages and deduplicating tool calls.
```jsonc
// opencode.json
{
  "plugin": ["@tarquinen/opencode-dcp@latest"]
}
```
### [DevBrowser](https://github.com/SawyerHood/dev-browser)
Skill to navigate and inspect pages during development.
```sh
git clone https://github.com/sawyerhood/dev-browser /tmp/dev-browser-skill
cp -r /tmp/dev-browser-skill/skills/dev-browser ~/.config/opencode/skills/dev-browser
rm -rf /tmp/dev-browser-skill
cd ~/.config/opencode/skills/dev-browser && npm install
```
### [opencode-claude-auth](https://github.com/griffinmartin/opencode-claude-auth)
Uses your Claude Code credentials for OpenCode — no separate login needed.
```jsonc
// opencode.json
{
  "plugin": ["opencode-claude-auth"]
}
```
### [rtk](https://github.com/rtk-ai/rtk)
CLI proxy that rewrites shell commands and filters their output before it reaches the LLM to save tokens.
```sh
curl -fsSL https://raw.githubusercontent.com/rtk-ai/rtk/refs/heads/master/install.sh | sh
rtk init -g --opencode
```
### [Superpowers](https://github.com/obra/superpowers)
Skills framework that enforces structured dev workflows (brainstorming, TDD, plans, code review) automatically.
```jsonc
// opencode.json
{
  "plugin": ["superpowers@git+https://github.com/obra/superpowers.git"]
}
```
### [Svelte](https://github.com/sveltejs/ai-tools)
Svelte 5 documentation lookup, code analysis, and autofixing.
```jsonc
// opencode.json
{
  "plugin": ["@sveltejs/opencode"]
}
```
