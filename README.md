# Markdown for Dev.to - Gemini CLI Extension

This extension provides tools to help format and fix Markdown content for publication on [Dev.to](https://dev.to).

## Installation

To install this extension, use the Gemini CLI `extension add` command:

```bash
gemini extension install https://github.com/derailed-dash/markdown-for-dev.to --auto-update
```

## Commands

### `devto-md`

Process a markdown file to fix common issues and prepare it for Dev.to.

**Features:**
- Adds/fixes YAML frontmatter.
- Converts raw Twitter and YouTube links to Liquid tags.
- Fixes image captions and missing alt text.
- Properly highlights inline variables and file paths.
- Adds language tags to code blocks.
- Removes unwanted "highlighted" artifacts.

**Usage:**

**Option 1: Direct Text Input (Copy/Paste)**

Encapsulate your text in quotes to avoid shell issues.

```bash
gemini devto-md "# My Title\n\nSome content..."
```

**Option 2: From a File**

Use command substitution to pass the file contents.

```bash
gemini devto-md "$(cat path/to/post.md)"
```
