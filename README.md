# tmux

## Start a new session
```
tmux             # Start a new session
tmux new -s name # Start with a custom name

exit             # Exit a pane (and close it)
Ctrl+b then d    # Detach from session (keeps it running)
```

### To reattach

```
tmux attach           # Attach to the most recent session
tmux attach -t name   # -t (target)
tmux ls               # List all sessions
```

## Navigation (Default Prefix is Ctrl+b)

### panes

split horisontially   ->> prefix- "
split vertically      ->> prefix- %
move between panes    ->> prefix- arrows
kill the current pane ->> prefix- x

### windows

create new window  ->> c
next window        ->> n
prev window        ->> p
list windows       ->> w
rename curr window ->> ,
kill window        ->> &


## Sessions

```
tmux new -s mysession
tmux switch -t mysession                 # you write this from within a session
tmux rename-session -t oldname newname
tmux kill-session -t mysession
```


## Useful Commands

```
tmux ls                   # lists sessoins
tmux list-sessions
tmux list-windows
tmux list-panes
tmux kill-server          # Kill all tmux sessions
```


## Configuration

Minimalistic...
[my config](https://github.com/ammarashraf99/dotfiles/blob/main/.tmux.conf)




