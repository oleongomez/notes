## Send reload command to all panes
```bash
tmux list-panes -a -F '#{session_name}:#{window_index}.#{pane_index}' | while read pane; do tmux send-keys -t "$pane" "source ~/.bashrc" Enter; done
```
