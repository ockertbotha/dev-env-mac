# Install and Configure NodeJS with NVM

## Installing NVM

  ```
  brew install nvm
  ```
  
### Follow the the on-screen instructions forom Homebrew. Usually: 
  ```
  mkdir ~/.nvm
  ```
  
  ```
echo 'export NVM_DIR="$HOME/.nvm"
  [ -s "/opt/homebrew/opt/nvm/nvm.sh" ] && \. "/opt/homebrew/opt/nvm/nvm.sh"  # This loads nvm
  [ -s "/opt/homebrew/opt/nvm/etc/bash_completion.d/nvm" ] && \. "/opt/homebrew/opt/nvm/etc/bash_completion.d/nvm"  # This loads nvm bash_completion' >> ~/.zshrc
  ```

---

## Installing a version of NodeJS

```
nvm install --lts
```

--- 

## Test with
```
node -v
```