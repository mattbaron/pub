# Tasks
In `tasks.json`, the first task, with `kind == build` and `isDefault == true`, is the default build task, which, with default VSCode key bindings, is run with
`Shift+Cmd+b`.

```
    {
      "label": "build-project",
      "type": "shell",
      "group": {
        "kind": "build",
        "isDefault": true
      },
      "options": {
        "cwd": "${workspaceFolder}"
      },
      "command": "bin/test.rb"
    },
```
