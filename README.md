## Features

- Launch applications and web pages directly from Vim.
- Store and manage the addresses of your apps and web pages in separate files.
- Cross-platform support for Windows, macOS, and Linux.

## Installation

To install flexibleVP, you can use a plugin manager like [Vim-Plug](https://github.com/junegunn/vim-plug). Add the following line to your Vim configuration file (e.g., `~/.vimrc` or `init.vim`):

```vim
Plug 'SuprimeBG/flexibleVP'
```

## Usage

To launch an app or open a web page, use the `:Launch` command followed by the name of the app or web page. For example:

```vim
:Launch facebook
```

This will search for the specified name in the app and web page address files and open the corresponding address.
You can add new app or web page addresses using the `:Addw` and `:Adda` commands or just go to webaddress.txt or appaddress.txt. 
For example:
```vim
:Addw example_name www.example.com
:Adda brave C:\Program Files\BraveSoftware\Brave-Browser\Application\brave.exe
```
## Common errors

If you encounter any error with launching something check the .txt files as they should be ```txt name: address ``` and the web addresses must be whole like this: http://www.example.com as the plugin uses the explorer function for windows to open web pages. If the address is not in this format it wil open Documentation folder.
