# `alt-and-select` plugin

This plugin binds the alt-c (copy), alt-v (paste), alt-x (cut) keyboard shortcut to a commands: copy-region-as-kill, yank, kill-region.

Execute command is remaped to Alt-Shift-X.

Text selection in terminal Shift-arrows:

- Selection is cleared when using a navigation key (arrow, home, end) WITHOUT shift
- Backspace and Del delete an active selection
- Selection is extended to the next/previous word when using Ctrl+Shift+Left/Ctrl+Shift+Right
- Shift+Home and Shift+End extend the selection to the beginning and end of line respectively. Ctrl+Shift+Home and Ctrl+Shift+End do the same.


```zsh
plugins=(... alt-and-select)
```

## Installation with Oh My Zsh

Install using git clone.

```zsh
cd  ~/.oh-my-zsh/plugins && git clone https://github.com/raisty/alt-and-select.git
```

Or (alternative) download the file using wget.

```zsh
mkdir -p ~/.oh-my-zsh/plugins/alt-and-select && wget https://raw.githubusercontent.com/raisty/alt-and-select/master/alt-and-select.plugin.zsh -nc --no-dns-cache -O ->> ~/.oh-my-zsh/plugins/alt-and-select
```

Activate the plugin in Oh My Zsh (~/.zshrc)

```zsh
plugins=(... alt-and-select)
```
