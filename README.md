# PromptBook - Chrome Extension

Save and organize your AI prompts from ChatGPT, Claude, Gemini, and more.

## Features (MVP)

- **Quick Save**: "Save Prompt" button appears next to text fields in AI applications
- **Auto-Detection**: Automatically detects which AI app you're using
- **Categorization**: Organize by application and use case (Coding, Marketing, Creative, Business)
- **Search**: Find prompts instantly with real-time search
- **Copy to Clipboard**: One-click copy for easy pasting
- **Tags**: Add custom tags for better organization
- **Export/Import**: Backup and restore your prompts

## Supported AI Applications

- ChatGPT (chat.openai.com, chatgpt.com)
- Claude (claude.ai)
- Gemini (gemini.google.com)
- NotebookLM (notebooklm.google.com)
- Perplexity (perplexity.ai)

## Installation

### Step 1: Generate Icons

1. Open `assets/icons/generate-icons.html` in your browser
2. Download each icon (16x16, 48x48, 128x128)
3. Save them as `icon16.png`, `icon48.png`, `icon128.png` in the `assets/icons/` folder

### Step 2: Load in Chrome

1. Open Chrome and go to `chrome://extensions/`
2. Enable "Developer mode" (toggle in top-right)
3. Click "Load unpacked"
4. Select the `PromptBook` folder
5. The extension icon should appear in your toolbar

## Usage

### Saving Prompts

1. Visit any supported AI website (ChatGPT, Claude, etc.)
2. Type your prompt in the input field
3. Click the "Save" button that appears
4. Fill in the title, category, and tags
5. Click "Save Prompt"

### Managing Prompts

1. Click the PromptBook icon in your toolbar
2. Browse, search, or filter your saved prompts
3. Click a prompt to view details
4. Use the copy button to copy to clipboard
5. Edit or delete prompts as needed

### Adding Prompts Manually

1. Click the PromptBook icon
2. Click the "+" button in the header
3. Fill in the prompt details
4. Click "Save"

## File Structure

```
PromptBook/
├── manifest.json           # Extension configuration
├── popup/
│   ├── popup.html         # Main popup UI
│   ├── popup.css          # Popup styles
│   └── popup.js           # Popup logic
├── content/
│   ├── content.js         # Injected into AI sites
│   └── content.css        # Content script styles
├── background/
│   └── service-worker.js  # Background tasks
├── utils/
│   ├── storage.js         # Storage operations
│   └── sites.js           # Site configuration
└── assets/
    └── icons/             # Extension icons
```

## Categories

### By Application
- ChatGPT
- Claude
- Gemini
- NotebookLM
- Perplexity
- Other

### By Use Case
- **Coding**: Debugging, Refactoring, Documentation, Code Review
- **Marketing**: Social Media, Ad Scripts, SEO, Email Campaigns
- **Creative Writing**: Storytelling, Poetry, Scripts, Blog Posts
- **Business**: Email Drafting, Meeting Summaries, Reports, Proposals
- **Research**: Literature Review, Data Analysis, Fact Checking, Summarization
- **Education**: Lesson Plans, Explanations, Quiz Creation, Study Guides

## Future Pro Features

- Cloud Sync across devices
- Prompt Variables (templates with placeholders)
- Team Sharing for organizations
- Advanced analytics

## Development

### Testing Changes

1. Make your changes to the code
2. Go to `chrome://extensions/`
3. Click the refresh icon on the PromptBook card
4. Test your changes

### Debugging

- **Popup**: Right-click the extension icon → "Inspect popup"
- **Content Script**: Open DevTools on the AI site → Console
- **Service Worker**: `chrome://extensions/` → "Service worker" link

## License

MIT License
