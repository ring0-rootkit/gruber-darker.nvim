# NOTE
This is a fork of this repo https://github.com/ring0-rootkit/gruber-darker.nvim
I've changed some colors to suit my needs, but you are welcome to use that and contribute.
(I've made popup windows darker than in original repo)

# My custom additions
## darker white (i have Astigmatism so it helps me to read better)`

![image](https://github.com/ring0-rootkit/gruber-darker.nvim/assets/111735837/f443d5f9-239d-4afe-a78a-b3ba8f65d1c3)

## darker popup windows

![image](https://github.com/ring0-rootkit/gruber-darker.nvim/assets/111735837/bc21dc45-85fe-4768-b059-42fbaa32fc22)

`ORIGINAL for comparison`

![image](https://github.com/ring0-rootkit/gruber-darker.nvim/assets/111735837/0b990766-b937-4dc7-8689-d22ba9ae7840)

# gruber-darker.nvim

_A modern Neovim port of a deftheme [adaptation][gruber-darker-theme] of an Emacs
[port][gruber-darker] of a BBEdit [colorscheme][gruber-dark]_

> **Note**
> This is a work in progress, but fairly stable

![image](https://user-images.githubusercontent.com/9439488/229402983-b27a2fc4-d938-4ed0-8f7f-7711f73aa985.png)

## Installation

### Lazy (recommended)

```lua
{ "ring0-rootkit/gruber-darker.nvim" }
```

### Packer

```lua
use "ring0-rootkit/gruber-darker.nvim"
```

### Plug

```vim
Plug 'ring0-rootkit/gruber-darker.nvim'
```

Then, somewhere in your `init.lua`, set the colorscheme

```lua
vim.cmd.colorscheme("gruber-darker")
```

## Configuration

### Defaults

```lua
{
  bold = true,
  invert = {
    signs = false,
    tabline = false,
    visual = false,
  },
  italic = {
    strings = true,
    comments = true,
    operators = false,
    folds = true,
  },
  undercurl = true,
  underline = true,
}
```

### With updated preferences

Change configuration options by calling `setup()`
prior to loading the colorscheme. Your preferences
will be merged with the defaults.

For example, with [Lazy](https://github.com/folke/lazy.nvim.git)...

```lua
{
  "ring0-rootkit/gruber-darker.nvim",
  opts = {
    bold = false,
    italic = {
      strings = false,
    },
  },
}
```

## Credits

These repositories were great knowledge sources and their
inspiration helped immensely with the development of this plugin.

- [rexim/gruber-darker-theme][gruber-darker-theme]
- [folke/tokyonight.nvim][tokyonight]
- [drsooch/gruber-darker-vim][gruber-darker-vim]

[gruber-darker-theme]: https://github.com/rexim/gruber-darker-theme
[gruber-darker]: https://jblevins.org/projects/emacs-color-themes/gruber-darker-theme.el.html
[gruber-dark]: http://daringfireball.net/projects/bbcolors/schemes/
[tokyonight]: https://github.com/folke/tokyonight.nvim
[gruber-darker-vim]: https://github.com/drsooch/gruber-darker-vim
