# YouTube Summarizer

A lightweight Chrome extension that summarizes YouTube videos using AI models.

## Features

- **Fast Summarization**: Extract YouTube video transcripts and generate summaries in seconds
- **Multiple AI Models**: Choose from ChatGPT, Claude, Gemini, Mistral, Grok, and more
- **Easy to Use**: Simple interface with one-click summarization
- **Works on YouTube**: Automatically detects YouTube videos and provides summarization options

## Installation

1. Clone or download this repository
2. Open Chrome and go to `chrome://extensions/`
3. Enable "Developer mode" (top right corner)
4. Click "Load unpacked" and select this repository folder
5. The extension will now appear in your Chrome toolbar

## Usage

1. Visit any YouTube video
2. Click the summarizer button in the extension
3. Choose your preferred AI model from the settings
4. Get an instant summary of the video

## Configuration

Open the extension settings to:
- Select your preferred AI model (ChatGPT, Claude, Gemini, etc.)
- Customize the summarization prompt
- Choose between on-page or new-tab summarization

## Supported AI Models

- ChatGPT (OpenAI)
- Claude (Anthropic)
- Gemini (Google)
- Mistral AI
- Grok
- And more...

## Technical Details

- **Manifest Version**: 3
- **Content Script**: YouTube pages only (`*.youtube.com`)
- **Permissions**: `tabs`, `storage`
- **Size**: Minimal (~1.5 MB with bundled dependencies)

## Development

This extension was created from the Glasp project and stripped down to YouTube summarization only.

### Build

To rebuild from source, you'll need webpack and the original source files.

### Directory Structure

```
├── manifest.json           # Extension configuration
├── background.bundle.js    # Service worker
├── iframe/                 # Content scripts
│   └── iframe-index.bundle.js
├── css/
│   └── yt_summary.css
├── images/                 # Extension icons
└── options/                # Settings page
```

## License

This project is based on the Glasp extension.

## Support

For issues or feature requests, please create an issue in the repository.
