# Project Requirements

This file contains project-specific user preferences, coding standards, and behavioral rules that AI assistants must follow when working on this project.

## Git and Commit Standards

### Commit Messages
- **NEVER include Co-Authored-By lines** in commit messages
- Use conventional commit format: `type: description`
- Write commit messages in English only
- Keep first line under 72 characters
- Use present tense ("add feature" not "added feature")

### Git Workflow
- Always stage files explicitly before committing
- Push changes immediately after committing when requested
- Use meaningful commit messages that explain the "why" not just the "what"

## Code Standards

### Language Requirements
- **All source code must be in English** - no Korean comments or strings in code
- **All documentation must be in English** - no Korean in .md files or comments
- Use clear, descriptive variable and function names

### File Handling
- Prefer editing existing files over creating new ones
- Never create documentation files unless explicitly requested
- Use absolute paths for file operations

## Communication

### Response Style
- Keep responses concise and direct
- Answer user questions without unnecessary explanation
- Focus on solving the specific problem asked

## Tool Usage

### Development Tools
- Use TypeScript for all CLI development
- Use Commander.js for CLI framework
- Use proper error handling and logging
- **Use pnpm for package management** - NOT npm or yarn

### Code Formatting
- **Always run prettier before committing** - `pnpm run format`
- All TypeScript files must be formatted with Prettier
- Use project's prettier configuration (default settings)

### Logging Standards
- **ALWAYS use `logger` instead of `console.log`**
- Import logger from `../utils/logger` or `./utils/logger` in all files
- Use appropriate logger methods:
  - `logger.info()` for informational messages
  - `logger.success()` for success messages
  - `logger.error()` for error messages
  - `logger.warning()` for warnings
  - `logger.step()` for step-by-step instructions
  - `logger.debug()` for verbose/debug information

### Git Workflow Specifics
- **When user says "commit and push"**: Execute BOTH operations:
  1. Project root: `git add . && git commit && git push`
  2. AGP push: `pnpm dev push` (handles .agp directory separately)
- Always check working directory before git operations
- AGP push and main project push are separate and both required

## Project-Specific Rules

### AGP System
- Follow AGP workflows from instructions.md
- Always update knowledge files after code changes
- Maintain session tracking for collaboration
- Keep knowledge files in English with structured format

---

**Last Updated**: 2025-06-12  
**Version**: 1.3