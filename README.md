# Opus UI Dashboard Builder

This JavaScript utility constructs an Opus UI-compatible JSON structure representing a DOM element and its child elements. It includes inline and computed styles (applied through CSS), filters out default or ignored properties, and copies the final dashboard structure to the clipboard.

## Features

- **Style Filtering**: Removes styles that are unnecessary for Opus UI, as specified in `window.ignoreProps`
- **Element Type Mapping**: Identifies elements as `image`, `input`, `label`, or `container`, based on their tag and child nodes, and assigns corresponding Opus UI component types
- **Recursive Element Processing**: Builds a hierarchical JSON structure by recursively traversing all child elements
- **Property Transformation**: Converts CSS properties from kebab-case to camelCase for Opus UI compatibility
- **Clipboard Export**: Copies the resulting JSON Opus UI dashboard configuration to the clipboard

## Usage

1. Navigate to the URL you wish to convert elements from
2. Open your browser's developer console
3. Select (in the DevTools elements panel) the element you wish to convert (this may be `body` also)
3. Copy and paste from `src/index.js` into the console
4. The JSON representation will automatically be copied to the clipboard, ready to be rendered in Opus UI