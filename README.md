# Dice Job Application Automation

This Python script automates the process of searching and applying for jobs on Dice.com. It uses Selenium WebDriver to navigate through job listings, extract job details, and submit applications.

## Features

- Automated job search based on keywords
- Job details extraction (title, company, location, skills, etc.)
- Automatic application submission
- CSV export of job details and application status
- Handles authorization questions
- Feedback form dismissal

## Prerequisites

- Python 3.7 or higher
- Chrome browser installed
- Dice.com account credentials

## Installation

1. Clone this repository
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Configuration

Before running the script, update the following variables in `apply_jobs.py`:

```python
USER_EMAIL = "your_email@example.com"
USER_PASSWORD = "your_password"
SEARCH_KEYWORDS = "Your Job Keywords"
```

## Usage

1. Run the script:
   ```bash
   python apply_jobs.py
   ```

2. The script will:
   - Open Chrome browser
   - Navigate to Dice.com
   - Search for jobs based on keywords
   - Extract job details
   - Apply to jobs
   - Save results to `job_details.csv`

## Output

The script generates a CSV file (`job_details.csv`) containing:
- Job ID
- Job Title
- Company
- Location
- Posted/Updated date
- Work Mode
- Pay
- Employment Type
- Application Status
- Scraped On timestamp
- Job Description
- Required Skills

## Notes

- The script includes error handling and retry mechanisms
- It automatically dismisses feedback forms
- It handles authorization questions during application
- Make sure to use your own Dice.com credentials
- The script includes appropriate delays to prevent rate limiting

## Disclaimer

This script is for educational purposes only. Please use responsibly and in accordance with Dice.com's terms of service. Automated job applications should be used ethically and with consideration for the hiring process. 