# cli.ts

## Purpose
- Main CLI entry point for the AGP system
- Sets up Commander.js program with all available commands
- Handles command line argument parsing and routing

## Dependencies  
- **Input**: Command modules from ./commands/ directory
- **Output**: Executable CLI program via bin configuration
- **External**: Commander.js@14.0.0

## Context
- Entry point defined in package.json bin field as "agp"
- Registers all sub-commands (init, start, push, connect)
- Provides help and version information
- Used by end users after global npm installation

## Gotchas
- Simple program.parse() for clean help/version output
- No custom error handling to avoid "Error:" messages in help
- Removed link command (no longer supported)
- Clean exit without additional error logging

## Related
- **Architecture**: .agp/architecture/cli-structure.md
- **Similar**: Command files in src/commands/ directory
