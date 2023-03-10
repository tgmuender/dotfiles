# Setup

Inspired by:

- https://news.ycombinator.com/item?id=11071754 
- https://www.atlassian.com/git/tutorials/dotfiles

```sh
$ git init --bare ~/.dotfiles/.git    
$ dotfiles='git --git-dir=${HOME}/.dotfiles/.git --work-tree=${HOME}'
$ dotfiles config status.showUntrackedFiles no

```

Use on a new host:

```sh
$ git clone --bare git@github.com:tgmuender/dotfiles.git $HOME/.dotfiles/.git
$ alias dotfiles='git --git-dir=${HOME}/.dotfiles/.git --work-tree=${HOME}'
$ dotfiles checkout

```

