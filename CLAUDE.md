# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is a personal automation scripts repository for creating Python scripts that automate repetitive tasks. The primary workflow is conversational: users describe tasks they want to automate, and Claude creates working programs for them.

## Development Workflow

### Creating New Automation Scripts

1. **Gather Requirements**: Ask clarifying questions before writing any code:
   - What specific files/data are being processed?
   - Single file or batch processing?
   - Should the script ask for confirmation or run automatically?
   - Input/output format examples

2. **Implementation Standards**:
   - Use Python 3 for all automation scripts
   - Include shebang line: `#!/usr/bin/env python3`
   - Add comprehensive error handling with clear user-facing messages
   - Make scripts executable with `chmod +x script_name.py`
   - Include inline comments explaining the logic

3. **Testing**: Test the script thoroughly before presenting to the user

4. **Documentation**: Provide step-by-step instructions for running the script

5. **Git Integration**: All changes are automatically committed to git

### Common Script Categories

- **File Management**: Renaming, organizing, deduplication
- **Data Processing**: CSV manipulation, text extraction, data transformation
- **Web Tasks**: Scraping, downloading, monitoring
- **Regular Cleanup**: Scheduled deletions, backups, file finding

## Platform Notes

This repository is currently on Windows (win32), but scripts should be cross-platform compatible where possible. When creating scripts:
- Use `pathlib` for file paths instead of hardcoded separators
- Check for platform-specific requirements (e.g., `chmod` is Unix/Mac only)
- Test file path handling on Windows

## User Experience Principles

- Prioritize user-friendly error messages over technical jargon
- Scripts should clearly indicate what they're doing and when they're done
- Default to asking for confirmation on destructive operations
- Provide examples of usage in the documentation
