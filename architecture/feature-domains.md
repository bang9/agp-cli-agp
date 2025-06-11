# Feature Domains

This document maps the feature domains in this unknown project.


## Commands
- **Files**: src/commands/connect.ts, src/commands/init.ts, src/commands/push.ts, src/commands/start.ts
- **Knowledge**: .agp/project/src/commands/
- **Removed**: src/commands/link.ts (removed in development phase)

## Types
- **Files**: src/types/index.ts
- **Knowledge**: .agp/project/src/types/

## Utils
- **Files**: src/utils/agp-connect.ts, src/utils/agp-init.ts, src/utils/agp-push.ts, src/utils/agp-start.ts, src/utils/logger.ts, src/utils/project-analyzer.ts, src/utils/project-detector.ts, src/utils/template-manager.ts
- **Knowledge**: .agp/project/src/utils/
- **Removed**: src/utils/agp-link.ts (removed with link command)


## Adding New Features
When adding new features, follow the existing domain structure and create corresponding knowledge files in .agp/project/.
