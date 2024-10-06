
## Installing Node.js

For some reason, my homebrew does not work so I had to install node via nvm. Here is how. 


```bash
sudo touch ~/.bash_profile
```

Install nvm using curl

```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.0/install.sh | bash
```
This will refresh the available commands in your system path.

```bash
source ~/.nvm/nvm.sh
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
