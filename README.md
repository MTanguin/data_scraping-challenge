# data_scraping-challenge

Background

This project is about web-scraping and data analysis, and identifying HTML elements on a page, their id and class attributes, and use this knowledge to extract information via both automated browsing with Splinter and HTML parsing with Beautiful Soup and scrape various types of information. These include HTML tables and recurring elements, like multiple news articles on a webpage.
Core skills: collecting data, organizing, and storing data, analyzing data, and then visually communicating insights.


Requirement

This new assignment consists of two technical products. You will submit the following deliverables:
•	Deliverable 1: Scrape titles and preview text from Mars news articles.
•	Deliverable 2: Scrape and analyze Mars weather data, which exists in a table


Methods

Part 1: Scrape Titles and Preview Text from Mars News

Open the Jupyter Notebook in the starter code folder named part_1_mars_news.ipynb. You will work in this code as you follow the steps below to scrape the Mars News website.

1.	Use automated browsing to visit the Mars news site Links to an external site.. Inspect the page to identify which elements to scrape.

2.	Create a Beautiful Soup object and use it to extract text elements from the website.

3.	Extract the titles and preview text of the news articles that you scraped. Store the scraping results in Python data structures as follows:

o	Store each title-and-preview pair in a Python dictionary and, give each dictionary two keys: title and preview. 

o	Store all the dictionaries in a Python list.

o	Print the list in your notebook.

4.	Optionally, store the scraped data in a file (to ease sharing the data with others). To do so, export the scraped data to a JSON file. 


Part 2: Scrape and Analyze Mars Weather Data

Open the Jupyter Notebook in the starter code folder named part_2_mars_weather.ipynb. You will work in this code as you follow the steps below to scrape and analyze Mars weather data.

1.	Use automated browsing to visit the Mars Temperature Data Site Links to an external site.. Inspect the page to identify which elements to scrape. Note that the URL is https://static.bc-edx.com/data/web/mars_facts/temperature.html.

2.	Create a Beautiful Soup object and use it to scrape the data in the HTML table. Note that this can also be achieved by using the Pandas read_html function. However, use Beautiful Soup here to continue sharpening your web scraping skills.

3.	Assemble the scraped data into a Pandas DataFrame. The columns should have the same headings as the table on the website. Here’s an explanation of the column headings:

id: the identification number of a single transmission from the Curiosity rover
terrestrial_date: the date on Earth
sol: the number of elapsed sols (Martian days) since Curiosity landed on Mars
ls: the solar longitude
month: the Martian month
min_temp: the minimum temperature, in Celsius, of a single Martian day (sol)
pressure: The atmospheric pressure at Curiosity's location

4.	Examine the data types that are currently associated with each column. If necessary, cast (or convert) the data to the appropriate datetime, int, or float data types.

5.	Analyze your dataset by using Pandas functions to answer the following questions:
o	How many months exist on Mars?
o	How many Martian (and not Earth) days worth of data exist in the scraped dataset?
o	What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:
	Find the average minimum daily temperature for all of the months.
	Plot the results as a bar chart.
o	Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:
	Find the average daily atmospheric pressure of all the months.
	Plot the results as a bar chart.
o	About how many terrestrial (Earth) days exist in a Martian year? To answer this question:
	Consider how many days elapse on Earth in the time that Mars circles the Sun once.
	Visually estimate the result by plotting the daily minimum temperature.
6.	Export the DataFrame to a CSV file.

Overview and Analysis


On average, the third month has the coldest minimum temperature on Mars, and the eighth month is the warmest. But it is always very cold there in human terms!

Atmospheric pressure is, on average, lowest in the sixth month and highest in the ninth.

At ground level the Martian atmosphere has a pressure of 6.518 millibars or 0.095 psi as compared to the Earth's sea level atmospheric pressure of 14.7 psi.(source:https://mars.nasa.gov/MPF/mpf/realtime/mars2.html#:~:text=At%20ground%20level%20the%20Martian,39%20UTC%20Earth%20receive%20time.) 

Overall, the Martian atmosphere is not breathable.

The distance from peak to peak is roughly 1425-750, or 675 days. A year on Mars appears to be about 675 days from the plot. Internet search confirms that a Mars year is equivalent to 687 earth days.

The temperature and the atmospheric pressure on Mars are just few of the problems that need to be solved before human can live on it.

Source: https://courses.bootcampspot.com/courses/2799/assignments/42880?module_item_id=803332
