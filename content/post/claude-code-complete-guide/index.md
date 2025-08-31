---
title: Claude Code - Complete Beginner's Guide
subtitle: Everything you need to get started with Claude Code effectively

# Summary for listings and search engines
summary: A comprehensive guide covering installation, essential commands, best practices, and advanced features for Claude Code across VS Code and Cursor editors.

# Link this post with a project
projects: []

# Date published
date: '2025-08-31T00:00:00Z'

# Date updated
lastmod: '2025-08-31T00:00:00Z'

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: true

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: 'Claude Code - AI-powered coding assistant'
  focal_point: ''
  placement: 2
  preview_only: false

authors:
  - admin

tags:
  - AI Tools
  - Programming
  - Claude Code
  - VS Code
  - Cursor
  - Developer Tools

categories:
  - Technical Guide
  - AI Tools
---

# Claude Code: Complete Beginner's Guide

[**View Course Files on GitHub**](https://github.com/https-deeplearning-ai/sc-claude-code-files/tree/main)

## Table of Contents

- [Getting Started](#getting-started)
- [Prompts](#prompts)
- [Summary of Claude Code Features](#summary-of-claude-code-features)
- [Essential Commands](#essential-commands)
- [Best Practices for Beginners](#best-practices-for-beginners)
- [Common Use Cases](#common-use-cases)
- [Troubleshooting](#troubleshooting)
- [Advanced Features](#advanced-features)
- [Additional Resources](#additional-resources)
- [Quick Reference Card](#quick-reference-card)

## Getting Started

### What is Claude Code?

Claude Code is an AI-powered coding assistant that helps you understand, write, debug, and refactor code. It can work with your entire codebase and maintain context across conversations.

### Installation Instructions

### For VS Code Users

### **macOS Installation**

1. **Install VS Code** (if not already installed):
    
    ```bash
    # Using Homebrew
    brew install --cask visual-studio-code
    
    # Or download from: https://code.visualstudio.com/
    
    ```
    
2. **Install Claude Code Extension**:
    - Open VS Code
    - Go to Extensions (`Cmd + Shift + X`)
    - Search for "Claude Code" or "Anthropic Claude"
    - Click "Install"
    
    **Alternative: Command Line**
    
    ```bash
    code --install-extension anthropic.claude-code
    
    ```
    
3. **Setup Authentication**:
    - Open Command Palette (`Cmd + Shift + P`)
    - Type "Claude: Sign In"
    - Follow the authentication prompts
    - Enter your Anthropic API key when prompted

### **Windows Installation**

1. **Install VS Code** (if not already installed):
    - Download from: https://code.visualstudio.com/
    - Run the installer as Administrator
    - Choose "Add to PATH" during installation
2. **Install Claude Code Extension**:
    - Open VS Code
    - Go to Extensions (`Ctrl + Shift + X`)
    - Search for "Claude Code" or "Anthropic Claude"
    - Click "Install"
    
    **Alternative: Command Line**
    
    ```bash
    code --install-extension anthropic.claude-code
    
    ```
    
3. **Setup Authentication**:
    - Open Command Palette (`Ctrl + Shift + P`)
    - Type "Claude: Sign In"
    - Follow the authentication prompts
    - Enter your Anthropic API key when prompted

### For Cursor Users

### **macOS Installation**

1. **Install Cursor**:
    
    ```bash
    # Download from: https://cursor.sh/
    # Or using Homebrew
    brew install --cask cursor
    
    ```
    
2. **Install Claude Code Extension**:
    - Open Cursor
    - Go to Extensions (`Cmd + Shift + X`)
    - Search for "Claude Code" or "Anthropic Claude"
    - Click "Install"
    
    **Alternative: Command Line**
    
    ```bash
    # If you have npm installed
    npm install -g @anthropic-ai/claude-code
    
    # Or use the extension marketplace
    cursor --install-extension anthropic.claude-code
    
    ```
    
3. **Setup Authentication**:
    - Open Cursor
    - Go to Settings (`Cmd + ,`)
    - Navigate to "AI" or "Claude" settings
    - Enter your Anthropic API key
    - Or use Cursor's built-in authentication

### **Windows Installation**

1. **Install Cursor**:
    - Download from: https://cursor.sh/
    - Run the installer as Administrator
    - Follow the installation wizard
2. **Install Claude Code Extension**:
    - Open Cursor
    - Go to Extensions (`Ctrl + Shift + X`)
    - Search for "Claude Code" or "Anthropic Claude"
    - Click "Install"
    
    **Alternative: Command Line**
    
    ```bash
    # If you have npm installed
    npm install -g @anthropic-ai/claude-code
    
    # Or use the extension marketplace
    cursor --install-extension anthropic.claude-code
    
    ```
    
3. **Setup Authentication**:
    - Open Cursor
    - Go to Settings (`Ctrl + ,`)
    - Navigate to "AI" or "Claude" settings
    - Enter your Anthropic API key
    - Or use Cursor's built-in authentication

### Getting Your API Key

1. **Create an Anthropic Account**:
    - Visit: https://console.anthropic.com/
    - Sign up or log in
2. **Generate API Key**:
    - Go to "API Keys" section
    - Click "Create Key"
    - Copy your API key (keep it secure!)
3. **Set Usage Limits** (recommended):
    - Set monthly spending limits
    - Monitor your usage regularly

### First Steps After Installation

1. **Navigate to your project directory** in the terminal
2. **Open your editor** (VS Code or Cursor)
3. **Launch Claude Code**:
    - **VS Code**: Use Command Palette (`Cmd/Ctrl + Shift + P`) → "Claude: Start Chat"
    - **Cursor**: Use the built-in chat interface or `Cmd/Ctrl + L`
4. **Run `/init`** to let Claude scan your codebase and create a `CLAUDE.md` file
5. **Start coding!** Ask Claude questions about your code or request help with tasks

### Setting Up Your First Project

```bash
# Navigate to your project
cd your-project-directory

# Open in your editor
code .          # For VS Code
cursor .        # For Cursor

# In Claude Code interface, run:
/init

```

### Verification Steps

After installation, verify everything works:

1. **Test Basic Commands**:
    
    ```
    /init          # Should scan your project
    /clear         # Should clear chat history
    
    ```
    
2. **Test File References**:
    
    ```
    @package.json  # Should load file content
    
    ```
    
3. **Test Project Understanding**:
    
    ```
    "Explain what this project does"
    
    ```

### Troubleshooting Installation

### Common Issues:

- **API Key Issues**: Make sure your key is valid and has sufficient credits
- **Extension Not Loading**: Restart your editor after installation
- **Permission Errors**: Run installer as Administrator (Windows) or check file permissions (macOS)
- **Network Issues**: Check firewall settings and proxy configuration

### Getting Help:

- Check the official documentation
- Visit the Anthropic support portal
- Join the community forums

## Prompts

Here are the links to the lessons' notes and prompts:

- [Prompts of Lesson 2: Setup & Codebase Understanding](https://www.notion.so/Claude-Code-25f68bac67ab8024a5e6fb72a4e94c10?pvs=21)
- [Prompts of Lesson 3: Adding Features](https://www.notion.so/Claude-Code-25f68bac67ab8024a5e6fb72a4e94c10?pvs=21)
- [Prompts of Lesson 4: Testing, Error Debugging and Code Refactoring](https://www.notion.so/Claude-Code-25f68bac67ab8024a5e6fb72a4e94c10?pvs=21)
- [Prompts of Lesson 5: Adding Multiple Features Simultaneously - Using Git Worktrees](https://www.notion.so/Claude-Code-25f68bac67ab8024a5e6fb72a4e94c10?pvs=21)
- [Notes for Lesson 6: References to GitHub Integration & Hooks](https://www.notion.so/Claude-Code-25f68bac67ab8024a5e6fb72a4e94c10?pvs=21)
- [Prompts of Lesson 7: Refactoring a Jupyter Notebook & Creating a Dashboard](https://www.notion.so/Claude-Code-25f68bac67ab8024a5e6fb72a4e94c10?pvs=21)
- [Prompts of Lesson 8: Creating Web App based on a Figma Mockup](https://www.notion.so/Claude-Code-25f68bac67ab8024a5e6fb72a4e94c10?pvs=21)

## Summary of Claude Code Features

### Managing Project Memory

### Types of CLAUDE.md Files

There are three types of CLAUDE.md files, each serving different purposes:

| File Type | Location | Purpose | Sharing |
| --- | --- | --- | --- |
| **`CLAUDE.md`** | Project directory | Generated with `/init`<br/>Contains project structure, architecture, and coding style<br/>Shared with team | ✅ Commit to source control<br/>✅ Shared with other engineers |
| **`CLAUDE.local.md`** | Project directory | Personal instructions and customizations<br/>Not shared with other engineers<br/>Contains your personal preferences | ❌ Not shared (add to .gitignore)<br/>❌ Personal use only |
| **`~/.claude/CLAUDE.md`** | User home directory | Global settings and preferences<br/>Applies to all projects<br/>Personal configuration | ❌ Not shared<br/>❌ Personal system-wide settings |

### Setting Up Your CLAUDE.md Files

- **`/init`**: Claude Code scans your codebase and creates `CLAUDE.md` file inside your project directory.
    - `CLAUDE.md` guides Claude through your codebase, pointing out important commands, architecture and coding style. It's automatically included in the context each time you launch Claude Code.
    - Here's an [example of a CLAUDE.md file generated by init for the RAG chatbot example](https://www.notion.so/Claude-Code-25f68bac67ab8024a5e6fb72a4e94c10?pvs=21).
- **`#`**: Use `#` to quickly add a memory. Useful when you see Claude Code repeats an error.
    
    **Example 1:** Since the project is a uv project, we added these to `CLAUDE.md` file using `#`:
    
    ```
    #use uv to run python files or add any dependencies
    
    ```
    
    **Example 2:** You can inform Claude Code about the database schema, in this case since you have a vector database, you can inform Claude Code about the collections stored in the vector database:
    
    ```
    #The vector database has two collections:
    course_catalog:
    stores course titles for name resolution
    metadata for each course: title, instructor, course_link, lesson_count, lessons_json (list of lessons: lesson_number, lesson_title, lesson_link)
    course_content:
    stores text chunks for semantic search
    metadata for each chunk: course_title, lesson_number, chunk_index
    
    ```

## Essential Commands

| Command | Description |
| --- | --- |
| `/clear` | clears current conversation history |
| `/compact` | summarizes current conversation history |
| `ESC` | interrupt Claude to redirect or correct it |
| `ESC ESC` | rewind the conversation to an earlier point in time |
| `@` | Mention files with `@` to include its content in your request |
| `/mcp` | Manage MCP connection & check available MCP servers with their provided tools (MCP with Claude Code) |

You can use regular bash command within Claude Code, but you need to start the command with `!` (for example: `!pwd`). You can type `exit` to quit Claude Code.

### Shortcuts

| Shortcut | Description |
| --- | --- |
| `shift+tab` | switch between planning and auto-accept mode |
| take a screenshot | `cmd+ shift+ ctrl + 4` (Mac) or `Win + Shift + S` (Windows) |
| paste a screenshot | `Ctrl + V` (might not work on Windows) |

## Best Practices for Beginners

### 1. Start with `/init`

Always run `/init` when you start working on a new project. This helps Claude understand your codebase structure and coding style.

### 2. Be Specific in Your Requests

Instead of: "Fix my code"
Try: "Fix the authentication bug in the login function where users can't log in with valid credentials"

### 3. Use `@` to Reference Files

When asking about specific files, use `@filename.py` to include the file content in your request.

### 4. Break Down Complex Tasks

For large features, break them into smaller, manageable steps:

- "Create the user model"
- "Add user authentication"
- "Create the user dashboard"

### 5. Utilize Project Memory

Use `#` to add important project-specific information to the appropriate `CLAUDE.md` file:

**For team-shared information (add to `CLAUDE.md`):**

```
#This project uses Django with PostgreSQL
#All API endpoints should return JSON responses
#Follow PEP 8 style guidelines

```

**For personal preferences (add to `CLAUDE.local.md`):**

```
#I prefer verbose error messages in debugging
#Always explain the reasoning behind code suggestions
#Use my preferred variable naming convention: snake_case

```

### 6. Ask for Explanations

Don't just ask for code - ask Claude to explain what it's doing:
"Explain how this authentication system works and why you chose this approach"

## Common Use Cases

### Understanding Existing Code

- "Explain what this function does: `@utils.py`"
- "Walk me through the authentication flow in this app"
- "What does this error message mean and how do I fix it?"

### Writing New Code

- "Create a REST API endpoint for user registration"
- "Write unit tests for the payment processing module"
- "Add error handling to the database connection function"

### Debugging

- "Why is my React component not re-rendering when state changes?"
- "Help me debug this SQL query that's returning unexpected results"
- "Fix the memory leak in this Python script"

### Refactoring

- "Refactor this function to be more readable and efficient"
- "Convert this class-based component to a functional component with hooks"
- "Optimize this database query for better performance"

### Learning

- "Explain the difference between async/await and Promises in JavaScript"
- "Show me best practices for error handling in Python"
- "What are the security considerations for this authentication method?"

## Troubleshooting

### Common Issues and Solutions

### Issue: Claude doesn't understand my project structure

**Solution:** Run `/init` and make sure `CLAUDE.md` is created. Add project-specific information using `#`.

### Issue: Claude gives generic answers

**Solution:** Be more specific, use `@` to reference files, and provide context about your project.

### Issue: Long conversation becomes slow

**Solution:** Use `/compact` to summarize the conversation or `/clear` to start fresh.

### Issue: Claude repeats the same mistakes

**Solution:** Add a note to `CLAUDE.md` using `#` to remind Claude about the specific requirement.

### Issue: Need to undo recent changes

**Solution:** Use `ESC ESC` to rewind the conversation to an earlier point.

### Getting Help

- Use "think" for complex problems that need deeper analysis
- Ask Claude to break down complex tasks into steps
- Request explanations for any code or concepts you don't understand

## Advanced Features

### Extended Thinking Mode

For complex tasks (e.g., complex architectural changes, debugging complicated issues), you can use the word "think" to trigger extended thinking mode. There are several levels of thinking:

`"think"` < `"think hard"` < `"think harder"` < `"ultrathink"`

Each level allocates more thinking budget for Claude.

### Use of Subagents

You've learned that one of the out-of-the-box tools for Claude Code is **Task**, which Claude Code can use to launch subagents for complex multi-step tasks. You can explicitly ask Claude Code to use subagents to brainstorm ideas or to investigate multiple aspects of a question or a problem you want to solve. These built-in agents are of general purpose.

You can also create your customized specialized subagents. Each subagent has its own context window, and you can define a custom system prompt and specific tools for each subagent. This part is not covered in this course, but you can check the details in the [documentation here](https://www.notion.so/Claude-Code-25f68bac67ab8024a5e6fb72a4e94c10?pvs=21).

## Additional Resources

To learn more about these features as well as other features, you can check:

- [Claude Code Documentation](https://www.notion.so/Claude-Code-25f68bac67ab8024a5e6fb72a4e94c10?pvs=21)
- [Claude Code Common Workflows](https://www.notion.so/Claude-Code-25f68bac67ab8024a5e6fb72a4e94c10?pvs=21)
- [Claude Code Best Practices](https://www.notion.so/Claude-Code-25f68bac67ab8024a5e6fb72a4e94c10?pvs=21)
- [Claude Code Use Cases](https://www.notion.so/Claude-Code-25f68bac67ab8024a5e6fb72a4e94c10?pvs=21)

There's also a great course on Anthropic Academy that you can check out to see more examples with Claude Code:

- [Claude Code in Action](https://www.notion.so/Claude-Code-25f68bac67ab8024a5e6fb72a4e94c10?pvs=21)

## Quick Reference Card

### Essential Commands for Daily Use

```
/init          # Initialize project understanding
/clear         # Clear conversation history
/compact       # Summarize conversation
@filename      # Include file in request
#note          # Add to project memory
ESC            # Interrupt Claude
ESC ESC        # Rewind conversation
!command       # Run bash command

```

### Sample Beginner Prompts

```
# Getting started
"Help me understand what this codebase does"
"Explain the main components of this project"

# Writing code
"Create a function that validates email addresses"
"Add error handling to this API endpoint"

# Debugging
"Why is this test failing?"
"Help me fix this TypeError"

# Learning
"Explain this design pattern to me"
"What are the best practices for this framework?"

```

### Pro Tips for Beginners

1. **Always start with `/init`** on new projects
2. **Be specific** - include error messages, file names, and context
3. **Use `@` liberally** to reference files
4. **Ask for explanations** not just solutions
5. **Break large tasks** into smaller steps
6. **Choose the right CLAUDE.md file:**
    - Team info → `CLAUDE.md` (shared)
    - Personal preferences → `CLAUDE.local.md` (private)
    - Global settings → `~/.claude/CLAUDE.md` (system-wide)
7. **Use `/compact`** when conversations get long
8. **Don't hesitate to ask** "why" or "how does this work?"

---

*This guide represents my curated notes and insights from working with Claude Code. As AI tools continue to evolve rapidly, I'll keep this post updated with the latest best practices and features.*