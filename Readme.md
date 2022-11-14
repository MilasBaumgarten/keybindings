# Keybinding Plugin
The code in this plugin is mostly copied from: https://github.com/godotengine/godot-demo-projects/tree/master/gui/input_mapping.
It was mostly just adjusted to work with Godot 4.

The keymap will be saved to the user directory.
```
Win: %APPDATA%/<Project Name>
Linus, macOS: ~/.local/share/godot/app_userdata/<Project Name>
```

## Note:
- the Directory of the keymap might not be the project name, if a custom user dir was set
	- Advanced Settings must be enabled to view "Use Custom User Dir"
	- Project Settings > General > Application > Config > Use Custom User Dir
- right now this plugin only cares about the primary binding and ignores the rest
- potentially it might remove additional bindings
	- has to be checked