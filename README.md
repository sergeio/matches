matches
=======
Execute a command if STDIN matches a pattern

Example usage:
--------------
```
long_running_command | matches WARNING "espeak 'long running command warning'"
```
Examines the output of `long_running_command`, and vocally warn you if the
output contains the text 'WARNING'.

```
tmux pipe-pane -t:5.1 -o '~/bin/matches compiled "espeak compiled"'
```
Tells tmux to watch window 5, panel 1, and say "compiled" (vocally) when the
output of that pane has "compiled" in it.
