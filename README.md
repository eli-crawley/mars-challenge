# Mars Temperature Data Scraper and Analyzer

This project involves scraping news articles and temperature data from Mars (or a similar dataset) and performing basic data analysis. The articles and preview texts are scrapped and exported to json. The temperature data is extracted from, and the data is then processed to visualize temperature trends over time and perform calculations like the minimum temperature per month. Finally, the data is saved to a CSV file for further use.

## Features

- Scrapes news articles from HTML.
- Creates a dictionary list of titles and preview text.
- Exports the articles to json.
- Scrapes temperature data from HTML.
- Converts and processes the scraped data using Pandas.
- Visualizes the temperature trends over time using a plot.
- Exports the processed data to a CSV file for further analysis.

## Required Libraries
- beautifulsoup4: To parse HTML and extract data.
- pandas: For data processing and analysis.
- matplotlib: For plotting the data.

## Usage
### 1. Scraping Data
The fisrt script, part_1_mars_news.ipynb, will scrape news article titles and previews and convert it to a json file. The second script, part_2_mars_weather.ipynb, will scrape temperature and pressure data from an HTML page and convert it into a pandas DataFrame.

### 2. Data Processing
The second script processes the weather data by:
* Converting the date column to datatime format
* Converting the sol column to integer format
* Converting the ls column to integer format
* Converting the month column to integer format
* Converting the min_temp column to float format
* Converting the pressure column to float format

### 3. Visulize Data
The script calculates the average min_temp and pressure by month and plots these values overr time and in ascending order to find the months with the lowest and highest values.

### 4. Analysis
This analysis found the following:
* The third Martian month has the lowest temperatures, averaging -83.31.
* The eighth month has the warmest temperatures, averaging -68.38.
* The sixth month has the lowest pressure, averaging 745.05.
* The ninth month has the highest pressure, averaging 913.31. 
* The temperature cycles over a Martian year, of approximately 700 terrestrial days.

## References
The Mars News is operated by edX Boot Camps LLC for educational purposes only. The news article titles, summaries, dates, and images were scraped from NASA's Mars News website, https://science.nasa.gov/mars, in November 2022. Images are used according to the JPL Image Use Policy, courtesy NASA/JPL-Caltech.