# IMDb Movie Data Web Scraping Project

## Overview

This project explores the utilization of web scraping techniques in Python to extract IMDb movie data. By leveraging libraries such as requests, BeautifulSoup, and pandas, the workflow involves making HTTP requests, parsing HTML responses, and extracting relevant movie details. The extracted data is then cleaned, organized into a structured format using a Pandas DataFrame, and subjected to analysis and visualization, providing comprehensive insights into the IMDb movie dataset.

## Modules Needed

- `requests`: For making HTTP requests to a specified URL.
- `html5lib`: A pure-python library for parsing HTML.
- `bs4`: BeautifulSoup object for web scraping.
- `pandas`: For data manipulation and organization.

## Workflow

1. **Importing Libraries**: Required libraries such as `requests`, `BeautifulSoup`, `re`, `pandas`, `matplotlib.pyplot`, and `seaborn` are imported.
   
2. **Making a Request**: The `requests.get()` method is used to send an HTTP request to the IMDb website and obtain the response.

3. **Parsing HTML**: The response content is parsed using `BeautifulSoup` to enable easy extraction of desired data from the HTML structure.

4. **Data Extraction**: Various sections of the webpage, such as rankings, titles, descriptions, movie runtimes, genres, ratings, votes, directors, and actors, are scraped using appropriate CSS selectors and stored in separate lists.

5. **Data Cleaning**: The extracted data is cleaned, removing unwanted characters and converting data types where necessary. Regular expressions (`re`) are utilized for data cleaning operations.

6. **Data Frame Creation**: The cleaned data is combined into a Pandas DataFrame, where each column represents a specific attribute of the movies.

7. **Data Analysis and Visualization**: The structure of the DataFrame is examined using `info()` and `head()` methods. Additionally, the data is visualized using libraries such as `matplotlib.pyplot` and `seaborn` to gain insights and present the information effectively.

8. **Saving Data**: The final DataFrame is saved as a CSV file using the `to_csv()` method.
