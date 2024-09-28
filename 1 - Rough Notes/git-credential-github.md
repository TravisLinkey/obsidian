
2024-09-28 11:10

Tags: [[Arch]]

### Overview
1. You need to clone the github repo then `cd` into it, build and run:
`makepkg -si`

2. Add the following to your `~/.gitconfig`
```bash
[credential "https://github.com"]
  helper = cache
  helper = github # important that you put it last because we only need to run gcg when other helpers have failed to give credentials
```

3. Attempt to push to repo. (`git push`)

4. Follow the instructions to add your device.

5. Should work

### Source Material
- [AUR link](https://aur.archlinux.org/packages/git-credential-github)
- [Github link](https://github.com/Xgames123/git-credential-github)
