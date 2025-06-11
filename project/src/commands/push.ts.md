# push.ts

## Purpose
- CLI command implementation for pushing AGP knowledge and session progress to remote repository
- Replaces deprecated sync command with Git-standard terminology

## Dependencies
- **Input**: Commander.js Command class, agp-push utility, Logger utility
- **Output**: None (CLI command)
- **External**: commander (CLI framework)

## Context
- Part of AGP CLI commands system
- Invoked when user runs `agp push` command
- Enables team collaboration by syncing knowledge changes

## Gotchas
- Uses Logger instead of console.log for consistent output
- Optional commit message parameter with -m flag
- Exits with error code 1 on failure

## Related
- **Patterns**: .agp/patterns/code-organization-patterns.md
- **Architecture**: .agp/architecture/feature-domains.md
- **Similar**: .agp/project/src/commands/init.ts.md