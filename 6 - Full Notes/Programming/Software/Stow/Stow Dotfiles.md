
2024-08-30 17:05

### Steps
1. Copy the files over into your `~/.dotfiles` directory the same way they exist in your file system.
2. Rename the original file to a temporary filename so `stow` command can work.
3. Change into the `~/.dotfiles` directory and run `stow .`

4. Verify this worked by running `ls -lah <file-name>` on the file you wished to stow. You should see it is a [[Symbolic Link]] to the file in our `~/.dotfiles` directory.

### Source Material
- [Youtube Link](https://www.youtube.com/watch?v=y6XCebnB9gs&list=PL9LLGJsP6hXjVCsMY4GSXpeR9R2v9bfXr&index=2)

