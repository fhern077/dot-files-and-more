# Git Settings

## Add Git SSH KEY

```bash
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"

eval "$(ssh-agent -s)"

# If you're using macOS Sierra 10.12.2 or later, you will
#need to modify your ~/.ssh/config file to automatically
#load #keys into the ssh-agent and store passphrases in
# your keychain.

 Host *
  AddKeysToAgent yes
  UseKeychain yes
  IdentityFile ~/.ssh/id_rsa

ssh-add -K ~/.ssh/id_rsa

pbcopy < ~/.ssh/id_rsa.pub
```

## Global Git Ignore

1. Open Terminal.
2. Run touch ~/.gitignore_global - this will create global .gitignore file in your home directory.
   Add some values that you would like to always ignore.
3. Run git config --global core.excludesfile ~/.gitignore_global this command will make all the patterns from ~/.gitignore_global ignored in all  situations.
