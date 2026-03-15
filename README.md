# opencode-tools
Because i mix then up all the time...

## Context
### rtk (rust token killer)
#### Install
```
curl -fsSL https://raw.githubusercontent.com/rtk-ai/rtk/refs/heads/master/install.sh | sh
rtk init -g --opencode
```
#### Link
https://github.com/rtk-ai/rtk

### DCP (Dynamic Context Pruning Plugin)
#### Install
``` yaml
// opencode.json
{
    "plugin": ["@tarquinen/opencode-dcp@latest"],
}
```
#### Link
https://github.com/Opencode-DCP/opencode-dynamic-context-pruning


## Agents
### Superpowers
#### Install
```
Fetch and follow instructions from https://raw.githubusercontent.com/obra/superpowers/refs/heads/main/.opencode/INSTALL.md
```
#### Link
https://github.com/obra/superpowers

## Coding
### DevBrowser
#### Install
```
git clone https://github.com/sawyerhood/dev-browser /tmp/dev-browser-skill
cp -r /tmp/dev-browser-skill/skills/dev-browser ~/.config/opencode/skills/dev-browser
rm -rf /tmp/dev-browser-skill
cd ~/.config/opencode/skills/dev-browser && npm install
```
#### Link
https://github.com/SawyerHood/dev-browser
### Svelte
#### Install
``` yaml
// opencode.json
{
  "plugin": ["@sveltejs/opencode"]
}
```
#### Link
https://github.com/sveltejs/ai-tools
