# ClipStack - Clipboard History Manager

Never lose what you copied! ClipStack remembers everything you copy so you can find it later.

## Why ClipStack?

**The Problem:** System clipboard only remembers ONE thing
- Copy something new = lose the old
- No search, no history
- Accidentally overwrite important data
- Can't go back to something you copied hours ago

**The Solution:** ClipStack remembers everything
- Unlimited clipboard history
- Search through past copies
- Pin important items
- Auto-categorizes content
- Persists across reboots

## Installation

```bash
curl -sSL https://raw.githubusercontent.com/strabo231/clipstack/main/install.sh | bash
```

**Requirements:**
- `xclip` (Linux) or `pbcopy/pbpaste` (macOS)

```bash
# Ubuntu/Debian
sudo apt install xclip

# macOS (built-in)
# No installation needed
```

## Quick Start

```bash
# Start monitoring (run once)
clipstack watch &

# View history
clipstack

# Search for something
clipstack search "password"

# Copy item #5 back to clipboard
clipstack copy 5

# Pin important items
clipstack pin 3
```

## Commands

```
clipstack              Show clipboard history
clipstack search <q>   Search history  
clipstack copy <n>     Copy item to clipboard
clipstack pin <n>      Pin item permanently
clipstack pinned       Show pinned items
clipstack delete <n>   Delete item
clipstack clear        Clear all history
clipstack stats        Usage statistics
clipstack watch        Monitor clipboard (daemon)
```

## Features

📋 **Unlimited history** - Never lose a copy again  
🔍 **Full-text search** - Find anything instantly  
📌 **Pin favorites** - Keep important items forever  
🏷️ **Auto-categorize** - URLs, code, text, emails, etc.  
💾 **Persistent** - Survives reboots  
⚡ **Fast** - Instant search and retrieval  
📊 **Statistics** - See what you copy most  
🎨 **Beautiful output** - Color-coded types  

## Usage Examples

**Start monitoring:**
```bash
clipstack watch &
```

This runs in background and captures everything you copy.

**View history:**
```bash
clipstack
```

**Search history:**
```bash
clipstack search "api"
```

**Copy old item:**
```bash
clipstack copy 5
✓ Copied item 5 to clipboard
```

Now you can paste it anywhere!

**Pin important items:**
```bash
clipstack pin 3
✓ Pinned item 3
```

## Use Cases

- **Recover Lost Copy** - Accidentally copied over something important
- **Code Snippets** - Keep useful snippets accessible
- **Research & Writing** - Track sources you've copied
- **Multi-step workflows** - Copy multiple things, paste later

## Requirements

- Bash 4.0+
- `xclip` (Linux) or `pbcopy/pbpaste` (macOS)

## License

MIT License

## Author

Sean - [@strabo231](https://github.com/strabo231)

---

**Never lose what you copied. Ever.** 📋
