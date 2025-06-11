# agp-push.ts

## Purpose
- Core utility for pushing AGP knowledge changes to remote Git repository
- Handles commit message generation, progress reporting, and submodule pointer updates

## Dependencies
- **Input**: AgpPushOptions interface from types
- **Output**: None (Git operations)
- **External**: child_process.execSync, fs-extra, Logger utility

## Context
- Used by push command to perform actual Git operations
- Operates on .agp directory as Git submodule
- Updates parent repository submodule reference after push

## Gotchas
- Changes working directory during execution (always restores)
- Generates smart commit messages based on changed file types
- Uses silent Git operations to avoid cluttering output
- Requires .agp to be initialized as Git repository

## Related
- **Patterns**: .agp/patterns/code-organization-patterns.md
- **Architecture**: .agp/architecture/feature-domains.md
- **Similar**: .agp/project/src/utils/agp-init.ts.md