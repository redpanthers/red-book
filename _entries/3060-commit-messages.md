---
sectionid: commit-messages
sectionclass: h2
title: Commit
parent-id: git
number: 3060
---

Git commit message is an important piece of information that explains to the reader why or what the change of code was about.

It is important to note that you don't write git commit messages for yourself, but to other who would be reading it during 
code review or later in future.

So kindly follow these simple rules while commiting:

* Do not write the commit in past tense
* Use short git message, say 50 characters
* Use multi line commits, if you want to exceed 50 characters
* It should explain what it is changing/adding

To make the git commit easier or more recognizable, we use a couple of tags in the git messages. So if you prefix these tags before
the commit message it would convey more meaning.


* **[UI]** - commit only has UI changes
* **[DB]** - commit is reference to a migration
* **[HotFix]** - this commit was urgently required to have been commited and send to production