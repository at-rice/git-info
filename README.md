# git-info

info for git

```
[filter "lfs"]
	clean = git-lfs clean -- %f
	smudge = git-lfs smudge -- %f
	process = git-lfs filter-process
	required = true
[user]
	name = __
	email = __
[core]
	excludesfile = $HOME/.gitignore_global
	editor = code --wait
[difftool "sourcetree"]
	cmd = opendiff \"$LOCAL\" \"$REMOTE\"
	path = 
[commit]
	template = $HOME/.stCommitMsg
[pull]
  rebase = true
[push]
	default = simple
[color]
  ui = auto
[alias]
  lg = log --graph --pretty=format:'%C(red)%h%Creset%C(yellow)%d%Creset %C(bold blue)%an%Creset %C(green)%cr%Creset %s' --abbrev-commit --date=relative --all
  lg2 = log --graph --pretty=format:'%C(red)%h%Creset%C(yellow)%d%Creset %C(bold blue)%an%Creset %C(green)%cr%Creset %s' --abbrev-commit --date=relative


