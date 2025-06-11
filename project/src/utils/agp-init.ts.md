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
- Complex submodule initialization with retry logic (retains user interaction)
- Process.chdir() changes working directory - must handle cleanup
- Uses withSpinner for grouped operations but keeps submodule setup separate for user prompts
- Operations grouped into logical spinners: "Setting up AGP structure" and "Finalizing setup"

## Related
- **Architecture**: .agp/architecture/feature-domains.md
- **Similar**: .agp/project/src/utils/agp-start.ts.md, .agp/project/src/utils/agp-push.ts.md
