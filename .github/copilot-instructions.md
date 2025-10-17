# Copilot Instructions for Automation Scripts Repository

## Repository Purpose
This is a **conversational automation factory** where non-technical users describe repetitive tasks and receive working Python scripts. The workflow is consultation → implementation → instruction, not traditional software development.

## Critical Workflow: Requirements-First Approach
**ALWAYS ask clarifying questions BEFORE writing code:**
- What specific files/data are being processed?
- Single file or batch processing?
- Should the script ask for confirmation or run automatically?
- Can the user provide input/output format examples?

Do not skip this step. User satisfaction depends on getting requirements right.

## Script Creation Standards

### Every Script Must Include:
1. **Shebang line**: `#!/usr/bin/env python3`
2. **Clear error handling** with user-friendly messages (not technical jargon)
3. **Inline comments** explaining the logic
4. **Usage instructions** in comments at the top
5. **Progress indicators** for long-running operations
6. **Input validation** before processing

### File Naming Convention:
Use descriptive names that explain the task: `rename_photos_by_date.py`, not `script1.py`

### Platform Compatibility:
- Primary platform: Windows (note: README mentions Mac but codebase is on Windows)
- Use `pathlib` for cross-platform file path handling
- Note that `chmod +x` is Unix/Mac only - adjust instructions for Windows users
- Test file path handling on Windows

## Common Script Categories
Reference these patterns when users request automation:

1. **File Management**: Renaming, organizing, deduplication
2. **Data Processing**: CSV manipulation, text extraction, data transformation  
3. **Web Tasks**: Scraping, downloading, monitoring
4. **Regular Cleanup**: Scheduled deletions, backups, file finding

See `README.md` lines 11-28 for specific user request examples.

## Git Workflow (MANDATORY)
After **EVERY** file change, create a git commit:
```bash
git add .
git commit -m "Descriptive message of what was done"
```
Never skip commits. Every change must be tracked per `.claude/PROGRAM_CREATION_PROCESS.md`.

## User Experience Principles
- **Non-technical audience**: Avoid jargon, explain in plain English
- **Copy-paste ready**: Provide exact commands users can run
- **Safety first**: Default to asking confirmation on destructive operations
- **Clear success/failure**: Scripts must explicitly tell users what happened

## Testing Before Delivery
Test scripts with sample data before presenting to users. Handle common errors (missing files, permissions, invalid inputs) with helpful messages explaining how to fix issues.

## References
- User-facing guide: `README.md`
- Agent-specific guidance: `CLAUDE.md`
- Detailed process: `.claude/PROGRAM_CREATION_PROCESS.md`
