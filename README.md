# SQL Injection Detection Tool

This Python-based tool scans web pages for potential SQL injection vulnerabilities by testing forms on the page with a list of common SQL injection payloads. It uses the `requests` library to make HTTP requests and `BeautifulSoup` to parse and extract form elements.

## Features
- Scans a given URL for forms that might be vulnerable to SQL injection.
- Tests each form with a set of predefined SQL injection payloads.
- Identifies potential vulnerabilities based on SQL error messages or unexpected responses.

## Requirements
- Python 3.x
- `requests` library
- `beautifulsoup4` library

Install the required libraries using pip:
pip install requests beautifulsoup4


## Usage
Clone the repository or download the script.
Run the script with Python.
Enter the URL you want to scan for SQL injection vulnerabilities.
The tool will scan all forms on the page and test them using various SQL injection payloads. It will notify you if any potential vulnerabilities are found based on the server's response.

## Example
Enter the URL to scan: http://example.com
Scanning http://example.com for SQL injection vulnerabilities...
Found 2 form(s) on the page.
Testing form 1 (http://example.com/form-action)...
No vulnerabilities detected in this form.
Testing form 2 (http://example.com/another-form)...
Potential vulnerability detected with payload: ' OR 1=1 --

## Payloads Used
'; DROP TABLE users; --
' UNION SELECT null, null, null --
' OR 'a'='a' --
1'or'1'='1'#
' AND 1=1 --
' OR 1=1 --
' OR 1=2 --
' AND 'x'='x' --
Contact For any questions or contributions, feel free to reach out:

Email: abdelrahman.emira311@gmail.com 
LinkedIn: www.linkedin.com/in/abdelrahman-emira-48b187239
