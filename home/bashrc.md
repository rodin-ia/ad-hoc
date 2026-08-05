root promt
```
PS1='${debian_chroot:+($debian_chroot)}\[\033[01;31m\]\u\[\033[01;32m\]@\h\[\033[00m\]:\[\033[01;34m\]\w\[\033[00m\]\$ '  
```

user promt
``` 
PS1='${debian_chroot:+($debian_chroot)}\[\033[01;33m\]\u\[\033[01;32m\]@\h\[\033[00m\]:\[\033[01;34m\]\w\[\033[00m\]\$ '
```

for screen 

```
if [[ -n "$PS1" ]] && [[ -z "$SCREEN" ]] && [[ -n "$SSH_CONNECTION" ]]; then
  screen -x ssh_screen || screen -S ssh_screen
fi
```
