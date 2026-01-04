# Tmux Configuration

Personal tmux configuration with session persistence and vim-style navigation.

## Key Bindings

Prefix: `Ctrl-b`

### Windows

| Key | Action |
|-----|--------|
| `F1`-`F10` | Switch to window 1-10 |
| `F11`/`F12` | Toggle last window |

### Panes

| Key | Action |
|-----|--------|
| `prefix + \|` | Split horizontally |
| `prefix + -` | Split vertically |
| `prefix + h/j/k/l` | Navigate panes (vim-style) |
| `prefix + o` | Next pane |
| `prefix + ;` | Previous pane |

### Copy Mode

| Key | Action |
|-----|--------|
| `prefix + [` | Enter copy mode |
| `prefix + ]` | Paste buffer |
| `y` (in copy mode) | Copy to system clipboard (Wayland) |

### Session Management

| Key | Action |
|-----|--------|
| `prefix + Ctrl-s` | Save sessions |
| `prefix + Ctrl-r` | Restore sessions |
| `prefix + r` | Reload config |

## Plugins

Managed via [TPM](https://github.com/tmux-plugins/tpm).

- **tmux-resurrect** - Save and restore tmux sessions across restarts
- **tmux-continuum** - Auto-save sessions every 15 minutes, auto-restore on start
- **tmux-prefix-highlight** - Highlight status bar when prefix is active

### Install Plugins

```bash
# In tmux
prefix + I

# Or via command line
~/.config/tmux/tpm/bin/install_plugins
```

## Settings

- Mouse support enabled
- Vi-style keys in copy mode
- History limit: 10000 lines
- Window/pane indexing starts at 1
