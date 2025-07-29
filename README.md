# claude-code-playwright-mcp

## How to setup Claude Code?

C:\Users\User\.claude.json

Claude Code Windows defaults to git bash in Terminal, so you need to set it to cmd to execute commands properly.

```json
{
  ...
  "mcpServers": {
    "playwright": {
      "command": "cmd",
      "args": [
        "/c",
        "npx",
        "-y",
        "@playwright/mcp@latest",
        "--user-data-dir=./playwright-profile"
      ]
    }
  },
...
}
```

1. Open Visual Studio Code
2. claude
3. After entering Google, search for YouTube in the search bar and perform a test by randomly clicking on a video you like and playing it.
