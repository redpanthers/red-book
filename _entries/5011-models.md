---
sectionid: models
sectionclass: h2
title: Model
is-parent: true
parent-id: ror
number: 5011
---

Default Scope

It creates a confusion, as we are not directly aware if there is a scope or not.

Don't Use

```
default_scope { order(created_at: :desc)}
```

Instead use

```
scope :feed, -> { order(created_at: :desc) }
```
and call the `model.feed` like `current_user.post.feed`.
