# agp-push.ts

## Purpose
- Core utility for pushing AGP knowledge changes to remote Git repository
- Uses spinner for clean progress indication during Git operations
- Handles commit message generation and submodule pointer updates

## Dependencies
- **Input**: AgpPushOptions interface from types
- **Output**: None (Git operations)
- **External**: child_process.execSync, fs-extra, Logger utility with withSpinner

## Context
- Used by push command to perform actual Git operations
- Operates on .agp directory as Git submodule
- Recently updated to use spinner for cleaner UX during push operations

## Gotchas
- Changes working directory during execution (always restores in finally block)
- Generates smart commit messages based on changed file types (sessions, project, patterns, architecture)
- Uses silent Git operations wrapped in spinner for clean output
- Requires .agp to be initialized as Git repository

## Related
- **Patterns**: .agp/patterns/code-organization-patterns.md
- **Architecture**: .agp/architecture/feature-domains.md
- **Similar**: .agp/project/src/utils/agp-init.ts.md