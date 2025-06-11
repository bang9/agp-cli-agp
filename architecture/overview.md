# Architecture Directory Overview

This directory contains high-level project architecture and organizational knowledge.

## Directory Purpose
- **Project Architecture**: Overall system design and structure
- **Feature Organization**: How different features are organized within the codebase
- **Global Standards**: Project-wide conventions and guidelines

## Auto-Generated Files

These files are automatically created and updated by `agp init`:

### Core Architecture
- `project-overview.md` - Overall project structure, detected framework, build tools, and package manager
- `feature-domains.md` - Feature areas grouped by functionality and their file locations within the project

### Additional Files
Files created as needed based on project complexity:
- Additional architecture files may be created manually as the project grows

## Usage Guidelines

### When to Read
- **Before starting new features**: Read relevant architecture files to understand where to place new code
- **When refactoring**: Check existing architectural decisions before making changes
- **When onboarding**: Review core architecture files to understand project organization

### When to Update
- **New feature domains**: Add to feature-domains.md and create domain-specific architecture files if needed
- **Architectural changes**: Update overview files when making significant structural changes
- **New conventions**: Document new standards in appropriate files

### File Naming Convention
- Use kebab-case for file names
- End with `.md` extension
- Use descriptive names that clearly indicate the content scope

## Maintenance Notes
- Keep this overview updated when adding new files to the architecture directory
- Link related files in the patterns directory when architectural patterns are involved
- Archive or remove obsolete files to maintain clarity