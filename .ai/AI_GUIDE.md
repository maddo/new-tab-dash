# AI Guide for New Tab Dashboard

This document provides guidance for AI assistants working with this new tab dashboard project.

## Project Overview
This is a single-page HTML application designed to be used as a browser's new tab page. It displays GitHub pull request information in a clean, dark-themed interface. The project consists of both a web application and a Chrome extension to handle CORS and other browser-specific functionality.

## Key Components

### 1. Core Files
- `new_tab_dash.html`: The main application file containing all HTML, CSS, and JavaScript
- `new-tab-dash-extension/`: Chrome extension directory
  - `background.js`: Handles CORS and network requests
  - `manifest.json`: Extension configuration
- `README.md`: User documentation and setup instructions
- `TODO.md`: Project roadmap and planned features
- `CLEANUP.md`: Code cleanup and improvement tasks

### 2. Main Features
- Dark theme with modern design
- GitHub PR review request display
- Personal open PR display
- Secure token management
- Real-time updates
- Responsive layout
- CORS handling via Chrome extension
- Cross-browser compatibility

### 3. Technical Implementation
- Pure HTML/CSS/JavaScript implementation
- Uses localStorage for token storage
- GitHub API integration
- Chrome extension for CORS handling
- Single-file architecture for main application
- Modular extension structure

## AI Development Guidelines

### 1. Code Structure
- Main application code is contained in a single HTML file
- Extension code follows modular structure
- CSS is in the `<style>` section of main HTML
- JavaScript is in the `<script>` section of main HTML
- Follow the existing code organization pattern
- Maintain separation between extension and main app code

### 2. Security Considerations
- Never expose full GitHub tokens
- Always use secure token handling methods
- Maintain existing security measures
- Keep token storage in localStorage
- Review CORS settings in extension
- Implement proper error handling for API calls
- Validate all user inputs
- Follow security best practices for Chrome extensions

### 3. UI/UX Guidelines
- Maintain dark theme (#000000 background)
- Use consistent color scheme
- Keep clean, minimal design
- Ensure responsive layout
- Follow existing component styling
- Maintain accessibility standards
- Use semantic HTML elements
- Implement proper ARIA labels

### 4. Feature Development
When adding new features:
1. Keep the single-file architecture for main app
2. Maintain existing security measures
3. Follow the established UI patterns
4. Ensure mobile responsiveness
5. Add appropriate error handling
6. Consider extension compatibility
7. Document new features
8. Update relevant documentation

### 5. Common Tasks
- Token management
- GitHub API integration
- UI updates
- Error handling
- Performance optimization
- Extension configuration
- CORS handling
- Cross-browser testing

### 6. Testing Guidelines
- Test in multiple browsers (Chrome, Firefox, Safari)
- Verify token security
- Check responsive design
- Validate API calls
- Test error scenarios
- Verify extension functionality
- Test CORS handling
- Validate cross-browser compatibility

## Best Practices
1. Keep the single-file architecture for main app
2. Maintain existing security measures
3. Follow established UI patterns
4. Document any new features
5. Test thoroughly before suggesting changes
6. Consider extension compatibility
7. Follow Chrome extension best practices
8. Maintain cross-browser compatibility
9. Keep code organized and maintainable
10. Follow accessibility guidelines

## Common Pitfalls to Avoid
1. Breaking the single-file structure
2. Compromising security measures
3. Deviating from the dark theme
4. Adding unnecessary dependencies
5. Overcomplicating the UI
6. Neglecting extension compatibility
7. Ignoring cross-browser issues
8. Forgetting to update documentation
9. Skipping proper testing
10. Violating Chrome extension policies

## Future Development Suggestions
1. Add more GitHub metrics
2. Implement customizable themes
3. Add more organization features
4. Enhance error handling
5. Improve performance
6. Add more extension features
7. Implement better state management
8. Add automated testing
9. Improve documentation
10. Add analytics capabilities

## Support
For any questions or issues, refer to:
- The README.md for user documentation
- The main HTML file for implementation details
- The extension files for browser-specific functionality
- This guide for development guidelines
- TODO.md for planned features
- CLEANUP.md for improvement tasks 