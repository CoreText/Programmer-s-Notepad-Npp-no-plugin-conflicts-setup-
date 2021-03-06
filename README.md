# The programmer's Notepad++ (no plugin conflicts setup)

The full-feature Notepad++ setup with some scripts collections from other repositories and installed plugins with stable releases (x64) that do not have any conflicts. Hit the `Ctrl+Shift+Alt+M` to read this file in the editor.


## Installation

Download the latest release from this repo. Before starting the Notepad++ make sure you run Notepad++Portable.exe, because if you run notepad++.exe directly all small configurations will be lost.

- You can install Notepad++ via PortableApps and replace `PortableApps/Notepad++Portable/` with this Notepad++, but it's not necessary.

- Find `Users\username` (with case sensitive) and replace it with your  `Users\<your-username>` in whole directory of `Notepad++Portable`. Replace `Users/username` with `Users/<your-username>` and replace `Users\\username` with `Users\\<your-username>`.

- Create shortcut for Notepad++Portable.exe and pin it to the Taskbar and Desktop, or you can access it from the PortableApps manager.


## Theme

My preferred theme is `Texter-Light` (because of Compare plugin, React JSX and PHP better highlight) and `Twilight-Neon` in the Windows High Contrast and editor's Dark Mode. If you want to have dark mode in Notepad++ everywhere go to `Language->User Defined Language->Define your language...` and change file extensions for each user defined Dark/Light language in the Extension field.


### Some hotkeys
- `Ctrl+Shift+Alt+S` - Change to your preferred command, e.x.: to save and compile current file
- `Ctrl+Shift+Alt+D` - Change to your preferred command
- `Shift+Alt+D` - you can clone the file to the next view, or. Useful for the large files navigation
- `Ctrl+Alt+D` - you can move the file to the next view
- `Alt+D`, `Alt+J` - Multicursor feature, select next occurrence, like in the SublimeText editor
- `Alt+W` - Select by word
- `Alt+K` - Skip to next selection
- `Alt+U` - Undo selection
- `Ctrl+Shift+L` - Select all occurrences
- `Ctrl+Shift+Alt+P` - Toggle spell checker
- `Alt+P` - go to next error
- `Shift+Alt+P` - go to previous error
- `Shift+Enter` - will break the line
- `Shift+Space` - will select between quotes
- `Shift+Alt+Space` - edit in the Distraction Free Mode
- `Alt+Z` - cursor to previous location
- `Shift+Alt+Z` - cursor to next location
- `Alt+A` - Emmet select inwards
- `Shift+Alt+A` - Emmet select outwards
- `Ctrl+Alt+A` - Select paragraph
- `Ctrl+Shift+A` - Select by Fold
- `Ctrl+Shift+Alt+A` - Format using JSBeautifier
- `Shift+Alt+R` - Reverse the caret position in selection
- `Alt+F` - Incremental search
- `Shift+Alt+F` - Multiline replace
- `Ctrl+Alt+F` - Filter results in new tab
- `Alt+N` - Create file in the same directory
- `Alt+S` - Rename current file

- Ctrl+Shift+Alt+` - to open Workspace panel
- Ctrl+Shift+Alt+1 - to open Workspace Panel 1
- Ctrl+Shift+Alt+2 - to open Workspace Panel 2
- Ctrl+Shift+Alt+3 - to open Workspace Panel 3


#### Projecting

In the context menu you'll find Workspace item that will have useful items to work with the project. If you installed Git - make sure the Workspace path is loaded (Workspace panel is active) and you can access Git features from the context menu `Git->Git Edit Global .gitignore` and then paste the following:

```
.DS_Store
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

The most useful plugin I found is NppGTags. Open any file in the workspace root directory and click `Workspace->Create database`. Make sure if the workspace path is loaded. To check the path - hit `Alt+\`.

If you know how to use ctags.exe - download and compile it from the sources and after running ctags you'll be able to use `NppTags` and `TagLEET`. If you want to generate tags database from the editor's interface - make sure you opened file in the root directory where you want tags database to be generated and Tags Tree panel is closed, otherwise it will too slow to generate tags file. The built `ctags.exe` version you can find in `Notepad++Portable\App\Notepad++64\ctags-p5.9.20210718.0` directory and you can setup `NppTags->Options...` path to `ctags.exe` location.


#### Git

If you want use Git features - it's better to download and install TortoiseGit. One more useful program is DiffUse - download and install it, hit `Ctrl+Shift+P` and write `path env` and chose `Open PATH Environment Variables`, add the absolute path to diffuse.exe to the user's `Path` environment variable.


#### Some features

- Better PHP, Python, SQL, CSS support (autocomplete, commands and more).
  All PHP functions from php.net + all WordPress functions from official docs.
  Run `Notepad++Portable\App\Notepad++64\b2npp.php` in the browser in order to generate `html.xml` to autocomplete CSS classes like Bootstrap 4, Foundation and etc. The original script is [here](https://github.com/brhndursun/Bootstrap-Autocomplete-for-Notepad). You can find generated classes for Bootstrap, Foundation, Tailwind CSS in `Notepad++Portable\App\Notepad++64\autoCompletion` directory. Just need to replace `html.xml.bak` to `html.xml` to use it and vice versa.

- Better `Function List` support for the Golang, Lua, TypeScript and JavaScript ES6 functions and methods.

- Extended context menu.

- Useful scripts collection for `Python Script` and `jN` plugins.

- Themes collection and user defined languages.

- In the Explorer's Favorites you can find useful links to some popular resources/services.

- Language-Help with helpful .chm docs and useful search engines.

- Open `TODO.txt` using `Ctrl+Shift+Alt+Space` shortcut, or access it from the context menu.

- While editing the document you can hit `Ctrl+Shift+P` (hotkey like in Sublime Text, vscode), type 10, and you'll see `Add 10 Lines`, press `Enter` key and after some time if you need more 10 new lines - hit `Ctrl+Shift+Alt+Enter` and previous command will be executed (`NppMenuSearch`).

- `Ctrl+Shift+Alt+Backspace` - Previous command of `NppExec` plugin.

- `Ctrl+Shift+Alt+\` - Previous command of `Python Script` plugin.


##### Windows 7 installation

If you have a compatibility issue with the `Python Script` plugin - replace downloaded `PythonScript.dll` from the official Notepad++ plugin repository in `Notepad++Portable\App\Notepad++64\plugins\PythonScript` directory.
