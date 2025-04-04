# Review_scraper_project 

A Python script to scrape product reviews from G2, Capterra, and TrustRadius for a specified company and date range, designed to run in Visual Studio Code (VS Code). The script outputs reviews in a JSON file.

## Objective
Scrape reviews from G2, Capterra, and TrustRadius based on a company name, start date, end date, and source, and save them as JSON. This README guides you through running the script in VS Code.

## Features
- Scrapes reviews from G2, Capterra, and TrustRadius (bonus third source).
- Accepts command-line inputs: company name, start date, end date, and source.
- Outputs a JSON file with review details (title, description, date, rating).
- Handles pagination and date filtering.
- Includes error handling and retry logic for failed requests.

## Prerequisites
- **VS Code**: Download from (https://code.visualstudio.com/).
- **Python 3.6+**: Install from (https://www.python.org/downloads/) and add to PATH.
- **Python Libraries**: `requests`, `beautifulsoup4`.

## Setup in VS Code

### 1. Install VS Code and Python
1. Install VS Code if not already installed.
2. Install Python 3.6+ and verify:
   ```bash
   python --version

   Open Project in VS Code

   Install Python Extension  ->  Search for "Python" (by Microsoft)
   -> Select Python interpreter:
Ctrl+Shift+P > "Python: Select Interpreter" > Choose your Python version.

Install Dependencies
Open the terminal in VS Code
paste this

pip install requests beautifulsoup4


Running the Script in VS Code

Option 1: Run via Terminal 
cd path/to/review_scraper_project

Run the script with arguments: 
Sample Command:     
python review_scraper.py "Company Name" "2023-01-01" "2023-12-31" "TrustRadius" 

python review_scraper.py "Slack" "2023-01-01" "2023-12-31" "capterra"

after run this
Output: A file like Slack_capterra_reviews.json will appear in the Explorer pane.

Option 2: Run with VS Code Run Button
Output appears in the terminal, and the JSON file is saved in the project folder.
