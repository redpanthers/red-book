---
sectionid: branch
sectionclass: h2
title: Branch
parent-id: git
number: 3055
---

A branch represents an independent line of development. It lets you work on your idea, while not corupting or mutating the existing
stable work. Every project we undertake would have three main branches. 

* **master** - Master has stable and working code, its the most up to date branch. We merge all our bug fixes and features to master
* **staging** - It has the code which we have in the staging server. It should only have commits which are from master. We should never directly commit to staging.
* **production** - It has the code which is live in the production server. It should only have commits which are from master. We should never directly commit to production.


**Naming a branch**

When you are working on a feature, you should use the prefix `feat_`, to the name of the branch.

Eg:- If you are working a feature called user authentication, then the branch should be called `feat-user_authentication`.


When you are working on a bug fix, you should use the prefic `fix_`, to the name of the branch.

Eg:- If you are working on a bug fix on user profile, then the branch should be called: `fix-user_profile`