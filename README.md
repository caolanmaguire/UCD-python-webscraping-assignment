# Dublin Rental Market Analysis

COMP41680 Assignment 1 - Spring 2025/26

![DESCRIPTION IMAGE](https://github.com/caolanmaguire/UCD-python-webscraping-assignment/blob/main/GITHUB%20PYTHON%20PROJECT%20IMAGE.png)

## What This Project Does

This project scrapes dummy data that represents rental listings from Dublin and analyses the data to understand pricing trends and market patterns across 2025.


## Project Files

- `Task1_Data_Collection.ipynb` - Scrapes the rental data
- `Task2_Analysis.ipynb` - Analyzes and visualizes the data
- `output/` - Contains scraped data organized by quarter (Q1-Q4)

## How It Works

### Data Collection
I scraped rental listings from http://mlg.ucd.ie/modules/python/sources/rental/ using BeautifulSoup. The script goes through each quarter and each page, extracting property details like price, location, bedrooms, bathrooms, parking, and garden availability.

Each listing gets saved as a JSON file in the output directory, organized by quarter.

### Data Analysis (Work in progress
The analysis notebook (Task 2) loads all the JSON files and calculates:
- Average rent per quarter
- Average rent per month
- Price trends by number of bedrooms
- Property type distribution
- Amenity availability

## Technologies

- Python 3
- BeautifulSoup4 for web scraping (library)
- Requests for HTTP (library)
- Matplotlib for graphs (library)
- JSON for data storage (I'd used this previously and find it really standard and reusable way to save data)

## Running the Code

Install dependencies:
```bash
pip install beautifulsoup4 requests matplotlib
```

Run Task 1 to collect data, then Task 2 to analyze it.

## Main Findings

The data shows rental price trends across different quarters, property sizes, and locations in Dublin. Key patterns include seasonal variations and pricing differences between property types.

## Author

Caolan Maguire
UCD COMP41680 Python for Data Science Module

## Data Source

http://mlg.ucd.ie/modules/python/sources
