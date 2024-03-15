echo "# Command-Line Text Editors: nano and vim" > readme.md

echo "## 1. touch Command" >> readme.md
echo "" >> readme.md
echo "The \`touch\` command is used to create an empty file." >> readme.md
echo "   " >> readme.md
echo "![touch](/assets/6.touch.png)" >> readme.md
echo "" >> readme.md

echo "## 2. nano Command" >> readme.md
echo "" >> readme.md
echo "\`nano\` is a simple terminal-based text editor that is user-friendly. It can be installed using the package manager. For example, on Debian/Ubuntu systems, use the following command:" >> readme.md
echo "\`\`\`bash" >> readme.md
echo "sudo apt-get install nano" >> readme.md
echo "\`\`\`" >> readme.md
echo "" >> readme.md
echo "Here's an example of the nano screen layout:" >> readme.md
echo "![nano](/assets/nano.png)" >> readme.md
echo "" >> readme.md
echo "**Navigation in the nano editor:**" >> readme.md
echo "- \`ctrl + G\`: Display the help menu" >> readme.md
echo "- \`ctrl + O\`: Save the file" >> readme.md
echo "- \`ctrl + R\`: Read a new file" >> readme.md
echo "- \`Ctrl + W\`: Search for a string" >> readme.md
echo "- \`Ctrl + K\`: Cut a line" >> readme.md
echo "- \`Ctrl + U\`: Paste a cut line" >> readme.md
echo "- \`ctrl + x\`: Exit nano" >> readme.md
echo "" >> readme.md

echo "## 3. vim Command" >> readme.md
echo "" >> readme.md
echo "\`vim\` is a highly configurable text editor included with most UNIX systems. It can be installed using the package manager. For example, on Debian/Ubuntu systems, use the following command:" >> readme.md
echo "\`\`\`bash" >> readme.md
echo "sudo apt-get install vim" >> readme.md
echo "\`\`\`" >> readme.md
echo "" >> readme.md
echo "Here's the screen layout of vim:" >> readme.md
echo "![vim](/assets/vim.png)" >> readme.md
echo "" >> readme.md
echo "### Modes in vim:" >> readme.md
echo "" >> readme.md
echo "**Normal mode (command mode):**" >> readme.md
echo "- Use arrow keys to move the cursor." >> readme.md
echo "- \`h\`, \`j\`, \`k\`, \`l\` for left, down, up, and right movements, respectively." >> readme.md
echo "- \`gg\` to go to the beginning of the file." >> readme.md
echo "- \`G\` to go to the end of the file." >> readme.md
echo "- \`:\set number\` to display line numbers." >> readme.md
echo "" >> readme.md
echo "**Insert mode:**" >> readme.md
echo "- \`I\` to enter into the insert mode before the cursor." >> readme.md
echo "- \`r\` to enter into the insert mode at the beginning of the line." >> readme.md
echo "- \`a\` to enter insert mode after the cursor." >> readme.md
echo "- \`A\` to enter insert mode at the end of the line." >> readme.md
echo "" >> readme.md
echo "**Saving and Exiting:**" >> readme.md
echo "- \`:\q\` to quit vim." >> readme.md
echo "- \`:\wq\` to save changes and quit vim." >> readme.md
echo "- \`:\q!\` to quit without saving changes in vim." >> readme.md

