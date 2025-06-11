# agp-init.ts

## Purpose
- Initializes AGP system with clean, user-friendly output
- Sets up .agp directory structure, Git submodule, and project analysis
- Handles template download and repository configuration

## Dependencies
- **Input**: project-detector.ts, template-manager.ts, project-analyzer.ts, logger.ts
- **Output**: Used by init command in commands/init.ts
- **External**: fs-extra, inquirer, child_process

## Context
- Core AGP initialization logic
- Handles both new setups and existing repository merging
- Manages Git submodule configuration with user prompts

## Gotchas
- Complex submodule initialization with retry logic
- Process.chdir() changes working directory - must handle cleanup
- Handles existing repository conflicts with user choices
- Output messages simplified for clean user experience

## Related
- **Architecture**: .agp/architecture/feature-domains.md
- **Similar**: .agp/project/src/utils/agp-start.ts.md, .agp/project/src/utils/agp-push.ts.md
