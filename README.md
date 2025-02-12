# UFO-Reporting-Scrape-Analysis

# Scraping
## Webpage Scraped
http://www.nuforc.org/webreports/ndxevent.html

## Scraping Procedure
In this project, Selenium was used to scrape the data from a various number of webpages.

The webpage shown above contained a list of indivudal links, pointing to other webpages that contained html tables filled with UFO reports. My script went through every link one-by-one, scraped every html table cell, and grouped them in their proper rows. This scraping script took about 4 hours to complete and scraped about 100,000 total reports.

Each row contained the columns:
- Date / Time
- City
- State
- Shape
- Duration
- Summary
- Posted

## Chrome Webdriver
https://chromedriver.chromium.org/downloads

# Data Cleaning

The cleaning process of the project consisted of
- Seperating the 'Date / Time' column into its very own columns
- Reformatting the 'Date' and 'Time' columns
- Clearing rows with unusual entries (e.g. Dates with year of 2070)
- Clearing all rows with any NaN present
- Dropping the 'Posted' column
- Regrouping values with different capitalizations (e.g. 'lights' and 'Lights')

# Analysis

# The year with the most amount of sightings was 2015

![years](https://user-images.githubusercontent.com/66498197/147865870-9ef77dbb-6039-4cc0-b66d-045244b9825d.png)

# The most occurred sighting by city was Pheonix with 566 sightings, about 0.65 % of the whole dataset

![city](https://user-images.githubusercontent.com/66498197/147865880-446857b0-af2d-46b1-bc58-827911250d23.png)

# The most occurred sighting by state was California with 10938 sightings, about 12.68 % of the whole dataset

![states](https://user-images.githubusercontent.com/66498197/147865873-80e59a26-350d-4808-9c0d-7607a49d092a.png)

# The most common thing seen during UFO encounters was simply light, with 18916 reportings

![shapes](https://user-images.githubusercontent.com/66498197/147865874-fb04fb01-89d5-4516-bfa2-16d184faffa4.png)

# Sightings were widley reported during military times 19-23 or 7:00PM to 11:00PM

![hours](https://user-images.githubusercontent.com/66498197/147865878-ae0b51d7-d5f7-4bba-97af-17c80d8c8405.png)

# Sightings were extremely common on the days of the 1st and the 15th, regardless of the month
# This two outliers are extremely strange

![days](https://user-images.githubusercontent.com/66498197/147865879-9518d604-c3d7-421e-bc20-c36d427565c4.png)

# Sightings were more slightly more common during the months of June through November

![months2](https://user-images.githubusercontent.com/66498197/147865876-9a37b6ed-3d5c-4f44-b0f9-f5fcece62702.png)
![months](https://user-images.githubusercontent.com/66498197/147865877-1e718412-ea02-429f-89f6-de0e7ced8ff4.png)

# Wordclouds

## Summary Wordcloud
![wordcloud](https://user-images.githubusercontent.com/66498197/147865871-43efe137-de35-412e-adc0-238a3dddf8dd.png)
## Duration Wordcloud
![wordcloud2](https://user-images.githubusercontent.com/66498197/147866188-e9b72f6f-ee0f-4388-9c0f-e58a457c11f1.png)
