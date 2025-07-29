# claude-code-playwright-mcp
When using Claude Code in a Windows environment to use browser automation, we encourage you to use Playwright MCP to leave a user profile so that you can load the profile without having to log in every time, and provide guidelines in CLAUDE.md to force you to use Playwright MCP for browser operations as much as possible.

## How to setup Claude Code?
> C:\Users\User\.claude.json

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
2. Ctrl + ` with open terminal
3. claude
4. say claude 
   "After entering Google, search for YouTube in the search bar and perform a test by randomly clicking on a video you like and playing it."

