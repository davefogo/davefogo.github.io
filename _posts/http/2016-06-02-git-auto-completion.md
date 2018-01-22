The shell’s auto-completion feature for directory and file names is amazing. Why couldn’t this also be possible for git? It is very cumbersome to write branch names over and over.
I searched online and found Bash git completion. I followed their guide and got git auto-completion up and running. It saves so much time. It makes pushing, merging and branching a breeze.

Here is a summary of how I did it for a Mac:

1. Install homebrew
2. Update home-brew
3. run

```
brew install bash-completion
```
(if you don’t have git installed already:)
```
brew install git && brew install bash-completion
```

4. Locate your .bash_profile found in your root (/Users/<account name>/.bash_profile)

5. Add to .bash_profile the following:

```
if [ -f $(brew — prefix)/etc/bash_completion ]; then
 . $(brew — prefix)/etc/bash_completion
 fi
 ```
 
 Credits: https://github.com/bobthecow/git-flow-completion/wiki/Install-Bash-git-completion
