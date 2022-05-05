# Removing JENV

### 1. Uninstall from Brew
- Run ```brew uninstall jenv```

### 2. Cleaning iTerm2 and ZSH profile
- Edit ```~/.bash_profile``` and / or ```~/.zshrc```
- Removing the jenv lines:
```
# To customize prompt, run `p10k configure` or edit ~/.p10k.zsh.
[[ ! -f ~/.p10k.zsh ]] || source ~/.p10k.zsh
export PATH="$HOME/.jenv/bin:$PATH"
eval "$(jenv init -)"
```
becomes:
```
# To customize prompt, run `p10k configure` or edit ~/.p10k.zsh.
[[ ! -f ~/.p10k.zsh ]] || source ~/.p10k.zsh
```

### 3. Remove JENV directory
- Run ```rm -rf .jenv```


### 4. Remove unwanted JVMs

```
ls -la  /Library/Java/JavaVirtualMachines/
```

```
rm -rf /Library/Java/JavaVirtualMachines/adoptopenjdk-8.jdk
```