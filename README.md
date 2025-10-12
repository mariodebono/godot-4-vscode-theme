# Godot 4 VS Code Theme for GDScript

[![Visual Studio Marketplace version](https://img.shields.io/visual-studio-marketplace/v/mariodebono.godot-4-vscode-theme)](https://marketplace.visualstudio.com/items?itemName=mariodebono.godot-4-vscode-theme)
[![Visual Studio Marketplace installs](https://img.shields.io/visual-studio-marketplace/i/mariodebono.godot-4-vscode-theme)](https://marketplace.visualstudio.com/items?itemName=mariodebono.godot-4-vscode-theme)

The Godot 4 VS Code Theme is now officially released as version 1.0.2. It mirrors the editor palette from Godot 4 and ships grammar tweaks that make GDScript easier to read inside Visual Studio Code. The latest update restores highlighting for the `wrap` helper so globals stay consistent across the API.

## Install and activate

1. Open the Extensions view in VS Code and search for **Godot Theme for VS Code**.
2. Install the extension published by `mariodebono`.
3. Open the Command Palette and run **Preferences: Color Theme**, then pick either **Godot 4** or **Godot 4 - Breeze Dark**.
4. If you prefer an offline install, download the `.vsix` from the releases page and install it with **Extensions: Install from VSIX**.

## Requirements

- Visual Studio Code 1.83.0 or later
- [Godot Tools](https://marketplace.visualstudio.com/items?itemName=geequlim.godot-tools) for best grammar support (the theme loads without it, but extra scopes rely on that extension)

## Release highlights for 1.0.2

- Restores the missing `wrap` global highlight so helper functions stay readable in scripts
- Accurate colors for classes declared with `class_name`, covering both built-in and project types

For earlier history, see the [changelog](CHANGELOG.md).

## Why choose this theme

- Editor colors match the official Godot 4 look, so switching between the engine and VS Code feels natural
- Two bundled variants: the default Godot 4 palette and the Breeze Dark theme used in the editor
- Clear contrast for signals, classes, control flow, and comments, tuned for long sessions in dark mode
- Support syntax highlighting #regions
- Terminal, activity bar, and status bar colors align with the code editor for a consistent workspace

## Syntax coverage

The theme builds on the scopes provided by Godot Tools and extends them with custom injections:

- Global helpers like `print`, `randf`, `lerp_angle`, and more
- Constants such as `true`, `false`, `null`, `PI`, and the `void` keyword
- The `self` keyword and other language identifiers that Godot developers use every day
- Region markers `#region` and `#endregion`
- Comment keywords including TODO, FIXME, NOTE, WARNING, CRITICAL, NOTICE
- Shader script scopes for types, uniforms, functions, and operators

## FAQ

**Does the theme work without Godot Tools?** Yes. You can enable it without Godot Tools, but the extra grammar injections (class names, comment tags, globals) require the scopes that extension adds.

**How do I switch between the two theme variants?** Open the Command Palette, run **Preferences: Color Theme**, and select either **Godot 4** or **Godot 4 - Breeze Dark**.

**Where do I report missing highlights?** Open an issue on the [GitHub repository](https://github.com/mariodebono/godot-4-vscode-theme/issues) and include a short code sample.

## Contributing

Contributions are welcome:

1. Fork the repository and create a branch for your change.
2. Update the theme JSON or grammar files as needed.
3. Run your tests or manual checks.
4. Open a pull request with screenshots that show the change in action.

If you discover an unstyled token, please raise an issue so it can be fixed.

## Acknowledgements

The project builds on the work of [ryanabx's Godot VS Code Theme](https://github.com/ryanabx/godot-vscode-theme) and feedback from the Godot community.

## License

This project is released under the MIT License. See the [LICENSE](LICENSE) file for details.
