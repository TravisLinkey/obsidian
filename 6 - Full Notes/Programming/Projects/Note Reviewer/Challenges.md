
2024-07-21 16:33

Tags: [[6 - Full Notes/Projects/Note Reviewer/Note Reviewer]]

### Requirements

This plugin has a need for storage for various data. Such as:
    - When a note was last reviewed
    - If a note is bookmarked
    - If a note should not be reviewable
    - etc.

Additionally, I need a way to filter through notes that share the same Tag so that I can display related notes for review.

### Challenges

I do not want to open up this plugin to making server calls to a DB, so this limits me to storing note data and metadata locally. Additionally, these plugins are clientside code, and do not have access to various SQL implementations for data storage.

### Solution

After some research, I have come to discover [[RxDB]], which should help storing data locally and add query functionality for the front end application.

### References
- [[6 - Full Notes/Projects/Note Reviewer/Note Reviewer]]
- [RxDB Link](https://rxdb.info/)

