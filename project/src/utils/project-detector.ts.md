# project-detector.ts

## Purpose
- Detects project type, framework, and build tools for AGP initialization
- Provides project metadata for knowledge generation

## Dependencies
- **Input**: fs-extra for file system operations
- **Output**: ProjectInfo with detected metadata
- **External**: fs-extra, path

## Context
- Used during agp init to understand project structure
- Analyzes package.json, config files, and directory structure
- Informs project-analyzer about project characteristics

## Gotchas
- Focuses on common frameworks and build tools
- May return 'unknown' for unrecognized project types
- Checks for standard configuration files and dependencies

## Related
- **Patterns**: .agp/patterns/code-organization-patterns.md
- **Architecture**: .agp/architecture/feature-domains.md
- **Similar**: .agp/project/src/utils/project-analyzer.ts.md