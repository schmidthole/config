# neovim config

## general settings

- **leader key:** `Space`
- **theme:** rose-pine
- **line numbers:** relative
- **clipboard:** synced with system
- **indentation:** 4 spaces (2 for web filetypes)
- **search:** case-insensitive with smart case
- **undo:** persistent across sessions
- **splits:** open right and below

## language servers

| language              | server  |
|-----------------------|---------|
| go                    | `gopls` |
| python                | `pylsp` |
| typescript/javascript | `ts_ls` |

---

## keybinding cheatsheet

### general

| key          | action               |
|--------------|----------------------|
| `<Esc>`      | clear search highlight |
| `<Space>j`   | format json with jq  |

### navigation (lsp)

| key         | action              |
|-------------|---------------------|
| `gd`        | go to definition     |
| `gD`        | go to declaration    |
| `gr`        | go to references     |
| `gI`        | go to implementation |
| `<Space>D`  | type definition      |
| `K`         | hover documentation  |

### lsp actions

| key          | action       |
|--------------|--------------|
| `<Space>rn`  | rename symbol |
| `<Space>ca`  | code action  |

### fzf-lua

| key     | action                      |
|---------|-----------------------------|
| `C-p`   | find files                  |
| `C-g`   | live grep (search in files) |

**inside fzf window:**

| key         | action                        |
|-------------|-------------------------------|
| `Enter`     | open file                     |
| `C-s`       | open in horizontal split      |
| `C-v`       | open in vertical split        |
| `C-t`       | open in new tab               |
| `Tab`       | toggle selection              |
| `S-Tab`     | toggle selection (reverse)    |
| `C-j / C-k` | move up/down in results      |
| `C-d / C-u` | scroll preview down/up       |
| `C-q`       | send results to quickfix list |
| `Esc`       | close                         |

### completion (nvim-cmp)

| key        | action                       |
|------------|------------------------------|
| `C-Space`  | trigger completion menu      |
| `C-n`      | next item                    |
| `C-j`      | previous item                |
| `Tab`      | next item / expand snippet   |
| `S-Tab`    | previous item / jump back    |
| `Enter`    | confirm selection            |
| `C-d`      | scroll docs up               |
| `C-f`      | scroll docs down             |

### commenting (comment.nvim)

| key    | mode     | action                    |
|--------|----------|---------------------------|
| `gcc`  | normal   | toggle line comment       |
| `gbc`  | normal   | toggle block comment      |
| `gc`   | visual   | toggle line comment       |
| `gb`   | visual   | toggle block comment      |
| `gcO`  | normal   | add comment above         |
| `gco`  | normal   | add comment below         |
| `gcA`  | normal   | add comment at end of line |

