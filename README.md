# New Tab Dashboard

A clean, dark-themed browser start page that displays your GitHub pull request review requests, your own open pull requests, and Jira tickets.

## Features

- Dark theme with clean, modern design
- Shows open PR reviews assigned to you
- Shows your own open pull requests
- Shows your open Jira tickets
- Status indicators for GitHub and Jira connections
- Settings panel for configuration
- Caching to reduce API calls

## Setup Instructions

### 1. Main Dashboard Setup

1. Download or clone this repository
2. Set `new_tab_dash.html` as your new tab page:
   - Chrome: Go to `chrome://settings/` > "On startup" > "Open a specific page" > Add `file:///path/to/new_tab_dash.html`
   - Firefox: Go to `about:preferences` > "Home" > "Custom URLs" > Add `file:///path/to/new_tab_dash.html`

### 2. CORS Extension Setup (for Jira)

To enable Jira integration, you'll need to install a small companion extension that handles CORS:

1. Create a new directory called `jira-cors-extension` with these files:

```
jira-cors-extension/
├── manifest.json
└── background.js
```

2. Load the extension in Chrome:
   - Open Chrome and go to `chrome://extensions/`
   - Enable "Developer mode" in the top right
   - Click "Load unpacked" and select the `jira-cors-extension` directory

### 3. Configure GitHub

1. Click the gear icon in the bottom left of the new tab page
2. Generate a GitHub token:
   - Go to https://github.com/settings/tokens
   - Click "Generate new token"
   - Select the `repo` scope
   - Copy the token
3. Paste the token in the GitHub configuration section
4. Click "Save Token"

### 4. Configure Jira

1. Click the gear icon in the bottom left of the new tab page
2. Generate a Jira API token:
   - Go to https://id.atlassian.com/manage/api-tokens
   - Click "Create API token"
   - Copy the token
3. Enter your Jira configuration:
   - Domain: Your Jira domain (e.g., `chesscom` for `chesscom.atlassian.net`)
   - Email: Your Jira account email
   - API Token: The token you generated
4. Click "Save Jira Config"

## Troubleshooting

### CORS Issues with Jira

If you see CORS errors in the console:
1. Make sure the CORS extension is properly loaded
2. Check that the background script is running
3. Verify the extension has the necessary permissions

### API Token Issues

If GitHub or Jira connections fail:
1. Verify your tokens are correct
2. Check that the tokens have the necessary permissions
3. Try generating new tokens

### Cache Issues

If data isn't updating:
1. The cache refreshes every 5 minutes
2. You can force a refresh by reloading the page
3. Check the cache timer in the bottom right

## Development

To modify the dashboard:
1. Make changes to `new_tab_dash.html`
2. Reload your new tab page

To modify the CORS extension:
1. Make changes to the extension files
2. Go to `chrome://extensions/`
3. Click the refresh icon on the extension card

## License

MIT 