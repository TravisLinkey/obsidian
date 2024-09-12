
2024-09-09 19:41

Tags: [[Fixes]]

### Overview
I accidentally added files from my /Private folder in obsidian to my commit history. I really don't want these files on my public repo in github.

### Solution
`git reset --soft HEAD~4`

### Explanation
The `--soft` flag removed commits from my local, without overwriting the files locally. (I wanted the files still).

I needed the `HEAD~4` because there were already 4 local commits in my history that I wanted to remove. (Or squash)

### Source Material
- [Github solution](https://stackoverflow.com/questions/12481639/remove-file-from-latest-commit)
