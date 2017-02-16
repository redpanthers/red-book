---
sectionid: editor-config
sectionclass: h2
title: Editor Configuration
parent-id: setup
number: 4020
---

Make sure you have configured your editor to maintain a consistent coding style. When sending pull requests, we shouldn't have basic problems like inconsistent indentation.

For Ruby, we follow [bbatsov/ruby-styleguide](https://github.com/bbatsov/ruby-style-guide#source-code-layout).

**Sublime**

```json
# Preferences > Settings - User
{
  "tab_size": 2,
  "translate_tabs_to_spaces": true,
  "trim_trailing_white_space_on_save": true,
  "rulers": [79],
  # ...
}
```

**Vim**

```vimscript
set shiftwidth=2
set tabstop=2
set expandtab
```

Apart from the basic settings above, you can also use the [vim-ruby](https://github.com/vim-ruby/vim-ruby) plugin to get smart indentation and other helpful features.

**VS Code**

```json
# File > Preferences > User Settings:
{
  "editor.tabSize": 2,
  "editor.insertSpaces": true,
  # ...
}
```
