# agp-start.ts

## Purpose
- Core utility for starting or resuming AGP user sessions
- Manages user identification, session creation, and configuration updates

## Dependencies
- **Input**: fs-extra, readline for user input
- **Output**: Updated .agp/.config.json and session files
- **External**: fs-extra, readline

## Context
- Used by start command to manage user sessions
- Creates user directories and session files
- Updates local configuration with current user info

## Gotchas
- Uses readline for cross-platform user input
- Creates session directory structure if missing
- Provides guidance for new users about next steps
- Mentions agp push for sharing progress

## Related
- **Patterns**: .agp/patterns/code-organization-patterns.md
- **Architecture**: .agp/architecture/feature-domains.md
- **Similar**: .agp/project/src/utils/agp-init.ts.md