# CoDoc - Code Analysis Tool

CoDoc is a web-based code analysis tool that helps developers understand and improve their code by providing metrics, complexity analysis, and AI-powered insights.

## Features

- Analyze code in multiple languages (Python, JavaScript, Java, C)
- Auto-detect language or manually select
- View code metrics (LOC, functions, complexity)
- Get function-level complexity analysis
- Receive AI-powered insights and refactoring suggestions
- Learn about time and space complexity through educational modules
- Meet the team behind the project

## Project Structure

\`\`\`
codoc/
├── app.py                  # Flask application entry point
├── updated_app.py          # Code analysis backend
├── api_key.env             # Environment variables (API keys)
├── static/                 # Static assets
│   ├── css/                # CSS stylesheets
│   │   ├── main.css        # Main styles
│   │   ├── analyzer.css    # Code analyzer page styles
│   │   ├── modules.css     # Learning modules page styles
│   │   └── about.css       # About page styles
│   └── js/                 # JavaScript files
│       ├── navigation.js   # Navigation and menu functionality
│       ├── samples.js      # Sample code for different languages
│       └── analyzer.js     # Code analysis functionality
└── templates/              # HTML templates
    ├── base.html           # Base template with common elements
    ├── index.html          # Main index page (redirects to analyzer)
    ├── analyzer.html       # Code analyzer page
    ├── modules.html        # Learning modules page
    └── about.html          # About page
\`\`\`

## Installation

1. Clone this repository
2. Install the required dependencies:

\`\`\`bash
pip install flask flask-cors python-dotenv radon prettytable google-generativeai javalang esprima pycparser
\`\`\`

3. Make sure you have a valid Google API key in the `api_key.env` file

## Running the Application

1. Start the Flask server:

\`\`\`bash
python app.py
\`\`\`

2. Open your web browser and navigate to `http://localhost:5000`

## Usage

1. Enter or paste your code in the editor
2. Select the language or use auto-detect
3. Click "Analyze Code"
4. View the results in the analysis panel
5. Optionally, click "Refactor Code" to get AI-powered refactoring suggestions

## Pages

- **Code Analyzer**: The main tool for analyzing and refactoring code
- **Modules**: Educational content about time and space complexity
- **About**: Information about the team and project purpose

## Requirements

- Python 3.7+
- Flask
- Google Gemini API key
