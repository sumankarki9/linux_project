## Basic Terminal Text Editors

1. **touch**:  
    The `touch` command is used to create an empty file.  
    ![touch](/assets/6.touch.png)

2. **nano**:  
    `nano` is a simple terminal-based text editor known for its user-friendly interface. It can be installed using a package manager like apt on Debian/Ubuntu systems:
    ```bash
    $ sudo apt-get install nano
    ```  
    Here's an example of the nano screen layout:  
    ![nano](/assets/nano.png)

    Navigation in nano includes:
    - **Ctrl + G**: Display the help menu
    - **Ctrl + O**: Save the file
    - **Ctrl + R**: Read a new file
    - **Ctrl + W**: Search for a string
    - **Ctrl + K**: Cut a line
    - **Ctrl + U**: Paste a cut line
    - **Ctrl + X**: Exit nano

3. **vim**:  
    `vim` is a highly configurable text editor designed for efficient text manipulation. It is included as "vi" with most UNIX systems.  
    It can be installed using a package manager like apt on Debian/Ubuntu systems:
    ```bash
    $ sudo apt-get install vim
    ```  
    Here's the screen layout of vim:  
    ![vim](/assets/vim.png)

    Vim has two modes:
    - **Normal mode (command mode)**
    - **Insert mode**

    In Normal mode:
    - We use arrow keys to move the cursor
    - `h` `j` `k` `l`for left, down, up, and right respectively
    - `gg` is used to go to the beginning of the file
    - `G` is used to go to the end of the file
    - `:set number` is used to display line numbers

    In Insert mode:
    - `I` to enter into the insert mode before the cursor
    - `r` to enter into the insert mode at the beginning of the line
    - `a` to enter insert mode after the cursor
    - `A` to enter insert mode at the end of the line

    Saving and exiting in vim:
    - `:q` to quit vim
    - `:wq` to save changes and quit vim
    - `:q!` to quit without saving changes in vim
