# Neon

> A vibrant Yazi flavor inspired by Tokyo's neon-lit nights

Neon is a stunning color scheme for [Yazi](https://github.com/sxyazi/yazi), the blazing-fast terminal file manager. Inspired by the electric glow of Tokyo's nighttime cityscape, Neon brings vibrant colors and exceptional file type differentiation to your terminal.

## Features

✨ **Vibrant Color Palette** - Eye-catching colors inspired by Tokyo's neon aesthetic
🎯 **Comprehensive File Type Support** - 100+ file extensions with meaningful color coding
🌙 **Hidden File Styling** - Dimmed, italicized dotfiles for reduced visual clutter
📁 **Smart Directory Colors** - Special colors for system, project, and user directories
🔧 **Developer-Focused** - Optimized colors for programming languages and config files
⚡ **High Contrast** - Easy-to-read selection and hover states
📅 **Smart Date Display** - Finder-style date/time formatting (English locale)

## Color Philosophy

Neon uses a carefully crafted color palette where each color serves a purpose:

- **Blue (#7aa2f7)** - Directories, TypeScript, C/C++
- **Orange (#ff9e64)** - Rust, Swift, Audio files
- **Yellow (#e0af68)** - JavaScript, JSON, Permissions
- **Green (#9ece6a)** - Executables, Tests, Databases
- **Purple (#bb9af7)** - Images, Kotlin, SCSS
- **Pink (#f7768e)** - Videos, HTML, Java, Archives
- **Cyan (#7dcfff)** - Go, Markdown, Documentation

## Installation

### Using ya (Recommended)

```bash
ya pkg add tomer-ben-david/neon
```

### Manual Installation

1. Clone this repository:
```bash
git clone https://github.com/tomer-ben-david/neon.yazi.git ~/.config/yazi/flavors/neon.yazi
```

2. Set the flavor in your `~/.config/yazi/theme.toml`:
```toml
[flavor]
dark = "neon"
```

3. (Optional) Enable the smart date display in your `~/.config/yazi/yazi.toml`:
```toml
[mgr]
linemode = "mtime"
```

## Special Features

### Smart Date Display
Neon includes a custom Finder-style date formatter that displays modification times in English:
- Files modified today: Show time only (e.g., "14:30")
- Files modified within 6 months: Show date and time (e.g., "Nov 17 14:30")
- Older files: Show date and year (e.g., "Jan 15  2024")

Enable it by setting `linemode = "mtime"` in your yazi.toml.

### Hidden Files
Hidden files (dotfiles) are rendered in dim gray with italic styling, making them less intrusive while still visible when needed.

### System Directories
- `.git/` - Bold red for visibility
- `node_modules/` - Dimmed green (less important)
- Build directories (`dist/`, `build/`, `target/`) - Yellow
- Cache directories - Dimmed gray

### Programming Languages
Each language gets its own distinctive color:
- Rust files glow in orange
- TypeScript shines in blue
- Python stands out in blue
- Go files appear in cyan
- And many more...

### User Directories
Your common directories get bold, vibrant colors:
- Downloads - Blue
- Documents - Cyan
- Pictures - Teal
- Music - Orange
- Videos - Pink

## Preview

![Neon theme preview](preview.png)

## Credits

- Created by [Tomer Ben David](https://github.com/tomer-ben-david)
- Inspired by the Tokyo Night color scheme
- tmTheme by Himanshu (MIT License)

## License

MIT License - See [LICENSE](LICENSE) for details

The included tmTheme file is also MIT licensed - See [LICENSE-tmtheme](LICENSE-tmtheme)
