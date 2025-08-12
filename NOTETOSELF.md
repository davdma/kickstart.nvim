# Note to Self

How I started using Kickstart neovim:
1. Familiarize with neovim/vim commands using `:Tutor`, as well the [neovim manual docs](https://neovim.io/doc/user/usr_toc.html#user-manual) which provide additional useful commands for movement etc. that is skipped in the tutorial
2. Using the following plugins: `telescope` for fuzzy finding, `nvim-tree` for file explorer, `LSP` language server protocol basics

For plugins use `<leader>` which is a special prefix for commands, this is by default set to `spacebar`. **For learning initially, just press `<leader>` and wait to see all available shortcuts you can use.**

Tips:
* For instance, for telescope file finding feature, press `<leader>sf` and then `<Enter>` at the file you find to switch `nvim` to that file.
* Instead of doing `:help~`, `<leader>sh` is easy to search help docs!

# LSPs

For getting the Language Server Protocol to work for your language of choice so you can have **Go To Definition** and **Go To Reference** commands, you must go into `init.lua` and modify the `local servers = {}` dictionary. Currently I have added python, C/C++ and Rust LSP but if you need other languages you must add them.
