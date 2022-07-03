# my vim vscode setting

my VS Code Settings about vim.

## universal setting

### settings.json

```json
"vim.useCtrlKeys": true,
"vim.handleKeys": {
    "<C-w>": false,
    "<C-f>": false
},
"vim.insertModeKeyBindings": [
    // insert模式退出normal模式
    {
        "before": ["j", "j"],
        "after": ["<Esc>"]
    }
],
"vim.normalModeKeyBindings": [
    // 光标移到到行首或行尾
    {
        "before": ["H"],
        "after": ["^"]
    },
    {
        "before": ["L"],
        "after": ["g", "_"]
    }
],
"vim.operatorPendingModeKeyBindings": [
    // 操作到行首或行尾
    {
        "before": ["H"],
        "after": ["^"]
    },
    {
        "before": ["L"],
        "after": ["g", "_"]
    }
],
```

## macos

### keybindings.json

```json
[
    // 防止insert模式下 ctrl + c 会进入到 normal 模式
    { "key": "cmd+c", "command": "execCopy" }
]
```

## windows

### settings.json

```json
// 防止insert模式下 ctrl + c 会进入到 normal 模式
"vim.handleKeys": {
    "<C-c>": false
},
```

