# How to install this theme

```lua
--lazy with lualine theme included
    return{
    "Pair-of-dice/Alienocean.nvim",
    --Lualine theme can also be put in a separate file and not as a dependency
	dependencies = {
		"Pair-of-dice/Alienocean-lualine", --lualine theme
	},
    }
```

```lua
--lazy with configuration and lualine theme
return
{
  "Pair-of-dice/Alienocean.nvim",
  --Lualine theme can also be put in a separate file and not as a dependency
  dependencies = {
    "Pair-of-dice/Alienocean-lualine", --lualine theme
  },
  lazy = false,
  priority = 1000,
  opts = {
    overrides = { --Use this to change a certain highlight group
      normal = { fg = "#999999", bg = "#00001b", undercurl = true },
      ["@boolean"] = { link = "Special" },
    },
    allowTextStyling = true, -- When disabled all text styling such as bold,italic,strikethrough and undercurl are not displayed.
  },
  init = function()
    vim.cmd.colorscheme("Alienocean") --Sets the colourscheme to Alienocean on load
  end,
}
```

## Preview

## Special thanks

This is what this colourscheme is based on and what taught me how to do this.
<a href="https://github.com/xero/evangelion.nvim">Evangelion colourscheme</a>
Helped with providing the palette.
<a href="https://github.com/LunarVim/colorgen-nvim">colorgen-nvim</a>

## Other versions of this colourscheme

<a href="https://codeberg.org/ParadiseOfMagic/Alienocean-alacritty">Matching Alacritty colourscheme</a>
<a href="https://codeberg.org/ParadiseOfMagic/Alienocean-lualine">Lualine theme</a>
