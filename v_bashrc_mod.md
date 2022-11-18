Apply the following content to .bashrc:
```bash
# Setup for eternal bash history (default HISTSIZE and HISTFILESIZE can be deleted)
# ---------------------
# Undocumented feature which sets the size to "unlimited".
# http://stackoverflow.com/questions/9457233/unlimited-bash-history
export HISTFILESIZE=
export HISTSIZE=
export HISTTIMEFORMAT="[%F %T] "
# Change the file location because certain bash sessions truncate .bash_history file upon close.
# http://superuser.com/questions/575479/bash-history-truncated-to-500-lines-on-each-login
export HISTFILE=~/.bash_eternal_history
# Force prompt to write history after every command.
# http://superuser.com/questions/20900/bash-history-loss

export PROMPT_COMMAND='history -a'
alias hgrep='history|grep --color'

# Shortcut for copying to clipboard
alias "cs=tr -d '\n' | xclip -selection c"

export CUDA_DEVICE_ORDER=PCI_BUS_ID

measure_cpu() { ps -p $1 -o pcpu | tail | tac | xargs; }
watch_cpu() {
while t=$(ps -p $1 -o etimes,time,pcpu); do echo "$t" | tail -n 1; sleep 3; done
}
```
