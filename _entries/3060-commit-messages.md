---
sectionid: commit-messages
sectionclass: h2
title: Commit Messages
parent-id: git
number: 3060
---

Git commit messages
are an important piece of information
that explain to the reader
why or what the change of code was about.

It is important to note that you don't write git commit messages for yourself,
but for others
who will read it during code review
or later in future.

Follow these simple rules while commiting:

* Use short git message, say 50 characters
* Do not write the commit in past tense
* Use multi line commits, if you want to exceed 50 characters
* It should explain what it is changing/adding

To make the git commit easier or more recognizable,
we use a couple of tags in the git messages,
to convey more meaning about them:

* **[UI]** - commit only has UI changes
* **[DB]** - commit is reference to a migration
* **[HotFix]** - this commit was urgently required in production
