
## Commit to GitHub using ssh key
1. generate ssh public/private keys
2. put public key to github.com
3. run `ssh -T git@github.com` to check if public key works
4. under repo dir run `git remote set-url origin git@github.com:<user>/<project>.git`
5. git push
