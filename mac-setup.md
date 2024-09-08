## Trackpad
- Point & Click
  - Enable Tap to click with one finger
  - Change Secondary click to right corner
  - Uncheck Three finger drag
- Scroll & Zoom
  - Uncheck all apart from Zoom in and out


## Finder
- General
  - Change New finder window show to open in your Home Directory
- Sidebar
  - Add Home and your Code Directory
  - UNcheck all Shared boxes


## MenuBar
- Remove Display and Bluetooth icons
- Change battery to Show percentage symbols


## User Defaults
- Create the folder where you'd like to store your screenshots: `mkdir ~/Documents/screenshots`
- Then run the following command: `defaults write com.apple.screencapture location ~/Documents/screenshots && killall SystemUIServer`
- Settings -> Privacy & Security -> Secruity -> Allow applications downloaded from App Store and identitfied developers


## XCode
- `xcode-select --install`. It'll prompt you to install the command line tools. Follow the instructions and you'll have Xcode and Xcode command line tools both installed.

## Homebrew
- `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`


## Git
- Your computer comes with a Git but might be an older version. First get its version and location, so later you know you are using the newly-installed version.
- Do `brew install git` to get the latest version. Then do `git --version` to test that it is installed and use `which git` got check the correct location.
- Depending on your context, you might need to define your git user.
```
git config --global user.name "Your Name Here"
git config --global user.email "your_email@youremail.com"
```
- You may also need to set up SSH with GitHub.

### gitignore
- You may or may not need to do this. This is to set a default version of your gitignore file. Check this: https://sourabhbajaj.com/mac-setup/Git/gitignore.html.


## Zsh
- `brew install zsh`
- Install Oh My Zsh. Check this: https://github.com/ohmyzsh/ohmyzsh.
  - Example plugins: 
`plugins=(git aliases vi-mode colorize colored-man-pages zsh-autosuggestions zsh-syntax-highlighting)`
  - Use this themem: https://github.com/romkatv/powerlevel10k.
  - After the install, run `cat ~/.zshrc.pre-oh-my-zsh >> ~/.zshrc && source ~/.zshrc` to bring back the previous settings in the zshrc file.



## Vim
- Get the latest version through `brew install vim`. Make sure your vim command directs to the version installed by brew.


## Java



## Go
Can be installed via `brew install go`. Then use `go version` to see the installed version.



## Other Plugins/Apps
- Karabiner-Elements
  - Complex Modifications: Check CAPS related 3 options (page down/up, hjkl)
- Rectangle
  - to move windows among screens easily
- Customize terminal


# Zshrc
```
alias dc='cd'
alias rm='rm -i' 
setopt HIST_IGNORE_SPACE 

```


# Homebrew
Install the below apps
- autojump and add `[ -f /opt/homebrew/etc/profile.d/autojump.sh ] && . /opt/homebrew/etc/profile.d/autojump.sh1` to zshrc file
- tree
- tmux
- fzf