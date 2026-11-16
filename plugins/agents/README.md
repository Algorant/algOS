# agents

account quota and this machine's token history on the bar. the panel has codex, claude, grok and opencode tabs.

## files

- [the complete exported clone](https://github.com/Algorant/dotfiles/tree/main/home/.config/omarchy/plugins/algorant.agents): `manifest.json`, `Panel.qml`, `Main.qml` and `bin/` belong together.
- collectors use node, python and omarchy's agent-usage helpers. the panel needs omarchy's quickshell ui modules.
- provider authentication and collected usage are machine-local state, not files to copy from somebody else's setup. cross-machine aggregation is optional.

this is my local panel, not just a theme applied to the stock one. adapt the collector/provider choices to your own accounts.

[back to the guide](../../README.md)
