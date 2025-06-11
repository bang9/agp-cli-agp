# logger.ts

## Purpose
- Clean, emoji-free logging utility for CLI output
- Provides consistent formatting with minimal ASCII symbols
- Supports clear progress indicators without visual clutter

## Dependencies
- **Input**: LoggerOptions for configuration
- **Output**: Formatted console output with ASCII symbols
- **External**: chalk for colors

## Context
- Core utility for all CLI output across AGP commands
- Recently refactored to remove excessive emojis and verbose formatting
- Provides professional, clean terminal output

## Gotchas
- Uses simple ASCII symbols: ✓ for success, ✗ for error, → for steps
- Progress uses spinner character ⠋ for minimal visual feedback
- All emoji-heavy formatting has been removed for cleaner UX
- clearProgress() essential for inline progress updates

## Related
- **Patterns**: .agp/patterns/code-organization-patterns.md
- **Architecture**: .agp/architecture/feature-domains.md
- **Similar**: All utils files depend on this logger