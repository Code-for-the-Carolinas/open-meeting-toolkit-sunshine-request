This is a collection of files for scraping the websites of counties, cities, and so forth for their listings of open meetings.  The data is meant to populate [this](https://docs.google.com/spreadsheets/d/1MOgzArardJB3TeZAEys9UewUqZUG7jgI08GbSdMNOcc/edit?usp=sharing) spreadsheet.

The scrapers belong to two groups:
- The Python scrapers.  These are built to scrape specific websites of individual counties.  There is no standardization of counties' website designs, so any scrapers have to be customized significantly.  However, they may be useful as references when trying to make scrapers for other counties.  These scrapers use the [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/#) library for processing and extracting information from the websites' HTML, outputting the results as a CSV file that can be intergrated into the meetings list.

- The C# code in the "ReusableXpathScraper" folder.  This code is intended to act as a more general, end-to-end scraper, being able to handle both scraping from multiple county websites and exporting the results to JSON for integration into the meetings list.
