# The programmer's Notepad++ (no plugin conflicts setup)

The advanced Notepad++ setup that does not have any conflicts between the installed plugins. The setup was done mostly for the back-end web developers. Hit the `Ctrl+Shift+Alt+M` to read this file in the editor.


## Usage

Before starting the Notepad++ make sure you run Notepad++Portable.exe , or if you will run notepad++.exe directly all small configurations will be lost. Download PortableApps, install Notepad++ and replace `PortableApps/Notepad++Portable/` with extracted directory, or you can create shortcut for Notepad++Portable.exe and pin it to the TaskBar and Desktop.


### Theme

My preferred theme is `Texter-Light` and `Texter-Twilight` in the Windows High Contrast and editor's Dark Mode. If you want dark mode in Notepad++ go to `Language->User Defined Language->Define your language...` and change file extensions for each Dark/Light theme. By default the color scheme will load "Light" syntax.


### The workflow

After you open the editor you'll see `TODO.txt` that could be opened using `Ctrl+Shift+Alt+Space` shortcut, or accessed from the context menu.

When you edit the document you can hit `Ctrl+Shift+P`, type 10, and you'll see `Add 10 Lines`, press `Enter` key and after some time if need more 10 new lines - hit `Ctrl+Shift+Alt+Enter` and previous command will be executed. 

- `Ctrl+Shift+Alt+Backspace` is used for NppExec plugin to repeat executed command, e.x. if you want to compile some script.
- `Shift+Alt+D` - you can clone the file to the next view, or
- `Ctrl+Alt+D` - you can move the file to the next view. It's useful when you need work with large files.
- `Alt+D`, `Alt+J` - Multicursor, select next occurrence, like in the SublimeText editor
- `Alt+W` - Select by word
- `Alt+K` - Skip to next selection
- `Alt+U` - Undo selection
- `Ctrl+Shift+L` - Select all occurrences 
- `Ctrl+Alt+P` - Toggle spell checker
- `Alt+P` - go to next error
- `Shift+Alt+P` - go to previous error
- `Shift+Enter` - will break the line
- `Shift+Space` - will select between quotes
- `Shift+Alt+Space` - edit in the Distraction Free Mode
- `Alt+Z` - cursor to previous location
- `Shift+Alt+Z` - cursor to next location
- `Ctrl+Alt+A` - Select paragraph
- `Ctrl+Shift+A` - Select by Fold


### Projecting

In the context menu you'll find Workspace item that will have useful items to work with the project. If you installed Git - make sure the Workspace path is loaded and you can chose from the context menu `Git->Git Edit Global .gitignore` and paste the following:

```
.DS_Store
.vscode
.idea
.tags
tags.idx
Thumbs.db
*.orig
*.swp
GPATH
GTAGS
GRTAGS
NppGTags.cfg
tags
tags.sqlite

```

The most useful plugin I found is NppGTags. Open any file in the workspace root directory and `Create database`. Make sure if the workspace path is loaded. If you know how to use ctags.exe - download and compile it from the sources and after that you'll be able to use NppTags and TagLEET, but if you will want to generate tags database it will be slow.


#### Git

If you want use Git features - it's better to download and install TortoiseGit. One more useful program is DiffUse - download and install it and hit `Ctrl+Shift+Alt+P` and add the absolute path to diffuse.exe to the user's `Path` environment variable.


#### Useful links

In the Explorer's Favorites you can find useful links to some popular services.

