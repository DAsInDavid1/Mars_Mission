# Mars_Mission
Scrapping from different sources to find updated news and weather on Mars using Splinter, BeautifulSoup, Pandas, and Matplotlib

![My Image](https://github.com/DAsInDavid1/Mars_Mission/blob/main/Images/Mars.jpg)


## Mars News
I scrapped https://redplanetscience.com/ for the Mars news articels. First I extracted the title and preview text from the news articles using a for loop, and getting them from their respective classes then changing them to text. Then in a dictionary of {title:"title", preview:"preview text"} I appended a empty dictionary and would input each new title and preview, then the loop woulld start again. I then stored all the dictionaries in a python list and exported it as a JSON file for future use.

<img src= "https://github.com/DAsInDavid1/Mars_Mission/blob/main/Images/For-Loop.png" width=50% height=50%> 

## Mars Weather
I scrapped https://data-class-mars-challenge.s3.amazonaws.com/Mars/index.html for the weather data of Mars. First I needed to extract all the rows of data from the table. Then using a for loop I extracted the data and changed it to a text format so that it would fit into a empty list. I made that list into a DataFrame and added headers and checked for the data types of each column. The date columns, along with the columns filled with numbmrs needed to be updated to be the correct data types. I then started the analysis of the data by checking the number of months, how many days their are in a year for mars, and the avg low temp by the month. After setting my variables, I made bar graphs to display the avg min temp by month (also in ascending order) and avg atmospheric pressure by month in ascending order. Then I wanted to have a visual line graph of the number of days on Mars, so I used the min temp of each day to be my y-axis and days be my x-axis. Then finally I exported my DataFrame as a csv file for future use.

| Avg Temp Per Month  | Coldest & Hottest Months | Avg Pressure Per Month | Amount of Days in Year.
| ------------- | ------------- | ------------- | ------------- | 
| <img src= "https://github.com/DAsInDavid1/Mars_Mission/blob/main/Images/Avg_Temp_Per_Month.png" width=100% height=100%>   | <img src= "https://github.com/DAsInDavid1/Mars_Mission/blob/main/Images/Coldest_%26_Hottest_Months.png" width=100% height=100%>   |<img src= "https://github.com/DAsInDavid1/Mars_Mission/blob/main/Images/Avg_Pressure_Per_Month.png" width=100% height=100%> |<img src="https://github.com/DAsInDavid1/Mars_Mission/blob/main/Images/Amount_of_Days_in_Year.png" width=100% height=100%>  |


