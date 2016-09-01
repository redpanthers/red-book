---
sectionid: generators
sectionclass: h2
title: Skip Generators
is-parent: true
parent-id: generators
number: 5005
---

Rails by default generate a lot of un-necessary files when we run `rails g controller`. To avoid poluting our codebase with un-necessary files have the below code placed in the `application.rb` of your rails project.

```rb
config.generators do |g|
  g.helper false
  g.stylesheets false
  g.javascripts false
  g.view_specs false
end
```

You can read more about from our [blog](http://blog.redpanthers.co/customize-rails-auto-generation/).