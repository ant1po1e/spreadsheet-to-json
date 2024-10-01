# Gulanova Website - Spreadsheet to JSON Converter

A simple, efficient tool to convert Google Spreadsheet data into JSON format.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Prerequisites](#prerequisites)
- [Contributing](#contributing)
- [License](#license)

## Installation

Follow these steps to set up the project locally:

```bash
# Clone this repository
git clone https://github.com/ant1po1e/spreadsheet-to-json

# Navigate to the project directory
cd spreadsheet-to-json
```

## Usage

1. Open the project in [Visual Studio Code](https://code.visualstudio.com).
2. Install the [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) extension for VSCode.
3. Right-click on `index.html` and select "Open with Live Server" to run the application locally.

## Features

### Key Components

1. **Google API Key Input**: 
   - Obtain your API key from the [Google Cloud Console](https://console.cloud.google.com).
   - Enable the Google Sheets API in your Google Cloud project.
   - Create an API Key: Navigate to APIs & Services > Credentials > Create Credentials > API Key.
   - **Security Note**: Keep your API key confidential. This tool runs locally on your machine for your security.

2. **Spreadsheet ID Input**:
   - Locate this in your Google Sheets URL between 'd/' and '/edit'.
   - Example: In `https://docs.google.com/spreadsheets/d/abc123xyz/edit#gid=0`, the ID is `abc123xyz`.

3. **Range Input**:
   - Specify the data range in A1 notation (e.g., 'Sheet1!A1:C10').
   - The first row in your selected range will be used as JSON property names.

4. **JSON Generation**:
   - Click "Generate JSON" to convert your spreadsheet data into JSON format.
   - The resulting JSON will be displayed in the text area below.

5. **Copy Functionality**:
   - Use the "Copy" button to easily copy the generated JSON to your clipboard.

## Prerequisites

- A modern web browser
- A Google account with access to Google Sheets
- A Google Cloud project with the Sheets API enabled

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is open source and available under the [MIT License](LICENSE).