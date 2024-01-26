This new assignment consists of two technical products. I submited the following deliverables:
- Deliverable 1: Scrape titles and preview text from Mars news articles.
- Deliverable 2: Scrape and analyze Mars weather data, which exists in a table.

  **Part 1: Scrape Titles and Preview Text from Mars News**
  1. Used automated browsing to visit the Mars news (https://static.bc-edx.com/data/web/mars_news/index.html). Inspected the page to identify which elements to scrape.
  2. Created a Beautiful Soup object and used it to extract text elements from the website.
  3. Extracted the titles and preview text of the news articles that I scraped. Stored the scraping results in Python data structures as follows:
     - Stored each title-and-preview pair in a Python dictionary and, gave each dictionary two keys: {title} and {preview}.
     - Stored all the dictionaries in a Python list.
     - Printed the list in my jupyter notebook.
    
  **Part 2: Scrape and Analyze Mars Weather Data**
  1. Used automated browsing to visit the Mars Temperature Data (https://static.bc-edx.com/data/web/mars_facts/temperature.html). Inspected the page to identify which elements to scrape.
  2. Created a Beautiful Soup object and used it to scrape the data in the HTML table.
  3. Assembled the scraped data into a Pandas DataFrame. Made sure that the columns had the same headings as the table on the website. Here’s an explanation of the column headings:
    - id: the identification number of a single transmission from the Curiosity rover
    - terrestrial_date: the date on Earth
    - sol: the number of elapsed sols (Martian days) since Curiosity landed on Mars
    - ls: the solar longitude
    - month: the Martian month
    - min_temp: the minimum temperature, in Celsius, of a single Martian day (sol)
    - pressure: The atmospheric pressure at Curiosity's location
  4. Examined the data types that are currently associated with each column. Converted the data to the appropriate datetime, int, or float data types.
  5. Analyzed the dataset by using Pandas functions to answer the following questions:
     - How many months exist on Mars?
     - How many Martian (and not Earth) days worth of data exist in the scraped dataset?
     - What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:
       - Found the average minimum daily temperature for all of the months.
       - Plotted the results as a bar chart.
     - Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:
       - Found the average daily atmospheric pressure of all the months.
       - Plotted the results as a bar chart.
     - About how many terrestrial (Earth) days exist in a Martian year? To answer this question:
       - Considered how many days elapsed on Earth in the time that Mars circles the Sun once.
       - Visually estimated the result by plotting the daily minimum temperature.
   6. Export the DataFrame to a CSV file.
