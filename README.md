<h1 align="center">
𝐃𝐞𝐬𝐞𝐫𝐭 𝐍𝐢𝐠𝐡𝐭
</h1>

![](https://user-images.githubusercontent.com/37491630/60248245-be3fdb00-98b1-11e9-8619-680d8fa086be.png)

## Installation

### Via Plugin Manager

Take [vim-plug](https://github.com/junegunn/vim-plug) for example:

```vim
Plug 'sainnhe/vim-color-desert-night'
```

For better syntax highlighting support, please install [sheerun/vim-polyglot](https://github.com/sheerun/vim-polyglot).

### Manually

1. Clone this repository.
2. Copy `/path/to/vim-color-desert-night/colors/desert-night.vim` to `~/.vim/colors/desert-night.vim`
3. To install [lightline](https://github.com/itchyny/lightline.vim) theme, copy `/path/to/vim-color-desert-night/autoload/lightline/colorscheme/desert_night.vim` to `~/.vim/autoload/lightline/colorscheme/desert_night.vim`

## Usage

### Vim

Put this in your vimrc:

```vim
colorscheme desert-night
```

If you want to apply this color scheme temporarily, run this command in vim:

```vim
:colorscheme desert-night
```

#### Lightline

To enable [lightline](https://github.com/itchyny/lightline.vim) color scheme, put this in your vimrc:

```vim
let g:lightline = {}
let g:lightline.colorscheme = 'desert_night'

" or this line
let g:lightline = {'colorscheme' : 'desert_night'}
```

To apply it without reloading:

```vim
:let g:lightline.colorscheme = 'desert_night'
:call lightline#init()
:call lightline#colorscheme()
```

### Tmux Status Line

Check this [gist](https://gist.github.com/sainnhe/b8240bc047313fd6185bb8052df5a8fb).

### Zsh

- [Syntax Highlighting](https://github.com/sainnhe/vim-color-desert-night/tree/master/zsh#syntax-highlighting)
- [Prompt](https://github.com/sainnhe/vim-color-desert-night/tree/master/zsh#prompt)

### Terminal Emulators

- [Alacritty](./alacritty/README.md)
- [Kitty](./kitty/README.md)
- [Tilix](./tilix/README.md)

### Xresources

[README.md](./xresources/README.md)

## FAQ

**Q: It doesn't work as expected.**

**A:**

1. This color scheme is designed for true colors, `set termguicolors` is required. Check output of `vim --version`, maybe your vim doesn't support `termguicolors`

2. Maybe your terminal emulator doesn't support true colors, you can test it using [this script](https://unix.stackexchange.com/questions/404414/print-true-color-24-bit-test-pattern)

3. If you are running vim in tmux, you need to override default true colors of tmux, as tmux cannot display true color properly: [#1246 How to use true colors in vim under tmux?](https://github.com/tmux/tmux/issues/1246)

4. There are many highlighting group links in syntax files while a color scheme may change them, enabling one color scheme based on another color scheme enabled is very likely to cause color broken. If there is any color broken, you can enable the color scheme in your vimrc instead of after vim startup.

**Q: What's your status line configuration?**

**A:** check this [gist](https://gist.github.com/sainnhe/b8240bc047313fd6185bb8052df5a8fb).

## Contribution

This color scheme is generated by [lifepillar/vim-colortemplate](https://github.com/lifepillar/vim-colortemplate). To hack it, install this plugin and edit `templates/desert_night.colortemplate`, then rebuild the color scheme.

## Inspirations

[morhetz/gruvbox](https://github.com/morhetz/gruvbox)

[srcery-colors/srcery-vim](https://github.com/srcery-colors/srcery-vim)

[Marfisc/vorange](https://github.com/Marfisc/vorange)

## License

[MIT](./LICENSE) && [Anti-996](./Anti-996-LICENSE)
