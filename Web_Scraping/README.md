# Web Scraping – Books to Scrape

## 1. Project Overview

This project focuses on extracting book information from the Books to Scrape website using Python Web Scraping techniques.

Website: https://books.toscrape.com/

The website contains 1000 books distributed across 50 pages.

## 2. Libraries Used

- Requests: To send HTTP requests and access web pages.
- BeautifulSoup: To extract information from HTML pages.
- Pandas: To organize and export the collected data.
- Time: To control delays between requests.
- URL Join: To handle book URLs and pagination links.

## 3. Data Extraction

The following information was extracted for each book:

- Book Name
- Category
- Price
- Availability

## 4. Pagination

The website contains multiple pages.

A pagination loop was implemented to navigate through all available pages and extract all book records.

## 5. Data Handling

- Missing information is assigned the value "Unknown".
- Extracted information is stored in a Python list.
- Pandas DataFrame is used to organize the extracted records.

## 6. Output

The extracted data was exported into a CSV file.

Output file: `books_data.csv`

Expected number of records: 1000 books.

## 7. Challenges and Solutions

**Challenge 1: Multiple Pages**

Solution: Used a pagination loop to navigate through all pages.

**Challenge 2: Extracting Book Categories**

Solution: Accessed individual book pages to extract category information.

**Challenge 3: Missing Information**

Solution: Used "Unknown" when information was unavailable.

## 8. Final Result

Successfully implemented a web scraping process to collect book information from all available pages and export the results into a CSV file.
