
2024-08-19 16:32

Tags: [[Interview]] | [[Personal Projects]]

### Overview
Wanted a way to help review subjects I was studying and help knowledge retention.

I use Obsidian to take notes.

### Idea
- Create an Obsidian Plugin that will help with knowledge retention
- Model it after `Github Notifications`.

### Challenges
- Needed persistant storage to track file system state.
- Plugin could not make server calls, (could not just store everything in a database)

### Solution 
- Used npm module [[RxDB]], to store file system details, (file location, tags, etc).

- A local state file to track files added / removed / changed events.
    - These events would trigger a PUT or DELETE on the [[RxDB]] database.

### Nice Features
- Can filter notes based on custom `Tags` that are added to the top of your files.

- Plugin would scan the file once it is modified and store near-realtime data about tags and files.

### References
- [[Note Reviewer]]

