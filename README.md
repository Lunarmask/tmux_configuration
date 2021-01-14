## TMUX CONFIG from Lunarmask_

---

* This config assumes you are using __[NeoVim](https://neovim.io/)__ as your vim source.  
* I would also like to recommend using __Alacritty__ for your terminal emulator.
__[Alacritty](https://github.com/alacritty/alacritty)__ paired
with __[tmux](https://github.com/tmux/tmux)__ makes for a killer combo!

* This config is only a part of my config compilation __[Lunarmasks Linux Config](https://gitlab.com/linux_configurations/tmux_configuration)__.

---------
### ABOUT

This configuration file tries to highlight the existing awesomeness of TMUX.  
The goal is to expand some existing basic features without creating bloat.  

Please feel free to read through the `tmux.conf` file yourself for more information.  

---------
### SETUP

1) Download this `tmux.conf` file and place it into _`~/.config/tmux/`_.  
  * If this folder does not exist, create it!
  * If the config does not source automatically when you launch tmux, 
    you will need to run this command:  
    $ `echo "source-file ~/.config/tmux/tmux.conf" >> ~/.tmux.conf`

2) Launch tmux with $ `tmux`

__You're all set!__

---

### TMUX GUIDE

__Tmux__ is a great terminal multiplexer that allows for you easily manage multiple terminal instances with some perks!

You have both windows and panes at your disposal.  
* Panes allow you to open multiple feeds of input on the same screen.  
* Windows allow you to group multiple panes into logical groups.   

---------------------
#### Pane Management

`<C-a>v` or `<Alt>v` Create a vertical split-pane.  

`<C-a>s` or `<Alt>s` Create a horizontal split-pane.  

`<C-a>z` or `<Alt>z` Maximize focus to the current pane. Toggle off with the same command.  

`<C-a>x` or `<Alt>x` Close out current pane.  

`<C-a>hjkl` or `<Alt>hjkl` Use Vim-keys to navigate between panes.  

---------------------
#### Window Management

`<C-a>c` or `<Alt>c` Create a new window.  

`<Alt-Shift>hk` Use Alt+shift + Vim-keys to navigate windows.  

`<Alt>LEFT|RIGHT` Use Alt and arrows-keys to navigate windows.  

`<C-a>,` or `<Alt>,` Rename current Window.  

---------------
#### VIM MODE

`<C-a>[` Enters into vim mode.  
* This allows you to navigate and copy text that appeared in the data feed.


`/` or `?` Search  for _{regex}_<br>  
`n` Jump to the next instance of highlighted word<br>  
`N` Jump to previous instance of highlighted word<br>  
`v` Start visualing text to copy<br>  
`y` Copy visualized text.  
