# template-manager.ts

## Purpose
- Manages downloading and extracting AGP template files from remote repositories
- Handles ZIP archive extraction and file copying operations

## Dependencies
- **Input**: Template URL, target directory path
- **Output**: Extracted template files in .agp directory
- **External**: https, fs-extra, path, yauzl

## Context
- Used during agp init to bootstrap AGP directory structure
- Downloads template from GitHub or other Git hosting services
- Extracts template files while preserving directory structure

## Gotchas
- Uses ZIP download instead of git clone for simplicity
- Handles GitHub archive URL format automatically
- Skips root directory when extracting to avoid nesting
- Requires network access to template repository

## Related
- **Patterns**: .agp/patterns/code-organization-patterns.md
- **Architecture**: .agp/architecture/feature-domains.md
- **Similar**: .agp/project/src/utils/agp-init.ts.md