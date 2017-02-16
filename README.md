# The Red Book

This document is guide on how we work at Red Panthers.

## create a new entry

To create a new entry we have created a rake task.

```sh
rake entry
```

It will ask you for the section id, class, title and priority number. The number decides the positon of the document
in the table of contents.

As per our internal convention numbers 

 * `1000 - 2999` will have the generate introduction & notes
 * `3000 - 8900` would have the various technical guidelines on coding
 * `9000 & beyond` would cover the non technical topics like project management, etc
