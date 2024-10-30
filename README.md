# RSSAggregator

## Task
Build an RSS feed reader

## Spec
- Store user settings in JSON config file (~/.gatorconfig.json)
- Save DB connection URL
- Save current username
- Read/write config operations
- CLI commands for user management

## Plan
1. Config system ✓
2. CLI command system ✓
3. Database setup
4. RSS handler
5. API layer

## Code
- `main.go`: Entry point with CLI command handling
- `commands.go`: Command registration and execution system
- `handler_user.go`: User-related command handlers
- `internal/config/config.go`: Handles reading/writing config file
  - Uses JSON for storage
  - Stores in ~/.gatorconfig.json
  - Currently manages DB URL and username