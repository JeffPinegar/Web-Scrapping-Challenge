<h1>Jeff Pinegar</h1><br>
jeffpinegar1@gmail.com<br>
<br>
<h2>Challenge 12 – Web scraping </h2>
Due: Dec 22, 2023
<br>
<br>
<h2>Overview</h2>
This project demonstrated the ability scrap webpages.  
The coding for this project is located in 5 files. These files are heavily commented, so it is clear what 
transformations are performed. Following is a brief description of these files and the operations performed.
<br><br>
I elected to keep the jupyter notebooks as 3 separate files. This not only simplified my development debugging, but it
is also representative of how these files will be used in the real world. Updates on the sales information and the
manufacturing information do not occur at the same time. Therefore they will be processed separately. I anticipate new 
challenges requiring additional transformations, so keeping the load separate will avoid the loading date before it is 
properly transformed.
<br><br>
<h4>JSP_part_1_mars_news.ipynb</h4>
In the first part we scrapped a news site for news articles.  We were asked to scrape the title and the short description.  In addition I scrapped the data posted since news isn’t news unless you know the date.
<br><br>
<h4>JSP_part_2_mars_weather.ipynb</h4>
In the second part we were asked to scrap mars temperature and pressure observations from a website.  The scrappings were loaded into a pandas data frame.  Scrapping brings everything as text (strings).  Therefore, once we scrapped the data, we needed to transform the data into the appropriate data types (int, datatime and floats).
<br>
Once the data was in a data frame we used that data to answer question and generate summary charts.
<br><br>
<h2>Outputs</h2>
 While working on Part 1 and Part 2 the following files were generated and stored in the subdirectory ‘Outputs’
<br><br>

<h4>nasa_news.json</h4>
Json containing the article title, article short description and publication date.
<br><br>

<h4>Mars_temp_data_raw.csv</h4>
This is the first export of the Mars data.  All the values are strings, and there are duplicate observations at this point
<br><br>

<h4>Mars_temp_data_clean.csv</h4>
This version of the csv file has been cleaned.  The duplicate observations have been dropped and the correct data types have been assigned.
<br><br>

<h4>Mars_temp_data_clean_with_day_no.csv</h4>
To answer the last question we needed a create an new variable that represented the number of days since the first day of observations.  This CSV file contains the original clean data plus this additional column.
<br><br>

<h4>Q3a_Averge_Min_Temp_by_Month.jpg</h4>
Image of the average minimum temperature by month
<br><br>

<h4>Q3b_Averge_Min_Temp_by_Month_sort.jpg </h4>
Image of the average minimum temperature by month warmest to coldest
<br><br>

<h4>Q4_Averge_Pressure_by_Month.jpg </h4>
Image of the average pressuer by month
<br><br>

<h4>Q5_Length_of_Martion_year.jpg</h4>
Image of the temperature by day starting with the first observation.  This chart was use to determine the length of a martion year by looking at the days between peak temperatures.
<br><br>

