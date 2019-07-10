![](https://user-images.githubusercontent.com/37491630/60938548-de18cb00-a2c3-11e9-8a83-8d14b08b4381.png)

# Syntax Highlighting

The syntax highlighting is implemented by [zdharma/fast-syntax-highlighting](https://github.com/zdharma/fast-syntax-highlighting). By using `default` theme with any [terminal emulator color scheme](https://github.com/sainnhe/vim-color-desert-night#terminal-emulators) of desert-night, you can get a desert-night syntax highlighting theme of zsh.

# Prompt

The prompt theme is desert-night version of pure power, it depends on [romkatv/powerlevel10k](https://github.com/romkatv/powerlevel10k).

To use it, simply source this file in your zshrc after powerlevel10k has been load:

```zsh
source /path/to/vim-color-desert-night/zsh/.zsh-pure-power
```

Alternatively, if you are using [zplugin](https://github.com/zdharma/zplugin), you can install the theme like this:

```zsh
zplugin light romkatv/powerlevel10k
zplugin snippet https://github.com/sainnhe/vim-color-desert-night/blob/master/zsh/.zsh-pure-power
```

## Customization

There are three modes of this prompt theme:

```zsh
PURE_POWER_MODE=modern    # use nerdfont characters in the prompt
PURE_POWER_MODE=fancy     # use unicode characters in the prompt(default)
PURE_POWER_MODE=portable  # use only ascii characters in the prompt
```

To switch between them, edit `/path/to/vim-color-desert-night/zsh/.zsh-pure-power`, and change the value of `PURE_POWER_MODE`.
