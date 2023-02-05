For this story, I began with this [dataset from various sources published on Wikipedia](https://en.wikipedia.org/wiki/List_of_cities_by_sunshine_duration).

From this dataset, I worked on an analysis of the total sunshine hours every year for cities around the world, finding that Nairobi’s sunshine is nearly the average.


![Sunshine analysis](/Users/ivynyayieka/Downloads/sunshine_folder/daylight_datetime_violin_chart.png)




I then merged this dataset with daylight information from [Sunset and Sunrise data](https://www.sunrise-and-sunset.com/en) from (daylight data is different from sunshine dataset mentioned prior because it refers to daylight even when cloudy).

 In order to obtain the relevant daylight data, I created a url pattern from the base dataset. The city was regularly labelled differently from one website to another eg. Benghazi-Bengazi, Bangalore-Bengaluru, Ferke-Ferkessédougou. Therefore, I manually matched them in a separate file. (sunshine_name_conversion.csv)

I merged this file to the name conversion file and then used that to generate urls for the daylight dataset. Here, I scraped for data for the sunrise, sunset and day length for 365 days for the 390 cities. (The code for that is in sunshine_year_tables,ipnyb), Afterwards, I analysed the resulting daylight data. I found that while some places have large differences between their longest and shortest days, Nairobi’s day length is generally the same throughout the year.

![Daylight analysis](/Users/ivynyayieka/Downloads/sunshine_folder/nrb_violin_chart.png)

A further step in this analysis could be an indepth scraping the length of shadows at noon on the shortest day and longest day of the year [on this website:](https://www.suncalc.org/#/-1.2835,36.8238,11/2020.11.23/11:23/1/2). I think it could help to show something I mention in the story, that people in Nairobi reliably use shadow length to tell you what time it is because shadow lengths are consistent