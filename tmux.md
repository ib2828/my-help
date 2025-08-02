### Сессии
```
tmux new - создать сессию
tmux ls - список сессий
tmux a -t <session_name> - attach
tmux kill-session <session_name> - удалить сессию 
d (внутри) -  detach
```

### Окна
```
c - создать
, - переименовать
p, n, <#> - переместиться
& - удалить
```

### Панели
```
% - деление по вертикали
" - деление по горизонтали
q - показать номера панелей
стрелки, q<#> - перемещение между панелями
Ctrl + стрелки - изменение размера
x - удалить
z - растянуть на всё окно
[ - scroll внутри панели
? - показать хоткеи
```

### tmuxinator
```
tmuxinator list - список
tmuxinator new <project> - создать
tmuxinator edit <project> - ред.
tmuxinator start <project>
```

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
