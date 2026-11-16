# notifications

my local omapager-derived notification service and bar widget. it is separate from the hokum sample cards in the terminal section.

## files

- [the complete exported fork](https://github.com/Algorant/dotfiles/tree/main/home/.config/omarchy/plugins/algorant.notifications): keep `Service.qml`, `Widget.qml`, supporting qml/js and `bin/` together.
- [the bar clone](https://github.com/Algorant/dotfiles/tree/main/home/.config/omarchy/plugins/algorant.bar) provides the centre-reveal api used by the indicator.
- helpers use python; remote-icon normalisation uses pillow. optional integrations include bubblewrap, wl-clipboard and kde connect. share detection uses the hyprland desktop portal.
- notification state stays on the machine. it is not part of the exported clone.

the source fork still contains upstream install instructions for a different plugin id. those install upstream omapager, not this local fork; use this page's source links as the reference.

no matching screenshot is included yet. a hokum card is not proof of this plugin's ui.

[back to the guide](../../README.md)
