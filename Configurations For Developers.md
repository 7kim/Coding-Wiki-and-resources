# Table of Contents
- [[#IDE Extensions|IDE Extensions]]
- [[#IDE Workspace settings.json|IDE Workspace settings.json]]
- [[#IDE User Settings.json|IDE User Settings.json]]
- [[#IDE KeyBindings.json|IDE KeyBindings.json]]

# IDE configurations
## IDE Extensions 
``` Python
Tailscale
Project Manager
Prettier
Paste Json as Code
Live Server
Jupyter Slide Show
Jupyter Notebooks
Python
vscode-pdf
Remote - SSH
Docx/ODT Viewer
Data Wrangler
C/C++
OpenCode
npm intellisense
```

## IDE Workspace settings.json
``` json
{
"workbench.colorCustomizations": {
"activityBar.activeBackground": "#2f7c47",
"activityBar.background": "#2f7c47",
"activityBar.foreground": "#e7e7e7",
"activityBar.inactiveForeground": "#e7e7e799",
"activityBarBadge.background": "#422c74",
"activityBarBadge.foreground": "#e7e7e7",
"activityBarTop.activeBackground": "#2f7c47",
"activityBarTop.background": "#2f7c47",
"activityBarTop.foreground": "#e7e7e7",
"activityBarTop.inactiveForeground": "#e7e7e799",
"commandCenter.border": "#e7e7e799",
"commandCenter.foreground": "#e7e7e7",
"sash.hoverBorder": "#2f7c47",
"statusBar.background": "#215732",
"statusBar.debuggingBackground": "#215732",
"statusBar.debuggingForeground": "#e7e7e7",
"statusBar.foreground": "#e7e7e7",
"statusBarItem.hoverBackground": "#2f7c47",
"statusBarItem.remoteBackground": "#1b122e",
"statusBarItem.remoteForeground": "#e7e7e7",
"titleBar.activeBackground": "#215732",
"titleBar.activeForeground": "#e7e7e7",
"titleBar.inactiveBackground": "#21573299",
"titleBar.inactiveForeground": "#e7e7e799"
},
"peacock.color": "#215732",
"editor.mouseWheelZoom": true,
"editor.minimap.enabled": true,
"editor.wordWrap": "on"
}
```

## IDE User Settings.json
``` json
{"workbench.colorTheme": "Dark+",
"explorer.confirmDelete": false,
"explorer.confirmDragAndDrop": false,
"workbench.editorAssociations": {
"*.copilotmd": "vscode.markdown.preview.editor",
"*.md": "vscode.markdown.preview.editor"},
"extensions.ignoreRecommendations": true,
"claudeCode.preferredLocation": "panel",
"chat.viewSessions.orientation": "stacked",
"liveServer.settings.donotShowInfoMsg": true,
"terminal.integrated.profiles.linux": {
"bash": {
"path": "/usr/bin/bash"},
"zsh": {
"path": "zsh"},
"fish": {
"path": "fish"},
"tmux": {
"path": "/usr/bin/tmux",
"icon": "terminal-tmux"},
"pwsh": {
"path": "pwsh",
"icon": "terminal-powershell"}
},
"terminal.integrated.defaultProfile.linux": "bash",
"terminal.integrated.initialHint": false,
"terminal.integrated.copyOnSelection": true}
```

## IDE KeyBindings.json
``` json
// Place your key bindings in this file to override the defaults
[{"key": "ctrl+c","command": "workbench.action.terminal.copySelection","when": "terminalFocus && terminalTextSelected"},
// 2. Remap Ctrl+V to Paste in the terminal
{"key": "ctrl+v","command": "workbench.action.terminal.paste","when": "terminalFocus"},
// 3. Make Shift+Ctrl+C stop/interrupt the running process in the terminal (SIGINT)
{"key": "ctrl+shift+c","command": "workbench.action.terminal.sendSequence","args": { "text": "\u0003" },"when": "terminalFocus"},
// 4. Make Ctrl+A select all text in the terminal
{"key": "ctrl+a","command": "workbench.action.terminal.selectAll","when": "terminalFocus"}]
```

# Obsidian Plugins

- [ ] Editor Toolbar 
- [ ] Excalidraw
- [ ] Drawio
- [ ] Tasks
- [ ] Dataview
- [ ] Templater
- [ ] Calender
- [ ] Git
- [ ] Kanban
- [ ] Iconize
- [ ] Importer
- [ ] Smart Connections
- [ ] Linter
- [ ] TaskNotes
- [ ] MindMap
- [ ] DayPlanner
- [ ] PDF++
- [ ] Custom Frames
- [ ] Code Styler
- [ ] table of contents


# Must Have Apps for developers
## backend apps / CLI's

``` json
Tailscale// Internet traffic and IPv6 safety
mise// python environment variables handlers
uv astral
bun// javascript compilers
pnpm
git// git tracking
gh
cargo//rust compilers
rustup
gcc // c compiler
g++ // c++ compiler
cmake //
clang // frontend for kernel compiler
llvm // backend for kernel compiler
```

## Front end apps

### IDE
```
Cursor
Antigravity
Vscode
warp // terminal
```
### AI Cli's
```
claude code
gemini cli
agy
opencode
hermes
openclaw
pi
crush (latest version of opencode)
ollama
llama.cpp

```
### Gnu linux apps
```
GNU octave
Labplot
drawio

```

### productivity apps
```
notion
obsidian
syncthing
github desktop
openrazer
polychromatic
htop
mission control
vlc
proton pass / bitwarden
cantor // for math
```

