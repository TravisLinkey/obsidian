
2024-07-28 16:34

Tags: [[Deployment]] | 

### Overview
The references linked will help you deploy an Obsidian plugin.

Scroll down to `Releasing new releases`

### Steps

1. Update `manifest.json` with new `version`
2. Update `versions.json` file with same version as Step 1
3. Create GitHub commit with a tag of new version used in Step 1 and 2:
	- `git add .`
	- `git commit -m "feat: new version"`
	- `git tag <version-number>`
	- `git push origin main`
	- `git push origin master --tags`

4. Navigate to GitHub and create a release for the newly created tag:
	- Upload the following files:
		- `main.js`
		- `manifest.json`
		- `styles.css`
		- .zip file for the build

### References
- [Sample Plugin GitHub](https://github.com/obsidianmd/obsidian-sample-plugin)

- [Youtube video explainer](https://www.youtube.com/watch?v=AgXa03ZxJ88)

