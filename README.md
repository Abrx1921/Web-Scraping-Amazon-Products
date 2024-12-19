# Web-Scraping-Amazon-Products

**Author: Abraham Saenz Sigala**

**Date: December 18, 2024**

:floppy_disk: File: [Python Jupyter Notebook](Webscraping_Scripts_Full.ipynb)

## :dart: Overview

This project involved creating a dataset of laptops sourced from Amazon's listings via web scraping. The goal was to help identify the best laptop for my cousin by comparing models similar to a specific one she liked, while exploring other options within her price range for better value or features.

## :flashlight: Dataset Details

The final dataset contains:

Rows: 33 (representing different laptops)
Columns: 9 (capturing various laptop attributes)

Columns:

- Title: The name/model of the laptop.
- Price: The price of the laptop (in USD or other available currency).
- Rating: The average customer rating.
- Touchscreen: Indicates whether the laptop has a touchscreen (Yes/No).
- Color: The primary color of the laptop.
- Ram: The RAM cinstalled (e.g., 8GB, 16GB).
- GPU: The graphics processing unit.
- CPU: The central processing unit.
- Link: The URL to the product listing on Amazon.

## :microscope: Purpose

The dataset was created to:

- Compare laptops with similar specifications to a preferred model.
- Identify options within a specific price range that offer better value or features.
- This dataset will serve as a foundation for future webscraping.

## :pencil: Data Source

All data was sourced directly from Amazon's listings using custom web-scraping scripts.

[Base Amazon URL](https://www.numbeo.com/premium/commercial-license](https://www.amazon.com/s?k=gaming+laptop&rh=n%3A21512780011%2Cp_36%3A59000-81000%2Cp_n_size_browse-bin%3A2423841011&dc&crid=2DJRTPGBY27LI&qid=1733934855&rnid=2242797011&sprefix=gamin%2Caps%2C416&ref=sr_pg_1
)

## :bulb: Methodology

:globe_with_meridians: Web Scraping:

- Data was collected using Python's BeautifulSoup, requests, pandas, and time libraries.

- Base URL (Search Results Page) was scrapped and passed through the script to extract all the links excluding sponsored products. A total of 5 pages worth of amazon laptops filtered for 15.6' and $600-$800 price range were scrapped. Links were saved into a file called: amazon_links_nosponsors.txt.

- We then began webscraping every individual product link for releveant specifications that could be used.

- Our final .csv file 'final_laptop_data' contained all the data we scraped and could be used for analysis to find a suitable laptop. 

:soap: Data Cleaning:

Implemented data cleaning techniques as we webscrapped and after to handle inconsistencies.
(For More information Refer to: Webscraping_Scripts_Full.ipynb)

:construction: Limitations:

- Some listings may have missing or inconsistent values.
- Manual cleaning may be required to address these issues during analysis.
- The dataset includes only laptops that we filtered before scraping, not an exhaustive list of all laptops on Amazon.
- Prices on Amazon can change frequently, so the dataset reflects the prices at the time of scraping. December 2024

:package: Scripts:

The web-scraping scripts used for this project are included in the repository. These scripts can be modified to:

- Scrape additional product categories or attributes.
- Refresh the dataset with updated listings and prices.
- Implement them in future web scraping projects

:green_circle: Access:

- Download the 'Webscraping Scripts and Files.zip' folder from this repository.
