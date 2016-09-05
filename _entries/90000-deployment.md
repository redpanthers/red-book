---
sectionid: deployment
sectionclass: h1
title: Deployment
number: 90000
is-parent: yes
---

Even though we use CodeShip/Circle CI/Jenkins for continuous integration, we still need to write scripts to automate our deployment. We also need to write small commands to clear cache, restart queues, etc. It's always a good practice to not have to enter the server directly but to have it done through scripts. There are many tools available for this purpose (in multiple languages) like Capistrano, Vlad, etc.

Mina is a similar tool, but faster. The reason why it runs faster is because it generates a bash script, upload it to the server and run there than creating a new ssh session and run every command one by one. Mina is one of our default tools at Red Panthers.

To use mina in your project, add mina to your Gemfile.

```
gem 'mina'
```

and to get started do


```
mina init
``
I am not going to be taking more details on how to get started or use mina, which can be learned from their [documentation](http://nadarei.co/mina/setting_up_a_project.html). Digital Ocean has written a good [article](https://www.digitalocean.com/community/tutorials/how-to-deploy-with-mina-getting-started) about it as well.


* Our code should be able to be deployed in a single command
* Our tool of choice for this purpose is [mina](http://nadarei.co/mina/)
