# Git notes

## Commit to GitHub using ssh key
1. generate ssh public/private keys
2. put public key to github.com
3. run `ssh -T git@github.com` to check if public key works
4. under repo dir run `git remote set-url origin git@github.com:<user>/<project>.git`
5. git push

## Status
```bash
git status -u  # show individual files in untracked directories
```

## Set configuration params
```bash
# check current values
git config user.name
git config user.email

# individual repo
git config user.name "Your Name"
git config user.email your@email.com

# global User name and Email (~/.gitconfig)
git config --global user.name "Your Name"
git config --global user.email your@email.com
```

