# dotfiles

Personal configuration shared between machines.

## Git aliases

`git/aliases.gitconfig` holds my git aliases. To use them on a new machine:

```sh
gh repo clone jacobgrevstad/dotfiles ~/dotfiles
git config --global include.path "~/dotfiles/git/aliases.gitconfig"
```

### `git recent`

Branches ordered by when I last switched to them (from the HEAD reflog), numbered from 0 (0 = current branch).

| Command | Does |
|---|---|
| `git recent` | List the last 5 branches |
| `git recent 10` | List the last 10 |
| `git recent -3` / `git recent ---` | Switch to entry 3 |
| `git recent -` | Switch to entry 1 (the previous branch) |
