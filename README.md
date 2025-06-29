# Lead Tracker Chrome Extension

This is a simple Chrome extension-style web app that allows users to save and manage a list of URLs (leads). It includes functionality for manual input, saving the current browser tab, and clearing all saved leads. All data is stored in the browser's `localStorage`.

## Features

- ✅ Save input manually via a text box.
- ✅ Save the current browser tab URL.
- ✅ Persist leads using `localStorage`.
- ✅ Render saved links as clickable items.
- ✅ Delete all saved leads on double-click.

## Tech Stack

- HTML
- CSS
- JavaScript
- Chrome Extension APIs (`chrome.tabs`)

## Files

### `index.html`

Defines the UI structure including:
- Input field for manual URLs
- Buttons to save input, save current tab, and delete all leads
- An unordered list to display saved URLs

### `index.css`

Styles the UI elements with:
- Responsive input and button layout
- Minimalist green-and-white color scheme
- List-style presentation for URLs

### `index.js`

Contains all the core JavaScript logic:
- Stores and retrieves leads from `localStorage`
- Saves URLs via input or current active tab
- Renders leads as clickable list items
- Clears storage on double-click

## How to Use

1. Open the app in a browser that supports `chrome.tabs` (like Chrome).
2. Type a URL in the input box and click "SAVE INPUT" to add it.
3. Click "SAVE TAB" to save the current tab’s URL.
4. Click "DELETE ALL" twice quickly to clear all saved leads.

## Notes

- To enable the `chrome.tabs` API, this project is meant to be used as a Chrome Extension.
- If running as a regular webpage, the "SAVE TAB" button will not function unless loaded as an extension with appropriate permissions.

## License

MIT License – free to use and modify.
