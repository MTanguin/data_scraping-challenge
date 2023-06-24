#### "Extracting Insights from Mars News Articles and Weather Data for Scientific Exploration"

# Background

This project focuses on web scraping and data analysis, aiming to extract information from webpages related to Mars. By utilizing tools such as Splinter, Beautiful Soup, and Pandas, the project involves scraping titles and preview text from Mars news articles, as well as analyzing Mars weather data from a table. The extracted data is then organized, stored, and analyzed to gain insights into Mars' climate and atmospheric conditions.

# Methods

#### Part 1: Scrape Titles and Preview Text from Mars News

In this part, the Mars News website is scraped using automated browsing with Splinter. The page is inspected to identify the specific elements to extract. A Beautiful Soup object is created to parse the HTML and extract the desired text elements. The titles and preview text of the news articles are then scraped and stored in Python data structures, including dictionaries and lists. Optionally, the scraped data can be saved in a JSON file for easier sharing.

#### Part 2: Scrape and Analyze Mars Weather Data

This part involves visiting the Mars Temperature Data Site using automated browsing. Similar to Part 1, the page is inspected to identify the relevant elements to scrape. A Beautiful Soup object is created to extract the data from the HTML table. The scraped data is organized into a Pandas DataFrame, with columns representing different attributes such as terrestrial date, sol, ls, month, min_temp, and pressure. Data types are checked and converted if necessary. The dataset is then analyzed using various Pandas functions to answer questions about the number of months on Mars, Martian days worth of data, coldest and warmest months, lowest and highest atmospheric pressure months, and the length of a Martian year in Earth days. The findings are plotted as bar charts for visualization. Finally, the DataFrame is exported to a CSV file.

# Analysis

The analysis of the Mars weather data reveals that the coldest minimum temperature on Mars is typically observed in the third month, while the eighth month experiences the warmest temperatures. However, it is important to note that the temperatures on Mars are consistently very cold from a human perspective. The atmospheric pressure on Mars is lowest in the sixth month and highest in the ninth month. The Martian atmosphere, with a pressure of 6.518 millibars or 0.095 psi at ground level, is significantly lower compared to Earth's sea level atmospheric pressure of 14.7 psi. It is evident that the Martian atmosphere is not breathable for humans. The analysis also indicates that a Martian year is approximately 675 Earth days, based on the plot of daily minimum temperatures.



Sources: https://courses.bootcampspot.com/courses/2799/assignments/42880?module_item_id=803332

https://mars.nasa.gov/MPF/mpf/realtime/mars2.html#:~:text=At%20ground%20level%20the%20Martian,39%20UTC%20Earth%20receive%20time
