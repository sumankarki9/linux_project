#!/bin/bash

# Command-Line Text Editors: nano and vim

# 1. touch
echo "The 'touch' command is used to create an empty file."
echo "![touch](/assets/6.touch.png)"

# 2. nano
echo "'nano' is a simple terminal-based text editor known for its user-friendly interface."

# Installation
echo "### Installation:"
echo "You can install nano using a package manager. For example, on Debian/Ubuntu systems, you can use the following command:"
echo "sudo apt-get install nano"

# Usage
echo "### Usage:"
echo "Here's an example of the nano screen layout:"
echo "![nano](/assets/nano.png)"

# Navigation
echo "### Navigation:"
echo "- Press 'ctrl + G' to display the help menu."
echo "- Press 'ctrl + O' to save the file."
echo "- Press 'ctrl + R' to read a new file."
echo "- Press 'Ctrl + W' to search for a string."
echo "- Press 'Ctrl + K' to cut a line."
echo "- Press 'Ctrl + U' to paste a cut line."
echo "- Press 'ctrl + X' to exit nano."

# 3. vim
echo "'vim' is a highly configurable text editor included with most UNIX systems."

# Installation
echo "### Installation:"
echo "You can install vim using a package manager. For example, on Debian/Ubuntu systems, you can use the following command:"
echo "sudo apt-get install vim"

# Usage
echo "### Usage:"
echo "Here's an example of the vim screen layout:"
echo "![vim](/assets/vim.png)"

# Modes
echo "### Modes:"
echo "- **Normal mode (command mode):**"
echo "  - Use arrow keys to move the cursor."
echo "  - Press 'h', 'j', 'k', 'l' for left, down, up, and right movements, respectively."
echo "  - Type 'gg' to go to the beginning of the file."
echo "  - Type 'G' to go to the end of the file."
echo "  - Type ':set number' to display line numbers."
echo
echo "- **Insert mode:**"
echo "  - Type 'I' to enter insert mode before the cursor."
echo "  - Type 'r' to enter insert mode at the beginning of the line."
echo "  - Type 'a' to enter insert mode after the cursor."
echo "  - Type 'A' to enter insert mode at the end of the line."

# Saving and Exiting
echo "### Saving and Exiting:"
echo "- Type ':q' to quit vim."
echo "- Type ':wq' to save changes and quit vim."
echo "- Type ':q!' to quit without saving changes in vim."
