# SmartBASIC Language Extension for Visual Studio Code

A Visual Studio Code extension with syntax highlighting for Laird Connectivity's SmartBASIC language.

## SmartBASIC

Laird Connectivity’s smartBASIC is an event-driven programming language that was designed to make BLE technology development quicker and simpler, vastly cutting down time to market. A simple smartBASIC application encapsulates the complete end-to-end process of reading, writing, and processing sensor data as well as advertising, connecting, security, power management, and wireless status. See https://www.lairdconnect.com/wireless-modules/bluetooth-modules for more information.

## Syntax Highlighting

Laird provides syntax highlighting files for Notepad++ (Windows) and Textpad (Mac OSX) along with their regular module firmware versiosn releases. This VS Code language extension is based on the latest Notepad++ syntax files for BL652, BL653 and BL654 (as of today... ping me in case there is a new firmware version, I might have missed). Other than the original syntax files from Laird, which cover only the language scope of each module's SmartBASIC implementation, this language extension is a superset of these scopes.

The drawback of this implementation is, that when working on e.g. a BL652 module, VS Code would also highlight SmartBASIC functions, which are only available on the higher-end BL653 or BL654 modules. The advantage is, that you only need one syntax file and no need to switch syntax files when working with different modules in parallel.

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
