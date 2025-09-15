# Book-Price-Scraper
## Project Overview
### Brief Summary of the Project
This project is a Python-based web scraper that extracts book titles and their prices from the website Books to Scrape. Since the prices on the site are listed in GBP (£), the script integrates with an exchange rate API to convert the prices into KES (Kenyan Shilling). The data is then saved into a structured JSON file, storing both the original GBP price and the converted KES price for future use.
### Goal
The main goal of this project is to:
1. Obtain the titles and prices of at least 10 books.
2. Convert book prices from foreign currency (GBP) into a local currency (KES) for easier analysis.
3. Store the results in a JSON file.

## Features
- Scrapes book titles and prices from Books to Scrape.
- Fetches real-time GBP to KES conversion rates using an API.
- Converts each book’s price from GBP to KES.
- Saves the results into a JSON file with both currencies recorded.
## How it Works
1. The script uses requests to fetch HTML pages from Books to Scrape.
2. BeautifulSoup parses the HTML and extracts the book titles and prices.
3. The raw GBP prices are cleaned and converted into floats.
4. The script calls an exchange rate API to get the latest GBP to KES conversion rate.
5. Each book’s price in GBP is multiplied by this rate to get its KES value.

## Requirements
1. Python 3.13.7
2. BeautifulSoup
3. Lxml
4. Json
5. Regex
6. Requests

## Usage
1. Clone or download the project files.
2. Run the script in terminal
3. The script will scrape book data, convert the prices, and save them into books.json.
4. Open the books.json file to view the results.

## Project Structure
1. Scraping Logic: Uses BeautifulSoup’s CSS selectors to target book titles and prices.
2. Price Cleaning: Removes the "£" symbol and converts string values into floats.
3. Currency Conversion: Uses an exchange rate API with a base currency GBP and target KES.
4. Data Storage: Exports results in JSON for portability and reusability.

## Technical Details


## Results
- Successfully scrapes multiple pages of book listings.
- Provides structured JSON data with both GBP and KES values.

## Contact
For questions or collaboration, contact cabralowiro@gmail.com or open an issue on the repo

## References
1. Python Documentation
2. W3 Schools
3. Geek for geeks
4. Exchange Rate Api
5. Books to scrape

## Licence
- MIT License Copyright (c) 2025 (Chege Cabral)
- - [![GitHub license](https://img.shields.io/github/license/Naereen/StrapDown.js.svg)](https://github.com/Naereen/StrapDown.js/blob/master/LICENSE)

