# tmux-sessionizer

tmux-sessionizer is a tmux script that makes your workflow BLAZINGLY FAST written by [ThePrimeagen](https://github.com/ThePrimeagen/)

## Installation

### tmux-sessionizer script

- Save the script on `~/.local/bin/tmux-sessionizer` where `tmux-sessionizer` is the name of the script

- Here change the find paths to your corresponding paths to projects folder on which you want to work on


## Add the macro `ctrl+f` on your `.bashrc`
```bash
bind '"\C-f": "tmux-sessionizer\n"'
```

## Add the macro `ctrl+f` on your `.zshrc`

```bash
bindkey -s ^f "tmux-sessionizer\n"
```

### For Fish use this

```sh
bind \cf "tmux-sessionizer"
```

## Add the following script on your `.tmux.conf`

```bash
bind-key F run-shell "tmux neww tmux-sessionizer"
```

- This will open fuzzy finder then you can search for the project you want and start new tmux session on that project directory on pressing `<prefix>F`


## Now restart your shell and enjoy the blazing fast workflow

### Steps to use

- Press `ctrl+f` to open the fzf finder
- type the name of project you want to work on and press enter
- Now you will be on the project directory on tmux session

> Note:
>
> you can see prime's [video](https://youtu.be/hJzqEAf2U4I) on this to understand in detail
