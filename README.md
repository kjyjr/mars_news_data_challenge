# mars_news_data_challenge

This challenge assignment was a web-scraping and data analysis project, applying the skill of identifying HTML elements on a page, including their id and class attributes, and then extracting information via both automated browsing with Splinter and HTML parsing with Beautiful Soup.

The assignment consisted of two technical products to be delivered:

Deliverable 1: Scrape titles and preview text from Mars news articles.

Deliverable 2: Scrape and analyze Mars weather data, which exists in a table.

Part 1: Scrape Titles and Preview Text from Mars News

A Jupyter Notebook was used to scrape the Mars News website. Automated browsing was employed to visit the Mars news site links to an external site, and then the webpage was inspected to identify which elements to scrape. A Beautiful Soup object was created and used to extract text elements, including titles, from the website. Text of news articles was scraped and previewed, then stored in Python data structures as follows:
  each title-and-preview pair was stored in a Python dictionary, and each dictionary given two keys: title and preview
  all the dictionaries were stored in a Python list
[In addition, the scraped data was stored in a file and exported to a JSON file.]

Part 2: Scrape and Analyze Mars Weather Data

Another Jupyter notebook was used to scrape and analyze Mars weather data.

Automated browsing was again employed to visit the Mars Temperature Data site links to an external site, and the webpage inspected to identify which elements to scrape.

A Beautiful Soup object was created and used to scrape the data in the HTML table, and that data subsequently was assembled into a Pandas DataFrame with its columns bearing the same headings as the table on the website.

Data types associated with each column were examined and, as necessary, cast or converted to the appropriate datetime, int, or float data types.

The dataset was then analyzed by using Pandas functions to answer the following questions:

How many months exist on Mars?
How many Martian (and not Earth) days' worth of data exists in the scraped dataset?
What are the coldest and the warmest months on Mars (at the location of Curiosity)? (To answer this question, the average minimum daily temperature for all of the months was found.)

Data found in answering those questions was then plotted as a bar chart.

An additional question answered was, "Which months have the lowest and the highest atmospheric pressure on Mars?" To answer that question, the average daily atmospheric pressure of all the months was found, and those results also plotted as a bar chart.

A final question about how many terrestrial (Earth) days exist in a Martian year was answered by considering how many days elapse on Earth in the time that Mars circles the Sun once, then visually estimating the result by plotting the daily minimum temperature. The associated DataFrame was then exported to a CSV file.
