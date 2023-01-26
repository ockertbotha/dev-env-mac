# Install and Configure Elixir with asdf

## Installing asdf
---
Install asdf - https://asdf-vm.com/guide/getting-started.html 
- Use Official Download (Git)
- For install use ZSH & Git oh-my-zsh - https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/asdf 

## Installing Erlang
---
Install  asdf-erlang plugin - https://github.com/asdf-vm/asdf-erlang
>Read the **Before ```asdf install```** section and focus on OSX instructions

  ```
  echo 'export PATH="/opt/homebrew/opt/openssl@1.1/bin:$PATH"' >> ~/.zshrc
  ```
  
  ```
  echo 'export KERL_BUILD_DOCS=yes' >> ~/.zshrc
  ```
  
  ```
  echo 'export ERL_AFLAGS="-kernel shell_history enabled"' >> ~/.zshrc
  ```

Add the erlang plugin
```
asdf plugin add erlang https://github.com/asdf-vm/asdf-erlang.git
```

Install the erlang plugin
```
asdf install erlang latest
```

```
asdf global erlang latest
```

## Installing Elixir
---
Add elixir plugin
```
asdf plugin-add elixir https://github.com/asdf-vm/asdf-elixir.git
```

Install the elixir plugin
```
asdf install elixir latest
```

```
asdf global elixir latest
```

## Test with
--- 
```
iex
```