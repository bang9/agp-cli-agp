# logger.ts

## Purpose
- Clean logging utility with ora-powered spinners for CLI output
- Provides consistent formatting with professional spinner animations
- Handles success/error states with proper visual feedback

## Dependencies
- **Input**: LoggerOptions for configuration
- **Output**: Formatted console output with ora spinners
- **External**: chalk for colors, ora for spinner animations

## Context
- Core utility for all CLI output across AGP commands
- Uses ora library for reliable, non-blocking spinner animations
- Provides withSpinner method for long-running operations

## Gotchas
- ora handles spinner animation automatically without blocking execSync
- withSpinner wraps operations and shows succeed/fail states
- Uses simple ASCII symbols: ✓ for success, ✗ for error, → for steps
- ora spinners work properly even with synchronous child processes

## Related
- **Patterns**: .agp/patterns/code-organization-patterns.md
- **Architecture**: .agp/architecture/feature-domains.md
- **Similar**: All utils files depend on this logger