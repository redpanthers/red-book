---
sectionid: exceptions
sectionclass: h2
title: Handelling Exceptions
parent-id: ror
number: 5049
---

No matter how much we plan, there will always occur cases which we can't preplan. It mostly happen stuff that is not under our control like

1. User Input
2. 3rd Party API
3. Network

So while working with the above three it is always better to lead with caution.

Always use `try` if you are doublt ful about an object. 

```rb
@person = Person.where(name: 'Panther').first
@person.try?(:name)
```

You can also pass in code blocks in try

```rb
report = params[:search_param]
.try { |term| build_search_query(term) }
.try { |formated_term| run_search(formated_term) }
```