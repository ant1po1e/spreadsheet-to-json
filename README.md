# Spreadsheet to JSON Converter

A versatile tool to convert Google Spreadsheet data into JSON format, available in both basic and advanced versions.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
  - [Basic Version](#basic-version)
  - [Advanced Version](#advanced-version)
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
3. Right-click on `index.html` (for basic version) or `advanced.html` (for advanced version) and select "Open with Live Server" to run the application locally.

## Features

### Basic Version

#### Key Components

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

#### How to Use (Basic Version)

1. Enter your Google API Key.
2. Input the Spreadsheet ID.
3. Specify the Range you want to convert.
4. Click "Generate JSON".
5. The generated JSON will appear in the text area.
6. Use the "Copy" button to copy the JSON.

### Advanced Version

#### Key Components

1. **Google API Key Input**: 
   - Same as in the basic version.

2. **Spreadsheet ID Input**:
   - Same as in the basic version.

3. **Custom Variables Input**:
   - Enter comma-separated variable names that will be used as keys in your JSON output.
   - Example: "userId, username, password"

4. **Formula Input**:
   - Specify multiple ranges in A1 notation, separated by commas.
   - Each range corresponds to a variable in the Custom Variables input.
   - Example: "F1:F3, H1:H3" (This will fetch data from cells F1 to F3 for the first variable, and H1 to H3 for the second variable)

5. **JSON Generation**:
   - Click "Generate JSON" to convert your spreadsheet data into a customized JSON format.
   - The resulting JSON will use the variable names you specified and contain data from the corresponding ranges.

6. **Copy Functionality**:
   - Use the "Copy JSON" button to easily copy the generated JSON to your clipboard.

#### How to Use (Advanced Version)

1. Enter your Google API Key.
2. Input the Spreadsheet ID.
3. In the "Custom Variables" field, enter the names you want to use for your JSON keys, separated by commas.
4. In the "Formula" field, enter the ranges that correspond to each variable, also separated by commas.
5. Click the "Generate JSON" button.
6. The tool will fetch data from the specified ranges and generate a JSON object using your custom variable names.
7. You can then copy the generated JSON using the "Copy JSON" button.

Example:
- Custom Variables: "id, name, email"
- Formula: "A2:A10, B2:B10, C2:C10"

This will create a JSON array where each object has "id", "name", and "email" keys, with values taken from columns A, B, and C respectively.

## Prerequisites

- A modern web browser
- A Google account with access to Google Sheets
- A Google Cloud project with the Sheets API enabled

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is open source and available under the [MIT License](LICENSE).