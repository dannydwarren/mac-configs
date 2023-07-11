# mac-configs

Steps to getting my MacOS ready for dev.

1. Terminal
  - Install git and MacOS dev tools: `git`
  - Install brew: `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
  - Install iterm2: `brew install --cask iterm2`
1. iTerm
  - Install Git Credential Manager (gcm)
    ```
    brew tap microsoft/git
    brew install --cask git-credential-manager-core
    ```
  - Install VS Code: `brew install --cask visual-studio-code`
1. Docker [for Mac](https://docs.docker.com/desktop/install/mac-install/)
   - [Download Docker Desktop Installer](https://desktop.docker.com/mac/main/amd64/Docker.dmg?utm_source=docker&utm_medium=webreferral&utm_campaign=docs-driven-download-mac-amd64&_gl=1*11tg1v6*_ga*NjU1NTc3OTAwLjE2ODkxMTA3Mzg.*_ga_XJWPQMJYHQ*MTY4OTExMDczOC4xLjEuMTY4OTExMDkxNS41MS4wLjA.)
   - ```
     cd ~/downloads
     sudo hdiutil attach Docker.dmg
     sudo /Volumes/Docker/Docker.app/Contents/MacOS/install
     sudo hdiutil detach /Volumes/Docker
     ```
