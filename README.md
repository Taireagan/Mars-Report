# Mars Report

## Background
You have been assigned a project to develop a comprehensive report on Mars, which involves scraping and analyzing data from various sources. The project consists of two main deliverables:

**Deliverable 1:** _Mars News Scraping_

 Extracting titles and preview texts from Mars-related news articles.

**Deliverable 2:** _Mars Weather Data Analysis_

 Scraping and analyzing weather data from a table, focusing on key meteorological metrics.
 
To achieve these objectives, you will employ HTML parsing techniques using BeautifulSoup and automate browsing activities with Splinter. This process involves identifying and targeting specific HTML elements, such as tags, IDs, and class attributes, to accurately extract the required data. Additionally, you will handle more complex scraping tasks, including retrieving data from HTML tables and recurring web elements like multiple news articles.

The analysis conducted in this report will showcase your ability to:

- Collect and extract data from web sources.
- Organize and store data efficiently.
- Perform detailed data analysis.
- Visually communicate insights derived from the data.
  
This project not only demonstrates technical proficiency in web scraping and data analysis but also the capability to transform raw data into meaningful insights through structured reporting.

---

## Deliverable 1:
### Scrape Titles and Preview Text from Mars News
In this task, you will work within the Jupyter Notebook titled **part_1_mars_news.ipynb** to scrape data from the [Mars News website](https://static.bc-edx.com/data/web/mars_news/index.html). 
The following steps outline the process:

### Step 1.  
**Automated Browsing:**  Begin by using automated browsing techniques to visit the [Mars News website](https://static.bc-edx.com/data/web/mars_news/index.html). Carefully inspect the webpage to identify the specific HTML elements that contain the data you want to scrape.

### Step 2:
**Create a Beautiful Soup Object:**  Once the page elements are identified, create a Beautiful Soup object to parse the HTML content. This object will be instrumental in extracting the desired text elements from the website.

### Step 3:
**Data Extraction:**  Extract the titles and preview text of the news articles from the webpage. This involves targeting the appropriate tags and classes to pull the correct information.

### Step 4:
**Data Storage:**  Store each title-and-preview pair in a Python dictionary, ensuring that each dictionary has two keys: title and preview.
Collect all the dictionaries in a Python list for easy management and further processing.
Output: Print the list of dictionaries in your notebook to verify the successful extraction and storage of the data.
Optional Export: To facilitate sharing, you can optionally export the scraped data to a JSON file. This step is not mandatory, but it can be useful for data portability.

## Deliverable 2:
### Scrape and Analyze Mars Weather Data  
For this section, you will Open the Jupyter Notebook in the starter code folder named **part_2_mars_weather.ipynb**. You will work in this code to scrape and analyze Mars weather data.

### Step 1:
**Visit the Website:**  Use automated browsing to visit the Mars [Temperature Data Site](https://static.bc-edx.com/data/web/mars_facts/temperature.html). Inspect the page to identify which elements to scrape.

### Step 2:
**Scrape the Table:**  Create a Beautiful Soup object and use it to scrape the data in the HTML table.

### Step 3:
**Store the Data:**  Assemble the scraped data into a Pandas DataFrame. The columns should have the same headings as the table on the website.
Here’s an explanation of the column headings:
- **id:** the identification number of a single transmission from the Curiosity rover
- **terrestrial_date:** the date on Earth
- **sol:** the number of elapsed sols (Martian days) since Curiosity landed on Mars
- **ls:** the solar longitude
- **month:** the Martian month
- **min_temp:** the minimum temperature, in Celsius, of a single Martian day (sol)
- **pressure:** The atmospheric pressure at Curiosity's location

  ![mars_df_table](https://github.com/Taireagan/Mars-Report/blob/main/Saved%20Graphs/mars_df_table.png)

### Step 4:
**Prepare Data for Analysis:**  Examine the data types that are currently associated with each column. If necessary, cast (or convert) the data to the appropriate **datetime**, **int**, or **float** data types.

### Step 5:
**Analyze the Data:**  Analyze your dataset by using Pandas functions to answer the following questions:

**1.**  How many months exist on Mars?
    
#### &#8594; 12 Months

**2.**  How many Martian (and not Earth) days worth of data exist in the scraped dataset?

#### &#8594; 1,867 Martian Days

**3.** What are the coldest and the warmest months on Mars (at the location of Curiosity)? 

![avg_temp_by_month](https://github.com/Taireagan/Mars-Report/blob/main/Saved%20Graphs/avg_temp_by_month.png)

**4.** Which months have the lowest and the highest atmospheric pressure on Mars?

![avg_pressure_by_month](https://github.com/Taireagan/Mars-Report/blob/main/Saved%20Graphs/avg_pressure_by_month.png)

**5.** About how many terrestrial (Earth) days exist in a Martian year?

![terrestrial_days_table](https://github.com/Taireagan/Mars-Report/blob/main/Saved%20Graphs/terrestrial_days_table.png)

![earth_days_graph](https://github.com/Taireagan/Mars-Report/blob/main/Saved%20Graphs/earth_days_graph.png)


---

## Conclusion
On Mars, the coldest average minimum temperature occurs in the third month, while the warmest month is the eighth. However, it's important to note that even the warmest temperatures on Mars are extremely cold by human standards. Regarding atmospheric pressure, it is at its lowest in the sixth month and peaks in the ninth. The time span between these pressure peaks is approximately 675 days. This analysis suggests that a Martian year is roughly 675 days long, which aligns closely with the fact that a Mars year is known to be about 687 Earth days, as confirmed by additional research


[- BACK TO TOP -](#mars-report)
