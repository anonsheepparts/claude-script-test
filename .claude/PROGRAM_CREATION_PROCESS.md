# Program Creation Process for Automation Tasks

## Purpose
This repository contains automation scripts for repetitive tasks. The primary user is a non-programmer working on macOS who needs reliable, easy-to-use automation solutions.

## Process for Creating New Programs

### 1. **Understand the Task** (REQUIRED FIRST STEP)
- Ask clarifying questions about the repetitive task
- Understand the inputs (files, data, user actions)
- Understand the expected outputs
- Identify any edge cases or error conditions
- Confirm the workflow before writing any code

### 2. **Choose the Right Tool**
- **Python**: For complex logic, file processing, data manipulation, web scraping
- **Bash/Shell**: For simple file operations, system commands, batch processing
- **JavaScript/Node.js**: For web automation, API interactions
- **AppleScript**: For macOS-specific GUI automation (Finder, apps)
- Default to Python for most tasks unless there's a clear reason to use another tool

### 3. **Program Requirements**
Every program MUST include:
- Clear comments explaining what the code does
- Input validation and helpful error messages
- Error handling (try/catch) for common failures
- A help message showing how to use the program
- Logging or progress indicators for long-running tasks
- Example usage in comments at the top of the file

### 4. **File Organization**
- Use descriptive filenames (e.g., `rename_photos_by_date.py`, not `script1.py`)
- Include a shebang line for executable scripts (`#!/usr/bin/env python3` or `#!/bin/bash`)
- Create a `README.md` for each program explaining:
  - What it does
  - How to run it
  - Required dependencies
  - Example usage

### 5. **Testing and Debugging**
- Test the program with sample data before marking as complete
- Handle common error cases (missing files, permissions, invalid inputs)
- Provide clear error messages that explain what went wrong and how to fix it
- If errors occur, debug thoroughly and explain what was fixed

### 6. **Installation and Dependencies**
- Check if dependencies are installed before running
- Provide clear instructions for installing any required packages
- For Python: include `requirements.txt` if needed
- For Node.js: include `package.json` if needed

### 7. **User Instructions**
After creating the program, provide:
- How to make the script executable (`chmod +x script_name.py`)
- How to run it with examples
- What to do if something goes wrong
- How to modify it for different use cases

### 8. **Completion Checklist**
Before marking a program as complete:
- [ ] Code runs without errors
- [ ] Help/usage message is clear
- [ ] Error handling is implemented
- [ ] File has descriptive name
- [ ] Comments explain the code
- [ ] Usage instructions provided
- [ ] Tested with example data
- [ ] User can run it without debugging

### 9. **Git Commits** (REQUIRED)
After EVERY change (creating, modifying, or deleting files):
- Stage all relevant files
- Create a git commit with a clear message
- Commit message should describe what was done (e.g., "Add photo renaming script", "Fix error handling in cleanup program", "Update README with usage examples")
- NEVER skip the commit step - every change must be tracked

## Communication Style
- Use simple, non-technical language when explaining
- Show example commands the user can copy/paste
- Explain what each step does and why
- When errors occur, explain them in plain English

## Platform Considerations for macOS
- Use forward slashes in paths (`/Users/...`)
- Default Python is usually `python3` on Mac
- Consider using Homebrew for installing dependencies
- Be aware of macOS permissions (especially for file access)
- Use `open` command for opening files/applications
