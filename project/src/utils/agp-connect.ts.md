# agp-connect.ts

## Purpose
- Configures AI tools (Claude, Cursor, ChatGPT) to integrate with AGP workflow system
- Automatically injects complete AGP instructions into CLAUDE.md for seamless integration

## Dependencies
- **Input**: AgpConnectOptions from types, .agp/instructions.md content
- **Output**: Updated CLAUDE.md, tool-specific config files
- **External**: fs-extra, path

## Context
- Used by connect command to setup AI tool integration
- Reads full instructions.md and embeds in CLAUDE.md
- Creates tool-specific configuration files based on platform

## Gotchas
- Claude setup reads entire instructions.md and embeds it completely
- Replaces existing MANDATORY sections in CLAUDE.md
- Different AI tools require different integration approaches
- Must validate .agp directory exists before configuration

## Related
- **Patterns**: .agp/patterns/code-organization-patterns.md
- **Architecture**: .agp/architecture/feature-domains.md
- **Similar**: .agp/project/src/utils/agp-init.ts.md
