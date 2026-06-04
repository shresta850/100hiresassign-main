# 100Hires 

## Tools Installed
- Cursor IDE - AI-powered code editor workspace.
- Claude Code for VS Code (by Anthropic) - AI coding extension.
- Codex - OpenAI's coding agent extension.
- Node.js v24.16.0 - Required local runtime environment for terminal-based AI dependencies.
- GitHub - Version control and repository hosting platform.

## Steps Completed
1. Created a Cursor account and installed Cursor IDE from cursor.com
2. Created a GitHub account at github.com
3. Connected GitHub account to Cursor during initial setup
4. Attempted to install Claude Code extension - discovered Extensions 
   panel was not loading properly
5. Researched the issue and found that Claude Code extension requires 
   Node.js v18 or higher to function
6. Downloaded and installed Node.js v24.16.0 from nodejs.org
7. Restarted Cursor - full Extensions panel became available
8. Installed Claude Code for VS Code extension by Anthropic
9. Installed Codex - OpenAI's coding agent extension
10. Created a public GitHub repository named 100hiresassign
11. Opened the repository in Cursor
12. Created and documented this README.md file

## Issues Encountered & Solutions

### Issue 1: Mismatched IDE Interface & Missing Extensions Panel
Upon launching Cursor, the standard VS Code Extensions panel (`Ctrl+Shift+X`) was entirely missing or replaced with a basic "Customize" layout. The interface did not match tutorials, and searching for "Claude Code" or "Codex" yielded no results.

*Solution: Attempted several UI fixes (logging out/in, testing alternate accounts, exploring all settings panels). Realized the IDE's extension architecture wasn't fully loading due to a missing backend environment dependency. 

### Issue 2: Terminal Command Error ("npm not recognized")
Attempted to bypass the broken UI by installing the tool directly via the Cursor terminal using the command: `npm install -g @anthropic-ai/claude-code`. This returned a critical command-line error stating that `npm` was not recognized as a cmdlet or executable program.

*Solution: Used Claude AI to translate the error block. The AI confirmed that `npm` is bundled with Node.js, proving that a local JavaScript runtime environment was completely missing from the PC.

### Issue 3: Activating the Correct Environment
Downloaded the latest LTS version of Node.js (v24.16.0) from [nodejs.org](https://nodejs.org/). Initially, the UI didn't update immediately.

*Solution: Closed the IDE and restarted the computer to allow the new system path variables to take effect. Upon re-opening Cursor, the full extensions marketplace loaded perfectly, confirming that Claude Code's background agent loop requires a local Node.js environment to run.

## Key Learnings
- Claude Code extension requires Node.js v18+ to function in Cursor
- Cursor has two separate add-on systems: Cursor Marketplace and VS Code Extensions - they serve different purposes
- npm comes bundled with Node.js and is not a standalone installation
- GitHub repositories can be opened directly inside Cursor as a workspace
- Documenting errors and their solutions is as valuable as the solution itself
