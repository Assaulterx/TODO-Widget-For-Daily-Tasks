# ASSAULTER-X v3.1
A lightweight, terminal-based task scheduler for Windows and Linux systems with persistent storage and daily resets.

## Features

- **Floating Terminal Widget**: Minimal, always-on-top task management interface
- **Quick Task Addition**: Type and press ENTER to add tasks instantly
- **Toggle Status**: Click tasks to mark them complete/incomplete
- **Daily Reset**: Tasks automatically reset daily for a fresh start
- **Persistent Storage**: All tasks saved to JSON locally
- **Dark Theme**: Eye-friendly terminal aesthetic with accent colors
- **Move Mode**: Drag the widget around your screen
- **Right-Click Menu**: Quick access to edit, delete, and system controls
- **Auto-Startup**: Configure to launch with your system (Windows & Linux)

## How can I use this?

### Use Lovable
Simply visit the [Lovable Project](https://lovable.dev) and start prompting. Changes made via Lovable will be committed automatically to this repo.

### Use your preferred IDE
If you want to work locally using your own IDE, you can clone this repo and push changes. Pushed changes will also be reflected in Lovable.

The only requirement is having Node.js & npm installed - [install with nvm](https://github.com/nvm-sh/nvm)

Follow these steps:

```bash
# Step 1: Clone the repository using the project's Git URL.
git clone <YOUR_GIT_URL>

# Step 2: Navigate to the project directory.
cd <YOUR_PROJECT_NAME>

# Step 3: Install the necessary dependencies.
npm i

# Step 4: Start the development server with auto-reloading and an instant preview.
npm run dev
```

## Setup Instructions

### For Windows Users

#### The Executable
1. Install Python and run `pip install pyinstaller`
2. Convert to EXE: Run this command
   ```bash
   pyinstaller --onefile --noconsole assaulterx.py
   ```
3. Auto-Startup
   - Press `Win + R`, type `shell:startup`
   - Copy the `.exe` from the `dist` folder and paste as shortcut into the startup folder

### For Linux Users

#### The Script
1. Install dependencies
   ```bash
   sudo apt install python3-tk
   ```
2. Set permissions
   ```bash
   chmod +x assaulterx.py
   ```
3. Auto-Startup
   - Create `.config/autostart/assaulter.desktop` and add:
   ```ini
   [Desktop Entry]
   Type=Application
   Exec=/path/to/assaulterx.py
   Hidden=false
   NoDisplay=false
   X-GNOME-Autostart-enabled=true
   ```

## Control Interface

| Action | Keys |
|--------|------|
| **Move Widget** | Hold `Shift` + Left-Click Drag |
| **Add Task** | Type in box and press `ENTER` |
| **Toggle Status** | Left-Click on any task |
| **Manage/Exit** | Right-Click on any task |
| **Toggle Overlap (Stay on Top)** | `Ctrl + T` |

### Right-Click Menu Options
- **PIN/UNPIN**: Keep window on top or float freely
- **EDIT**: Modify task text
- **DELETE**: Remove task
- **EXIT SYSTEM**: Close application

## Application Status Indicators

- **PINNED**: Window stays on top of all others
- **FLOATING**: Window behaves like normal window
- **MOVEMODE**: Drag mode active (hold Shift)
- **SYSLOCKED**: Normal mode (no dragging)

## File Structure

```
ASSAULTER-X/
├── assaulterx.py          # Main application file
├── README.md              # This file
└── [Windows]
    └── dist/
        └── assaulterx.exe # Compiled executable
```

## Data Storage

Tasks are stored in JSON format at:
- **Windows**: `%LOCALAPPDATA%/AssaulterX/terminaltasks.json`
- **Linux**: `~/.local/share/appdata/AssaulterX/terminaltasks.json`

## Requirements

- **Python**: 3.6+
- **tkinter**: Included with Python on most systems
- **Node.js & npm**: For development environment (if using Lovable/IDE)

## License

MIT License - Feel free to use and modify for your personal or professional projects.

## Support

For issues, suggestions, or feature requests, please open an issue on GitHub or contact the maintainer.
piyushpjamdhade@gmail.com

---

**Made with ❤️ for productive developers**

