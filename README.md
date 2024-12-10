# Godot 4 VS Code Theme

This Visual Studio Code theme is inspired by the Godot 4 editor, aiming to provide a similar look and feel to facilitate a seamless transition between the two environments.

> **Note:** This theme offers syntax highlighting exclusively for `.gd` scripts.

## Requirements

- VS Code `1.83.0` or later
- Requires [Godot-Tools Extension](https://marketplace.visualstudio.com/items?itemName=geequlim.godot-tools)


## Inaccuracies

The syntax highlighter provided by the godot-tools extension does not fully replicate the distinctions made by the internal Godot editor.

To enhance the identification of various tokens provided by the godot-tools extension, several overrides have been implemented. While the color scheme may not be an exact match to the Godot editor, these adjustments try to improve the visibility and differentiation of syntax elements, particularly in dark theme settings.

> **Note:** Currently, there is no distinction between internal classes and user-defined classes; both are colored the same. This may cause some confusion when trying to differentiate between built-in and custom classes in your scripts.

## Color Themes

- Godot 4 Theme (Default Godot Engine Theme)
- Godot 4 Breeze Dark (Matching the Godot Engine Editor Theme `Breeze Dark`)

## Features

### Syntax Highlighting

To align the script highlighting with the Godot editor, the following additional syntax highlighting features have been implemented:

- **Globals**: Includes global functions such as `print`, and global math functions such as `rand` and `deg_to_rad`.
- **Constants**: Encompasses constants like `true`, `false`, `null`, and `PI`, as well as the `void` keyword and the `self` variable.
- **Comments**: Highlights comment keywords such as `TODO`, `FIXME`, `NOTE`, and others.
- **Regions**: Highlights `#region` and `#endregion` directives.

## Contributing

If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request on the [GitHub repository](https://github.com/mariodebono/godot-4-vscode-theme).

**If you find unstyled classes, please raise an issue so they can be addressed.**

## Acknowledgements

Special thanks to [ryanabx's Godot VS Code Theme](https://github.com/ryanabx/godot-vscode-theme) for the inspiration. This theme was developed as a continuation of that work.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
