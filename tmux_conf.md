## Конфиг
`vim ~/.tmux.conf`
```
set -g base-index 1
setw -g pane-base-index 1
set -g default-terminal "screen-256color"
set -g history-file ~/.tmux_history
set -sg history-limit 5000
bind-key -T prefix S setw synchronize-panes
```
