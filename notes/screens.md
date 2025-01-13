# tmux

```bash
tmux
tmux new -s session1
tmux attach
tmux attach -t session1
tmux detach
tmux ls
tmux kill-server
tmux kill-session -t session1
tmux list-commands

tmux split-window -v
tmux split-window -h
```

`Ctrl + b` keys:
* `c` - create window
* `x` - close window
* `d` - detach
* `w` - list windows
* `n`,`p` - next,prev
* `0`-`9` - jump to window with the number
* `"` - split window horizontally
* `%` - split window vertically
* `arrow` (left, right, up, down) - move between split window
* `c + arrow` - resize

[Documentation](https://tmux.github.io/)

---

# Screen

```bash
screen 
screen -r 
screen -r PID
screen -R
screen -list
```

`Ctrl + a` keys:
* `c` - create
* `"` - list all windows
* `d` - detach
* `n`,`p` - next, prev
* `A` - set window title
* `N` - number and title of the current window
* `'` - jump to window by title / number
* `0`-`9` - jump to window with number
* `i` - info on the current window
* `m` - last message
* `t` - system information
* `v` - version
* `*` - list all displays

[Documentation](https://www.gnu.org/software/screen/)