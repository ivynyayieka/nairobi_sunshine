
<h4>How I collected the news headlines</h4>
For the satirical gif of a collage of news headlines, I googled "Kenya/ Nairobi ranked highest/ worst in..."


<h4>How I analysed the initial dataset on hours of sunshine</h4>
For this story, I began with this [dataset from various sources published on Wikipedia](https://en.wikipedia.org/wiki/List_of_cities_by_sunshine_duration)  published on Wikipedia.

From this dataset, I worked on an analysis of the total sunshine hours every year for cities around the world, finding that Nairobi’s sunshine is nearly the average.

<h4>How I analysed the  duration of daylight year round for different cities</h4>
I merged the sunshine dataset with daylight information from [Sunset and Sunrise](https://www.sunrise-and-sunset.com/en) data. Daylight data is different from sunshine dataset mentioned prior because it refers to daylight even when cloudy.

 In order to obtain the relevant daylight data, I created a url pattern from the base dataset. The city was regularly labelled differently from one website to another eg. Benghazi-Bengazi, Bangalore-Bengaluru, Ferke-Ferkessédougou. Therefore, I manually matched them in a separate file. (sunshine_name_conversion.csv)

I merged this file to the growing dataset and then used the new names to generate urls for the daylight dataset. Here, I scraped for data for the sunrise, sunset and day length for 365 days for more than 300 cities. (See sunshine_year_tables.ipnyb for the code), Afterwards, I analysed the resulting daylight data. I found that while some places have large differences between their longest and shortest days, Nairobi’s day length is generally the same throughout the year.

<h4>How I analysed temperature disparity year round</h4>
For this, I used [temperature data](https://en.wikipedia.org/wiki/List_of_cities_by_average_temperature) on different cities published on Wikipedia. For ease of legibility, I selected only cities starting with N to show disparity in monthly average temperature year round. 

<h4>How I analysed shadow length disparity year round</h4>

To analyse shadow  length disparity, I used data from [Suncalc](https://www.suncalc.org/#/40.4106,-3.4997,3/2020.11.23/11:23/1/2). For the cities starting with N I had sampled in order to make visualisation legible, I put together a column for the time in UTC at noon in each city. Then I used Suncalc to find the length of a one metre shadow at noon at each city.

With more time, a further step in this analysis could be an indepth scraping of the length of shadows at noon on the shortest day and longest day of the year [on Suncalc](https://www.suncalc.org/#/-1.2835,36.8238,11/2020.11.23/11:23/1/2). I think it could help to be thorough about the analysis of the sampled cities. I think moving the scale of time on the website via a scraper could be challenging but a worthwhile endeavour to prove the hypothesis.

I have saved [some csv files](https://drive.google.com/drive/folders/1vHdm6bCcIEM7TdyfS7OysJ_hxcskXtVW?usp=sharing) that could not be uploaded here. 

Tech: #Python, #R, #Datawrapper, #Canva, #HTML, #CSS
