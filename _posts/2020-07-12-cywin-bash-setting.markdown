---
layout: post
title:  cygwin bash 설정 파일
date:   2020-07-12 21:53:47 +0900
description: cygwin bash 설정 파
---
```
alias C:='cd /cygdrive/c'
alias F:='cd /cygdrive/f'
alias G:='cd /cygdrive/g'
alias TMP:='cd /cygdrive/c/cygwin/tmp'
alias CYG:='cd /cygdrive/c/cygwin'
alias GIT:='cd /cygdrive/c/git'
alias PY:='cd /cygdrive/c/python'
alias cls='clear'
alias euc='export LANG=ko_KR.euckr'
alias utf='export LANG=ko_KR.utf8'
alias tm='unset TMOUT'
alias egrep='egrep --color=auto'
alias fgrep='fgrep --color=auto'
alias grep='grep --color=auto'
alias ci='/cygdrive/c/cygwin/setup-x86_64.exe -q -P '
alias gem='/cygdrive/c/Ruby26-x64/bin/gem.bat'


# Original
#export PS1="\[\e]0;\w\a\]\n\[\e[32m\]\u@\h \[\e[33m\]\w\[\e[0m\]\n\$ "
# 5c
#export PS1="\[\e]0;\w\a\]\n\[\e[32m\]5c \[\e[33m\]\w\[\e[0m\]\n\$ "
export PS1="\[\e]0;\w\a\]\[\e[32m\]5c \[\e[33m\]\w\[\e[0m\]\$ "

set -o vi

```
