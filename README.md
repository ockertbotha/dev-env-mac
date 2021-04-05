# Setting up Dev Env on Mac

> Last completed using **Big Sur** on **5 April 2021**

| Last Completed | 5 April 2021   |
|----------------|----------------|
| Mac OS         | Big Sur 11.2.3 |

| Installed Tools / Software |
|----------------------------|
| Xcode                      |
| Homebrew                   |
| git                        |
| iTerm2                     |
| zsh, Oh My Zsh             |
| Powerlevel10K              |
| Java JDK                   |
| jEnv                       |
| Maven                      |

<br/>

**Fire up the Terminal and get started:**

</br>

## 1. Install Xcode
```
sudo xcode-select --install
```

## 2. Install Homebrew
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```

## 3. Configure Homebrew
Once Homebrew installation is complete a **Next steps:** message is displayed the first of which is **Add Homebrew to your PATH**, copy and execute **YOUR** version of message.
```
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> /Users/ockert/.zprofile
```

## 4. Verify Homebrew
```
brew doctor
```

## 5. Install Git
```
brew install git
```

## 6. Install iTerm2
> Home: https://iterm2.com/index.html
```
brew install iterm2
```
## 7. Launch iTerm2
Use iTerm for terminal commands from this step onward.

## 8. Check Zsh version
```
zsh --version
```

## 9. Install Oh My Zsh
> Home: https://github.com/ohmyzsh/ohmyzsh
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

## 10. Restart iTerm2


## 11. Install Powerlevel10K Zsh theme
> Home: https://github.com/romkatv/powerlevel10k
```
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
```

## 12. Set Powerlevel10K theme
```
nano ~/.zshrc
```
Find and set:
```
ZSH_THEME="powerlevel10k/powerlevel10k"
```

## 13. Restart iTerm2 > Starts up in Powerlevel10K configuration wizard
Select / Set the following options:
- Install Meslo Nerd Font? **Yes**
- Restart iTerm2: **⌘ Q**
- Answer diamond question.
- Answer lock question.
- Answer logo question.
- Answer overlap question.
- Prompt Style: **(3) Rainbow**
- Character Set: **(1) Unicode.**
- Show current time? **(2) 24-hour format.**
- Prompt Separators: **(1) Angled.**
- Prompt Heads: **(1) Sharp.**
- Prompt Tails: **(1) Flat.**
- Prompt Height: **(2) Two lines.**
- Prompt Connection: **(2) Dotted.**
- Prompt Frame: **(3) Right.**
- Connection & Frame Color: **(2) Light.**
- Prompt Spacing: **(2) Sparse.**
- Icons: **(2) Many icons.**
- Prompt Flow: **(1) Concise.**
- Enable Transient Prompt? **(n) No.**
- Instant Prompt Mode: **(1) Verbose**
- Apply changes to ~/.zshrc? **(y) Yes.**

To run it again:
> ``` 
> p10k configure 
> ``` 

## 14. Install Java
```
brew tap adoptopenjdk/openjdk
```
```
brew install adoptopenjdk8
```
```
brew install adoptopenjdk11
```

## 15. Install jEnv
>Home: https://www.jenv.be/

```
brew install jenv
```
```
echo 'export PATH="$HOME/.jenv/bin:$PATH"' >> ~/.zshrc
```
```
echo 'eval "$(jenv init -)"' >> ~/.zshrc
```

## 16. Restart iTerm2

## 17. Setup jEnv
```
jenv add /Library/Java/JavaVirtualMachines/adoptopenjdk-8.jdk/Contents/Home
```

```
jenv add /Library/Java/JavaVirtualMachines/adoptopenjdk-11.jdk/Contents/Home
```

## 18. Install Maven
```
brew install maven
```