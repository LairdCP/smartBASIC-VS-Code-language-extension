# SmartBASIC Language Extension for Visual Studio Code

A Visual Studio Code extension with syntax highlighting for Laird Connectivity's SmartBASIC language.

## SmartBASIC

Laird Connectivity’s smartBASIC is an event-driven programming language that was designed to make BLE technology development quicker and simpler, vastly cutting down time to market. A simple smartBASIC application encapsulates the complete end-to-end process of reading, writing, and processing sensor data as well as advertising, connecting, security, power management, and wireless status. See https://www.lairdconnect.com/wireless-modules/bluetooth-modules for more information.

## Language Extension

### Syntax Highlighting

Laird provides syntax highlighting files for Notepad++ (Windows) and Textpad (Mac OSX) along with their regular module firmware versiosn releases. This VS Code language extension is based on the latest Notepad++ syntax files for BL652, BL653 and BL654. Other than the original syntax files from Laird, which cover only the language scope of each module's SmartBASIC implementation, this language extension is a superset of these scopes.

The drawback of this implementation is, that when working on e.g. a BL652 module, VS Code would also highlight SmartBASIC functions, which are only available on the higher-end BL653 or BL654 modules. The advantage is, that you only need one syntax file and no need to switch syntax files when working with different modules in parallel.

### Snippets

Snippets were contributed by [cvanbeek13](https://github.com/cvanbeek13). To add a snippet, start typing the snippet prefix. VS Code will list it as an auto-fill option:

![image](https://user-images.githubusercontent.com/35079932/145184982-2e7a749d-e8bc-4ab7-b6df-d56a921902ad.png)

Clicking enter on the snippet will insert it. You then can fill out the fields, clicking tab after each to fill in additional data (such as name, args, and return_val here).

![image](https://user-images.githubusercontent.com/35079932/145185047-5a35dc5e-5bc6-40cc-a9dc-9efce991eb32.png)

### Code Folding

[cvanbeek13](https://github.com/cvanbeek13) also contributed code folding, so you can collapse sections/blocks of code. E.g. a for loop:

![image](https://user-images.githubusercontent.com/35079932/145185674-7b3af677-307c-47da-a2b2-77a106d0e660.png)

gets collapsed like this:

![image](https://user-images.githubusercontent.com/35079932/145185729-b2a89730-3ebe-4433-8755-d9d0ae1c7d3c.png)

## File Recognition

SmartBASIC files are usually given names with suffix .sb or .sblib. This language extension recognizes both.

## Manual Installation

Place the full folder cloned from this repository in the VS Code extensions folder at

* Windows: %USERPROFILE%\\.vscode\\extensions
* MaxOS/Linux: ~/.vscode/extensions

Might require a restart of VS Code.

## Install with Extension Manager

This extension is not yet available through the extension manager.

## License

This package is licensed under the MIT License.
