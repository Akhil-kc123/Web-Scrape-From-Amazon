# Web-Scrape-From-Amazon
This project is a web scraper for extracting product data from Amazon using Selenium and Microsoft Edge WebDriver. It automates search queries, navigates multiple pages, and collects key details such as product descriptions, prices, ratings, review counts, and URLs. 

# Amazon Web Scraper

## Overview
This project is an automated web scraper for extracting product data from Amazon. It uses Selenium with Microsoft Edge WebDriver to navigate Amazon search result pages, collect product details, and store them in a CSV file for analysis.

## Features
- Scrapes product listings from Amazon based on a specified search term.
- Extracts key product details, including:
  - **Description**
  - **Price**
  - **Rating**
  - **Review Count**
  - **Product URL**
- Supports pagination, collecting data from multiple search result pages (up to 20 pages).
- Saves extracted data into a structured CSV file.
- Implements randomized sleep intervals to mimic human behavior and reduce the risk of detection.
- Runs headless using Microsoft Edge WebDriver for efficiency.

## Requirements
- Python 3.x
- Selenium
- Microsoft Edge WebDriver

## Installation
1. Install the required dependencies:
   ```bash
   pip install selenium
   ```
2. Download and install Microsoft Edge WebDriver compatible with your Edge browser version.
3. Add WebDriver to your system's PATH or specify its location in the script.

## Usage
Run the scraper by specifying a search term:
```python
python scraper.py
```
The script will scrape Amazon for the given search term (default: 'dell laptop') and save the extracted data to a CSV file with a timestamped filename.

## Notes
- Due to Amazon's anti-scraping measures, consider implementing proxy rotation or using Amazon's API for large-scale data extraction.
- The script currently supports the US Amazon domain (`amazon.com`). Modify URLs if targeting other regions.

## License
This project is intended for educational and research purposes only. Use responsibly and comply with Amazon's terms of service.

