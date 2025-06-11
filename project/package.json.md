# package.json

## Purpose
- NPM package configuration for agp-cli distribution
- Defines CLI binary mapping and build scripts
- Manages dependencies and project metadata

## Dependencies  
- **Input**: src/cli.ts and all command modules (init, start, push, connect)
- **Output**: Distributed NPM package with global CLI binary
- **External**: Commander.js@14.0.0, fs-extra@11.3.0, inquirer@12.6.3, node-fetch@3.3.2, yauzl@3.2.0

## Context
- Published to NPM registry as "agp-cli" package
- Users install globally with npm install -g agp-cli
- bin field maps "agp" command to compiled dist/cli.js
- Current version: 0.1.1 (fixed CLI help/version error messages)

## Gotchas
- Version must be incremented for each NPM publish
- prepublishOnly script ensures clean builds before publish
- bin field maps "agp" command to dist/cli.js
- Removed chalk dependency in v0.1.1 for cleaner CLI output
- Link command support removed (no agp-link.ts utility)
- Main entry point: dist/cli.js (not index.js)

## Related
- **Architecture**: .agp/architecture/project-overview.md
- **Similar**: .agp/project/src/cli.ts.md