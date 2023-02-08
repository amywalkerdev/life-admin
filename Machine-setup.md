# Machine Setup

Things to do when setting up a new machine

## Downloads
- Chrome
- Firefox
- VS Code
- Sublime
- Docker
- Zoom
- Slack

## Settings
- Dock & Menu Bar: Enable "Automatically hide and show the Dock"
- Trackpad Point and Click: Enable secondary click with bottom right corner
- Trackpad Scroll and Zoom: Disable Scroll Direction: Natural
- Change battery settings
- Change screensaver settings

## Dev
- Install XCode from App Store
- Install XCode command line
```
xcode-select --install
```
- Install [Oh my zsh](https://ohmyz.sh/), make sure that the file .zshrc is exporting the below path at the top:
```
# Path to your oh-my-zsh installation
export ZSH="/Users/<USERNAME>/.oh-my-zsh"
```
- Install [Homebrew](https://brew.sh/)
- Install [Node and NVM](#node-setup)
- Install [git](#git-setup)
- Install Python if needed

## Node Setup
- Remove existing installations
```
brew uninstall --ignore-dependencies node
brew uninstall --force node
```
- Install NVM with brew
```
brew install nvm
```
- Create a directory in home folder
```
mkdir ~/.nvm
```
- Add config inside ~/.zshrc
```
export NVM_DIR="$HOME/.nvm"
[ -s "/opt/homebrew/opt/nvm/nvm.sh" ] && \. "/opt/homebrew/opt/nvm/nvm.sh"  # This loads nvm
[ -s "/opt/homebrew/opt/nvm/etc/bash_completion.d/nvm" ] && \. "/opt/homebrew/opt/nvm/etc/bash_completion.d/nvm"  # This loads nvm bash_completion
```
- Restart the terminal and run `nvm --version` to check
- Install the current LTS node version
```
nvm install --lts
```

## Git Setup
- Install git
```
brew install git
```
- [Create new Github SSH keys and connect to account](https://docs.github.com/en/authentication/connecting-to-github-with-ssh)
- Test ssh connection
```
ssh -T git@github.com
```
- Set github username and email
```
git config --global user.name "Amy Walker"
git config --global user.email "birdsandbutterflys@hotmail.com"
```
