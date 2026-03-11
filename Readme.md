🖥️ Assaulter-X Terminal Task Widget

A minimalist terminal-style desktop task widget built with Python and Tkinter.
It behaves like a lightweight floating terminal panel that lets you manage daily tasks while maintaining a cyberpunk / hacker aesthetic.

Designed as a personal productivity overlay, it runs quietly on the desktop with no window borders and can stay pinned above other applications.

The widget uses a Matrix-style green terminal theme, supports daily task resets, and stores tasks locally.

Project originally implemented using Python + Tkinter GUI framework. 

CODE FOR THIS TODO LIST

✨ Features
Terminal Aesthetic

Matrix-green text on deep black background

Blinking command cursor

Terminal-style status labels

Ghost Window Mode

No window borders or title bar

Floating desktop widget

Semi-transparent interface

Task Management

Add tasks quickly via input line

Toggle completion with a click

Edit or delete tasks using right-click menu

Smart Daily Reset

Tasks automatically reset every day so the list can function as a daily mission tracker.

Always-On-Top Mode

Pin the widget above all windows or allow it to float normally.

Persistent Storage

Tasks are stored locally in a JSON file.

Example storage locations:

Windows

LOCALAPPDATA/AssaulterX/terminal_tasks.json

Linux

~/.local/share/AssaulterX/terminal_tasks.json
🧠 How It Works

The application creates a borderless Tkinter window that behaves like a floating terminal widget.

Core components:

Tkinter GUI framework

JSON storage for tasks

datetime logic for daily reset

keyboard shortcuts for system control

The main class responsible for the application is:

TerminalWidget

Responsibilities include:

window management

rendering tasks

handling keyboard and mouse events

saving and loading task data

automatic daily resets

⌨️ Controls
Action	Command
Add Task	Type text and press ENTER
Toggle Task Status	Left Click task
Edit / Delete Task	Right Click task
Move Widget	Hold SHIFT + Drag
Toggle Always-On-Top	CTRL + T
Exit Widget	Right click → Exit System

Control summary adapted from the implementation instructions. 

CODE FOR THIS TODO LIST

⚙️ Installation
Windows
1️⃣ Install Python

Download Python and ensure it is added to PATH.

2️⃣ Install PyInstaller
pip install pyinstaller
3️⃣ Build the executable
pyinstaller --onefile --noconsole assaulter_x.py

The executable will appear inside:

dist/
4️⃣ Enable Auto Startup

Press:

Win + R

Then run:

shell:startup

Create a shortcut to the .exe file in this folder.

Linux
1️⃣ Install dependency
sudo apt install python3-tk
2️⃣ Make script executable
chmod +x assaulter_x.py
3️⃣ Add to startup

Create:

~/.config/autostart/assaulter.desktop

and configure it to launch the script.

📁 Project Structure
assaulter-x-terminal-widget
│
├── assaulter_x.py
├── README.md
└── terminal_tasks.json (auto-generated)
🎯 Purpose of This Project

This project was built as a personal desktop productivity tool for people who prefer:

terminal aesthetics

lightweight utilities

distraction-free task tracking

It demonstrates how a simple Python script can behave like a native desktop widget.

🚀 Future Improvements

Possible upgrades:

notifications for tasks

categories or tags

keyboard-only task management

cloud synchronization

plugin system

system monitoring integration

🧑‍💻 Author

Assaulter X

Computer Engineering Student
Interested in cybersecurity, automation, and terminal-based tools.