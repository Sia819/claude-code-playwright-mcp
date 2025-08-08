# claude-code-playwright-mcp
When using Claude Code in a Windows environment to use browser automation, we encourage you to use Playwright MCP to leave a user profile so that you can load the profile without having to log in every time, and provide guidelines in CLAUDE.md to force you to use Playwright MCP for browser operations as much as possible.

## Project-Level MCP Configuration
This project includes a `.mcp.json` file for project-specific MCP server configuration. This approach is preferred over global configuration as it:
- Keeps MCP settings with the project
- Makes the setup reproducible for other users
- Avoids conflicts with other projects

The `.mcp.json` file in this project configures Playwright MCP with persistent browser profiles:

```json
{
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
  }
}
```

## How to use

1. Open Visual Studio Code
2. Ctrl + ` with open terminal
3. claude
4. say claude 
   "After entering Google, search for YouTube in the search bar and perform a test by randomly clicking on a video you like and playing it."

