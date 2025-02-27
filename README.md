# Googlespreadsheet
# Spreadsheet Web App

A web-based spreadsheet application that allows users to enter and calculate formulas, perform mathematical operations, and interact with cells and ranges like a basic version of Google Sheets.

## Features

- **Cell Editing**: Users can input data or formulas into cells.
- **Mathematical Operations**: Supported by Math.js for evaluating complex formulas.
- **Cell Selection**: Users can select cells, ranges, and modify values.
- **Formula Evaluation**: Supports dynamic formulas and recalculation based on dependencies.
- **Cycle Detection**: Detects circular references when updating cells.
- **Responsive Interface**: Uses the HTML `contenteditable` attribute for user input.
- **Canvas Rendering**: The grid is rendered on a `<canvas>` element for smooth interaction.

## Tech Stack

- **HTML5**: For the structure of the page.
- **JavaScript**: For handling all interactions, formulas, and dynamic updates.
- **Math.js**: A library for performing advanced mathematical calculations.
- **Canvas**: Used to render the spreadsheet grid and manage visual interactions.

## Setup

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/spreadsheet-web-app.git
    ```

2. **Open the `index.html` file**:
    Open the `index.html` file in a web browser to view the spreadsheet application.

3. **Dependencies**:
    - Math.js is included via CDN in the `<head>` tag. No other dependencies are required for the basic functionality.

## Usage

- **Navigating the Spreadsheet**:
    - Use arrow keys to move between cells.
    - Use `Shift + Arrow` keys to expand the selection range.
    - Press `Enter` to start editing the selected cell.
    - Press `Backspace` to delete the content of the selected cell.

- **Editing Cells**:
    - Select a cell by clicking on it.
    - Enter data or formulas (e.g., `=A1+B1`).
    - Press `Enter` to apply changes and move to the next cell.

- **Formula Evaluation**:
    - Formulas are automatically evaluated and recalculated when their dependencies change.
    - Circular references are detected and an alert is shown when trying to enter a value that would cause one.

## File Structure
/spreadsheet-web-app │ ├── index.html # The HTML structure of the app ├── app.js # JavaScript file with logic for handling user interactions ├── style.css # CSS file for styling the spreadsheet and UI elements ├── README.md # This README file with project details └── LICENSE # (Optional) A file for the project's license (e.g., MIT)
