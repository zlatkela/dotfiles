# dotfiles

## Installation

1. Install [Homebrew](http://brew.sh) with the instructions from their website
2. Run `brew install ansible`
3. Run `git clone https://github.com/3AP-AG/dotfiles.git ~/Projects/.dotfiles`
4. Run `cd ~/Projects/.dotfiles`
5. Run `cp host_vars/localhost.yml.dist host_vars/localhost.yml`
6. Adjust variables in `host_vars/localhost.yml`
7. Run `ansible-playbook site.yml --diff --ask-become-pass`

Hint: you might want to uncomment the section "- name: install apps from app store", some of those apps are not free and there are a couple of errors from the app store if it cannot install them, therefore best manually install them in the app store, when you really need them
