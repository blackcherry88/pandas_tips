# Neovim Kickstart Tutorial: Essential Operations

## Getting Started

Your Neovim setup uses **Kickstart.nvim** - a modern, well-documented configuration. The leader key is `<space>`.

## 1. Discovery & Help

**Most Important**: Press `<space>` and wait - which-key shows all available commands!

- `<space>sh` - Search help documentation
- `<space>sk` - Search keymaps
- `;` - Enter command mode (mapped from `:`)

## 2. File Operations

### Opening Files
- `<space>sf` - Find files (fuzzy search)
- `<space>s.` - Recent files
- `<space>sn` - Open Neovim config files

### Buffer Management
- `<space><space>` - Switch between open buffers
- `:w` - Save file
- `:q` - Quit
- `:wq` - Save and quit

## 3. Navigation & Search

### Text Search
- `<space>sg` - Live grep (search in all files)
- `<space>sw` - Search current word under cursor
- `<space>/` - Search in current buffer
- `<Esc>` - Clear search highlights

### Code Navigation (LSP)
- `grd` - Go to definition
- `grr` - Find references
- `grn` - Rename symbol
- `gra` - Code actions
- `gO` - Document symbols

## 4. Window Management

### Creating Splits
- `:split` or `:sp` - Horizontal split
- `:vsplit` or `:vs` - Vertical split

### Navigation
- `<space>wh` - Move to left window
- `<space>wj` - Move to bottom window
- `<space>wk` - Move to top window
- `<space>wl` - Move to right window

### Resizing
- `<C-w>=` - Equal size windows
- `<C-w>>` - Increase width
- `<C-w><` - Decrease width
- `<C-w>+` - Increase height
- `<C-w>-` - Decrease height

## 5. Terminal Integration

### Using Terminal
- `:terminal` - Open terminal
- `<Esc><Esc>` - Exit terminal mode to normal mode
- `:!git status` - Run git commands

### Git Integration
- Visual indicators: `+` (added), `~` (changed), `_` (deleted) in gutter
- `<space>h` - Git hunk operations (stage, reset, preview)

## 6. Code Features

### Formatting & Completion
- `<space>f` - Format code
- `<C-y>` - Accept completion (in insert mode)
- `<C-space>` - Open completion menu

### Diagnostics
- `<space>sd` - Search diagnostics
- `<space>q` - Open diagnostic quickfix list

## 7. Configuration Management

### Reloading Config
- `:source %` - Reload current file (if editing init.lua)
- `:source ~/.config/nvim/init.lua` - Full reload
- `:Lazy sync` - Update plugins

### Plugin Management
- `:Lazy` - Open plugin manager
- `:Mason` - Manage language servers

## 8. Essential Vim Motions

### Basic Movement
- `hjkl` - Left, down, up, right
- `w` - Next word
- `b` - Previous word
- `0` - Start of line
- `$` - End of line

### Editing
- `i` - Insert mode
- `a` - Append after cursor
- `o` - New line below
- `dd` - Delete line
- `yy` - Copy line
- `p` - Paste

## Quick Workflow Examples

### Opening a Project
1. `nvim` - Start Neovim
2. `<space>sf` - Find files
3. Type filename, press Enter

### Code Navigation
1. Place cursor on function/variable
2. `grd` - Go to definition
3. `<C-o>` - Jump back

### Git Workflow
1. See changes in gutter (`+`, `~`, `_`)
2. `<space>h` - Stage/reset hunks
3. `:!git commit -m "message"` - Commit
4. `:!git push` - Push

### Search & Replace
1. `<space>sg` - Search text across files
2. `<space>sw` - Search word under cursor
3. `:%s/old/new/g` - Replace in current file

## Pro Tips

1. **Always start with `<space>`** - let which-key guide you
2. **Use Telescope for everything** - files, buffers, help, symbols
3. **Learn one feature at a time** - don't try to memorize everything
4. **Read the comments** in your init.lua - they explain everything
5. **Use `:help <topic>`** when stuck

## Key Features of Your Setup

### Plugins Included
- **Telescope** - Fuzzy finder for files, text, and more
- **LSP with Mason** - Language server support with auto-installation
- **Blink.cmp** - Modern autocompletion
- **Treesitter** - Syntax highlighting and code understanding
- **Gitsigns** - Git integration with visual indicators
- **Which-key** - Keymap discovery and help
- **Mini.nvim** - Collection of useful utilities

### Custom Mappings
- `;` mapped to `:` for easier command entry
- `<Esc><Esc>` to exit terminal mode
- Relative line numbers enabled
- Smart case searching
- Auto-formatting on save

This setup gives you a modern IDE experience while teaching you Vim fundamentals. Start with file navigation and gradually add more features to your workflow.