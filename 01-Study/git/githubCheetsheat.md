---
id: githubCheetsheat
aliases: []
tags: []
---

# push neovim config

1. go to nvim config path
   git add .
   git commit -m "update"
   git push

# push current nvim config / obsidian notes

in current folder, eiter nvim config or obsidian vault check if correct by:
pwd
git status = wheither Git sees youre changes and which branch you are on
git branch = youre local branch
git remote -v = which which Github repo this folder is connected to for fetch/puch
look like:
origin https://github.com/Jimbolol13/nvim-config.git (fetch)
origin https://github.com/Jimbolol13/nvim-config.git (push)

git add.
git commit -m "UPDATE/change"
// branch is name of current branch
git push origin BRANCH

# push curernt nvim config/ obisidan notes

git pull origin YOUR-Branch
