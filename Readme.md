# Keybinding Plugin
The code in this plugin is mostly copied from: https://github.com/godotengine/godot-demo-projects/tree/master/gui/input_mapping.

The keymap will be saved to the user directory.
```
Win: %APPDATA%/<Project Name>
Linus, macOS: ~/.local/share/godot/app_userdata/<Project Name>
```

## Setup
- implement your own keybinding menu (addons/keybinding_menu can be used as a reference)
	- the translation file (addons/keybindings/localisation/keybind_menu_strings.en.translation) for the example menu has to be added manually to work (Project Settings > Translations)

## Note:
- the Directory of the keymap might not be the project name, if a custom user dir was set
	- Advanced Settings must be enabled to view "Use Custom User Dir"
	- Project Settings > General > Application > Config > Use Custom User Dir
- right now this plugin only cares about the primary binding and ignores the rest
- potentially it might remove additional bindings
	- has to be checked