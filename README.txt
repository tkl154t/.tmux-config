- Put this project to ~/.tmux-config
- Copy tmux.conf to ~/.tmux.conf
- Prefix + I to reload env
- Prefix + r to load config file

Prefix = Ctrl + B

#Change title name of pane
:select-pane -T pane-name

#Move current pane to session:windows
:join-pane -t session:windows

#Capture pane
tmux capture-pane -t 0 -S -1000 -E 20 -p > log.txt
