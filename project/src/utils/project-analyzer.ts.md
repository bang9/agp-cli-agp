# project-analyzer.ts

## Purpose
- Analyzes project structure and generates initial AGP knowledge files
- Language-agnostic system supporting 50+ programming languages

## Dependencies
- **Input**: ProjectInfo from types, fs-extra, Logger utility
- **Output**: Generated architecture and pattern documentation
- **External**: fs-extra, path

## Context
- Used during agp init to create initial knowledge base
- Scans source files and categorizes by type and language
- Generates feature-domains.md and project-overview.md

## Gotchas
- Supports extensive file extensions beyond JavaScript/TypeScript
- Excludes common build/cache directories across languages
- Limits knowledge file generation to 10 files initially
- Uses generic file types (source, test, config, docs, build)

## Related
- **Patterns**: .agp/patterns/code-organization-patterns.md
- **Architecture**: .agp/architecture/feature-domains.md
- **Similar**: .agp/project/src/utils/project-detector.ts.md