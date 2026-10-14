gh auth status
cd C:\Users\n_ase\thecut && gh repo create thecut --public --source=. --remote=origin --push
gh api repos/$(gh api user --jq .login)/thecut/pages -X POST -f source[branch]=master -f source[path]=/
