# logger.ts

## Purpose
- Centralized logging utility with progress indicators and consistent formatting
- Provides clean terminal output with color coding and inline progress updates

## Dependencies
- **Input**: LoggerOptions for configuration
- **Output**: Formatted console output
- **External**: chalk for colors

## Context
- Used throughout AGP CLI for consistent user feedback
- Replaces direct console.log usage across the application
- Supports progress bars, success/error states, and debug output

## Gotchas
- Progress methods use ANSI escape codes for inline updates
- clearProgress() method is public for external control
- Silent mode suppresses all output except errors
- Handles emoji display length calculations

## Related
- **Patterns**: .agp/patterns/code-organization-patterns.md
- **Architecture**: .agp/architecture/feature-domains.md
- **Similar**: None (utility pattern)