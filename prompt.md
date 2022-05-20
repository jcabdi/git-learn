Make your prompt to tell you about the repository status

1- open ~/.bashrc in an editor, look for the following lines and make it look like this:

if [ "$color_prompt" = yes ]; then
   #PS1='${debian_chroot:+($debian_chroot)}\[\033[01;32m\]\u@\h\[\033[00m\]:\[\033[01;34m\]\w\[\033[00m\]\$ '
    PS1='${debian_chroot:+($debian_chroot)}\[\033[01;32m\]\u@\h\[\033[00m\]:\[\033[01;34m\]\w\[\033[01;32m\]$(__git_ps1)\[\033[00m\]\$ '
else
   #PS1='${debian_chroot:+($debian_chroot)}\u@\h:\w\$ '
    PS1='${debian_chroot:+($debian_chroot)}\u@\h:\w$(__git_ps1)\$ '
fi
unset color_prompt force_color_prompt

then add at the end of the file the following lines:

# Git
GIT_PS1_SHOWDIRTYSTATE='y'

GIT_PS1_SHOWSTASHSTATE='y'

GIT_PS1_SHOWUNTRACKEDFILES='y'

GIT_PS1_SHOWUPSTREAM='auto'
___


### The explanation to understand each symbols is here:

| Option | Value | Description
| --- | ----------- | ------------------
| GIT_PS1_SHOWDIRTYSTATE | any nonempty value | shows * or a + for unstaged and staged changes, respectively
| GIT_PS1_SHOWSTASHSTATE| any nonempty value| shows $ if there are any stashes
| GIT_PS1_SHOWUNTRACKEDFILES| any nonempty value| shows % if there are any untracked files
| GIT_PS1_SHOWUPSTREAM| auto| shows <, >, <>, or = when your branch is behind, ahead, diverged from, or in sync with the upstream branch, respectively
