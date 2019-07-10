# Installation

## Method 1

Copy the content of the [desert-night.Xresources](./desert-night.Xresources) into the `~/.Xresources` file and reload the settings with `xrdb`.

## Method 2

Add the following line to `~/.Xresources`:

```xdefaults
#include "/path/to/vim-color-desert-night/xresources/desert-night.Xresources"
```

## Method 3

Execute the following command:

```sh
xrdb -merge /path/to/vim-color-desert-night/xresources/desert-night.Xresources
```
