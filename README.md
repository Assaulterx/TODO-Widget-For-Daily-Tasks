# TODO-Widget-For-Daily-Tasks


SETUP STEPS FOR TODO LIST PYTHON APP FOR LOCAL DEVICES: For Windows Users (The Executable)
1.
Install Python and run: pip install pyinstaller

2.
Convert to EXE: Run this command: pyinstaller --onefile --noconsole assaulter_x.py

4.
Auto-Startup:

o
Press Win + R, type shell:startup.

o
Copy the .exe from the dist folder and paste as shortcut into the startup folder.

For Linux Users (The Script)

1.
Dependency: sudo apt install python3-tk

3.
Permissions: chmod +x assaulter_x.py

5.
Auto-Startup: Create ~/.config/autostart/assaulter.desktop and add:

Control Interface Summary

•
Move Widget: Hold Left SHIFT + Left-Click Drag.

•
Add Task: Type in box and press [ENTER].

•
Toggle Status: Left-Click on any task.

•
Manage/Exit: Right-Click on any task.

•
Toggle Overlap (Stay on Top): Ctrl + T

•
Quick ToggleRight-click any task → ➲ PIN/UNPIN

