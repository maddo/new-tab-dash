# GitHub PR Dashboard

A clean, dark-themed browser start page that displays your GitHub pull request review requests and your own open pull requests.

## Features

- Dark theme with clean, modern design
- Displays count and list of PRs awaiting your review
- Shows your own open pull requests
- Secure token management using localStorage
- Real-time updates
- Responsive design

## Security

This application:
- Stores GitHub tokens securely in localStorage
- Only displays the last 4 characters of the token
- Automatically clears invalid tokens
- Never exposes full tokens in the UI
- Requires user consent for token storage

## Setup

1. Clone this repository or download the `new_tab_dash.html` file
2. Set up your GitHub token:
   - Go to [GitHub Settings > Developer Settings > Personal Access Tokens](https://github.com/settings/tokens)
   - Generate a new token with `repo` scope
   - Copy the token and paste it into the dashboard when prompted

## Setting as Browser Start Page

### Chrome
1. Open Chrome settings
2. Go to "On startup" section
3. Select "Open a specific page or set of pages"
4. Click "Add a new page"
5. Enter the full path to your local HTML file:
   ```
   file:///path/to/your/new_tab_dash.html
   ```
   For example:
   ```
   file:///Users/username/Documents/new_tab_dash.html
   ```

### Chromium
1. chrome://flags/#custom-new-tab-page

### Firefox
1. Open Firefox settings
2. Go to "Home" section
3. Under "Homepage and new windows", select "Custom URLs"
4. Enter the full path to your local HTML file:
   ```
   file:///path/to/your/new_tab_dash.html
   ```
   For example:
   ```
   file:///Users/username/Documents/new_tab_dash.html
   ```

## Troubleshooting

- If the page doesn't load, ensure you're using the correct file path format
- Make sure the file path doesn't contain spaces (use %20 for spaces if needed)
- Verify file permissions allow the browser to read the file
- Check browser console for any error messages

## Contributing

Feel free to submit issues and enhancement requests!

## License``

MIT License - feel free to use and modify as needed. 