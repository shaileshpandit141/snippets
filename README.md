# Zed Editor Configuration

This `settings.json` file customizes the Zed Editor to enhance productivity and align with specific development workflows. Below is an explanation of each configuration section and the selected settings.

## Table of Contents

- [Assistant Configuration](#assistant-configuration)
- [UI and Display](#ui-and-display)
- [Project Panel](#project-panel)
- [Editor Settings](#editor-settings)
- [File Management](#file-management)
- [Formatting](#formatting)
- [Language Server Protocol (LSP)](#language-server-protocol-lsp)
- [Terminal Settings](#terminal-settings)
- [Vim Mode](#vim-mode)

---

### Assistant Configuration

The assistant model is set up with the following configurations:

- **Model Provider**: `zed.dev`
- **Model**: `claude-3-5-sonnet-latest`
- **Version**: `2`

### UI and Display

- **UI Font Size**: Set to `16` for readability across interface elements.
- **Buffer Font Size**: Also set to `16` to maintain consistency with UI font size.
- **Theme**:
  - **Mode**: System-based, meaning it adapts to the system theme (light/dark mode).
  - **Light Theme**: `One Light`
  - **Dark Theme**: `Summercamp`

### Project Panel

The project panel is docked on the **right** side of the editor, optimizing space and providing a clear view of project files and folders.

### Editor Settings

Key editor customizations include:

- **Completion**: Path-based autocompletion is enabled.
- **Hover Popover**: Enabled for quick access to information on hover.
- **Auto-closing**: Automatically closes pairs (like braces and quotes), matching pairs, and HTML tags, streamlining coding.
- **Auto-renaming**: HTML tags auto-rename when one tag is edited.
- **Tab Size**: Set to `2` spaces for cleaner, more compact code indentation.
- **Base Keymap**: `VSCode` keymap is used, allowing users familiar with VSCode shortcuts to transition smoothly.

### Autosave

- **After Delay**: Automatically saves files after 1.5 seconds (1500 milliseconds) of inactivity, ensuring minimal data loss.

### File Management

- **Exclude Files**: The following directories are excluded from the editor for a cleaner workspace:
  - `__pycache__`, `node_modules`, `.git`, `migrations`, `dist`, and `.next`.
- **Watcher Exclude**: Prevents editor from watching certain directories, reducing system resource usage.

### Formatting

- **Formatter**: `language_server` is used as the formatter.
- **Format on Save**: Enabled, so files are automatically formatted upon saving.
- **Format on Paste**: Ensures consistency by formatting pasted code immediately.

### Language Server Protocol (LSP)

- **Rust Analyzer**:
  - Uses the `clippy` command to ensure code quality and adherence to best practices in Rust.
- **TypeScript Language Server**:
  - Formatting is enabled for TypeScript projects, enhancing code consistency.

### Terminal Settings

- **Shell Program**: `/bin/bash` is set as the default shell.
- **Working Directory**: Defaults to the `current_project_directory`.
- **Font Size**: Set to `16` for readability.
- **Blinking Cursor**: Disabled to provide a stable visual environment in the terminal.

### Vim Mode

This configuration includes enhanced Vim support:

- **System Clipboard**: Always uses the system clipboard, making copying and pasting easier.
- **Normal Mode Keybindings**: Custom keybindings in Normal Mode:
  - `j` navigates **down**
  - `k` navigates **up**

---

## Additional Notes

- **Telemetry**: Diagnostics and metrics telemetry are enabled to help improve the editor’s performance and stability.
- **Auto-update**: Set to `true` to keep the editor up-to-date automatically.

This configuration provides a balanced development environment focused on efficiency, readability, and customization for users familiar with VSCode, Rust, TypeScript, and Vim keybindings.
