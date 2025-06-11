# Patterns Directory Overview

This directory contains reusable patterns, implementation guidelines, and common knowledge that applies across multiple parts of the project.

## Directory Purpose
- **Implementation Patterns**: Standardized ways to implement common functionality
- **Reusable Guidelines**: Best practices that apply to multiple features
- **Cross-cutting Concerns**: Knowledge that spans multiple domains or components

## Auto-Generated Files

These files are automatically created and updated by `agp init` based on project analysis:

### Core Patterns
- `code-organization-patterns.md` - Generated when source files are detected (shows languages, directories, file naming)
- `testing-patterns.md` - Generated when test files are detected

### Additional Files
Files created as needed based on project analysis and manual additions:
- Additional pattern files may be created based on detected frameworks and project complexity

## Usage Guidelines

### When to Read
- **Before implementing new features**: Check for existing patterns that apply to your work
- **When solving common problems**: Look for established solutions before creating new approaches
- **During code reviews**: Reference patterns to ensure consistency

### When to Update
- **New reusable patterns**: Create new pattern files when you solve problems that could apply elsewhere
- **Pattern improvements**: Update existing patterns when better approaches are discovered
- **Cross-feature solutions**: Document solutions that work across multiple features

### File Naming Convention
- Use kebab-case for file names
- End with `-patterns.md` for implementation patterns
- End with `-guidelines.md` for process or quality guidelines
- Use descriptive names that clearly indicate the CLI pattern scope

## Pattern Categories

### CLI Implementation Patterns
Files that show how to implement specific CLI functionality
- Command structure and organization using Commander.js
- Utility function patterns for common operations
- Terminal output and logging patterns

### Process Guidelines
Files that describe CLI development processes and quality standards
- CLI testing approaches with proper mocking
- Code review standards for CLI applications
- Performance optimization for CLI tools

### CLI Best Practices
Files that capture CLI-specific best practices and lessons learned
- Common CLI pitfalls and how to avoid them
- Terminal UX optimization techniques
- Cross-platform compatibility considerations

## Maintenance Notes
- Keep this overview updated when adding new files to the patterns directory
- Link related files in the architecture directory when patterns relate to specific architectural domains
- Regularly review and update patterns based on project evolution
- Remove or archive patterns that are no longer relevant