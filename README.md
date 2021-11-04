# cfg-install
bootstrapper for installing dotfiles and setup scripts

## How to use it
1. Make sure that a `.ssh`* folder with the correct SSH keys is in `$HOME`  
Download command line developer tools (before using a git command to clone the dotfiles repo)  
  `$ sudo xcode-select —-install`  
  then update it with  
  `$ softwareupdate --all --install --force `  
3. Transfer to a file this simple script with `curl` to automatize first-step setup to clone the settings/dotfiles repo on any new machine
  ```bash
  touch bootstrap
  curl -Lks https://raw.githubusercontent.com/webdev-skynet/cfg-install/main/bootstrap > bootstrap
  chmod 755 bootstrap
  ./bootstrap
  ```
3. Then `source .zshrc` to initialize last config and git user info setting routine from `.private`*  and do the setup

<span>* file on secret place</span>
