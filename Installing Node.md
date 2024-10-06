
## Installing Node.js

For some reason, my homebrew does not work so I had to install node via nvm. Here is how. 


```bash
sudo touch ~/.bash_profile
```

Install nvm using curl

```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.0/install.sh | bash
```

Check to make sure nvm is installed

```bash
nvm --version
```

install node using nvm 

```bash
nvm install node
```

Check the node version 

```bash 
node --version
```

## <font color="#bd2d26">Possible Errors</font>

1. You enter nvm or npm and the result is
   ```bash
   command not found
   ````

   In this case check your shell by entering
   ```bash
   echo $SHELL
   ````

   If you are not using bash and are using zsh, reinstall using this 

  ```bash
  curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.0/install.sh | zsh
  ```

  another more complicated alternative is creating a ~/.zshrc file 
  ```bash
  
  
  ```
  <font color="#bd2d26">You may have to you use root priviallage via the sudo command</font>
  
  add this line to the ~/.zshrc file 
  ```bash
  source ~/.nvm/nvm.sh
  ```

  I would use nano to edit this file 
  ```bash
  sudo nano ~/.zshrc
  ```

  Edit the file 
  ```bash
  # >>> conda initialize >>>
  # !! Contents within this block are managed by 'conda init' !!
  __conda_setup="$('/opt/miniconda3/bin/conda' 'shell.zsh' 'hook' 2> /dev/null)"
  source ~/.nvm/nvm.sh
  if [ $? -eq 0 ]; then
      eval "$__conda_setup"
  else
      if [ -f "/opt/miniconda3/etc/profile.d/conda.sh" ]; then
          . "/opt/miniconda3/etc/profile.d/conda.sh"
      else
          export PATH="/opt/miniconda3/bin:$PATH"
      fi
  fi
  unset __conda_setup
  # <<< conda initialize <<<
  ```
  Close the terminal and type nvm or npm again.

  Feel free to email me if you encounter any issues.

  Happy Hacking!
  


   
