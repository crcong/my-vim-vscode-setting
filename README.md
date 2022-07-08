# my vim vscode setting

my VS Code Settings about vim.

## universal setting

### settings.json

```json
"vim.useCtrlKeys": true,
"vim.handleKeys": {},
"vim.insertModeKeyBindings": [
    // insert模式退出normal模式
    {
        "before": [
            "j",
            "j"
        ],
        "after": [
            "<Esc>"
        ]
    }
],
"vim.normalModeKeyBindings": [
    {
        "before": [
            "H"
        ],
        "after": [
            "^"
        ]
    },
    {
        "before": [
            "L"
        ],
        "after": [
            "g",
            "_"
        ]
    },
    {
        "before": [
            "J"
        ],
        "after": [
            "5",
            "j"
        ]
    },
    {
        "before": [
            "K"
        ],
        "after": [
            "5",
            "k"
        ]
    },
],
"vim.visualModeKeyBindings": [
    {
        "before": [
            "J"
        ],
        "after": [
            "5",
            "j"
        ]
    },
    {
        "before": [
            "K"
        ],
        "after": [
            "5",
            "k"
        ]
    },
],
"vim.operatorPendingModeKeyBindings": [
    {
        "before": [
            "H"
        ],
        "after": [
            "^"
        ]
    },
    {
        "before": [
            "L"
        ],
        "after": [
            "g",
            "_"
        ]
    }
],
// 折叠鼠标经过不会自动展开
"vim.foldfix": true,
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
    "<C-c>": false,
    "<C-d>": false,
    "<C-b>": false,
    "<C-f>": false
},
```

