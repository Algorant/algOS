# bar

my clone of omarchy's bar keeps the centre group as one hover unit, including the clock and adjacent indicators.

## files

- [the complete bar clone](https://github.com/Algorant/dotfiles/tree/main/home/.config/omarchy/plugins/algorant.bar): `Bar.qml`, `BarModel.js`, `widgets/` and `indicators/` stay together.
- [console](../console/README.md) and [notifications](../notifications/README.md) consume its shared centre-reveal properties.
- the source declares `clonedFrom: omarchy.bar`. omarchy's quickshell modules and the machine's own shell layout are still required.

the trigger is the centre group plus roughly 40 pixels on each side, held steady while open. it replaces the upstream left-of-clock peek zone; it is not an extra widget layered over the clock.

clone built-in plugins with omarchy's supported plugin-clone workflow; don't patch the packaged files. adapt your layout to use the clone rather than copying somebody else's entire shell settings.

[back to the guide](../../README.md)
