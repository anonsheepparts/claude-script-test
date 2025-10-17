# Automation Scripts

This repository contains scripts to automate repetitive tasks on your Mac.

## How to Request a New Program

Just describe the repetitive task you want to automate in plain English. Claude will ask clarifying questions, then create a working program for you.

### Examples of Good Requests

**File Management:**
- "I need to rename all photos in a folder by their date taken"
- "Help me organize my downloads folder by file type"
- "Create a program that finds and removes duplicate files"

**Data Processing:**
- "I have a spreadsheet with customer emails and I need to send them all a personalized message"
- "Extract all the phone numbers from a text file and save them in a clean list"
- "Combine multiple CSV files into one"

**Web Tasks:**
- "Download all the images from a webpage"
- "Check a list of websites and tell me which ones are down"
- "Scrape product prices from a website and save them"

**Regular Cleanup:**
- "Delete files older than 30 days from my temp folder"
- "Back up specific folders to another location every day"
- "Find all files larger than 100MB on my computer"

## What to Expect

1. **Questions First** - Claude will ask about your specific needs before writing code
2. **A Working Program** - You'll get a tested script with clear instructions
3. **How to Run It** - Step-by-step instructions for using the program
4. **Error Handling** - The program will tell you clearly if something goes wrong
5. **Documentation** - Comments and explanations so you understand what it does

## Running Your Programs

Most programs will be Python scripts. To run them:

```bash
# Make the script executable (only needed once)
chmod +x program_name.py

# Run the program
./program_name.py
```

Or:

```bash
python3 program_name.py
```

## If Something Goes Wrong

Just tell Claude what error message you saw or what didn't work as expected. Claude will debug it and fix the issue.

## Tips for Best Results

- Be specific about what files or data you're working with
- Mention if you want to process one file or many files
- Say whether you want the program to ask for confirmation or run automatically
- If you have an example of the input and what you want as output, share that

## Getting Started

Try asking: "I want to create a program that..." and describe your repetitive task!
