# Mars_HTML

## Part 1- Mars News Scrapping

Beautiful Soup is used on a website with the following url: 'https://static.bc-edx.com/data/web/mars_news/index.html'. All the text elements within this website are extracted and looped through individually to find the "title" and "preview" values for each article. The "title" and "preview" values are stored as a pair in dictionary format. After this objective is completed, the browser is terminated.  


## Part 2- Mars Weather Data Analysis

Beautiful Soup is used once again on another website with this url: 'https://static.bc-edx.com/data/web/mars_facts/temperature.html'. All the data within this website is scrapped and placed into a Pandas DataFrame. The columns for this DataFrame are: id, terrestrial_date, sol, ls, month, min_temp, and pressure. The datatypes for the columns' values are converted into: Object, datetime, integer, integer, integer, float, and float. This DataFrame, which is called 'mars_dataframe', is used to answer five major questions:

1. How many months are on Mars?

In order to answer this question, the DataFrame is grouped by month and then the count of each month in the dataset is found.  


2. How many Mars days of data is contained in this dataset?

To solve this problem, the length of values in the column 'sol' in the 'mars_dataframe' DataFrame is calculated.


3. What are the warmest and coldest months on Mars?

The 'mars_dataframe' dataframe is grouped by month and the average value in the 'min_temp' is calculated. Then, a bar plot is made with all the months on the x-axis and the average temperature on the y-axis. Another bar plot is also made with these same parameters, but it is sorted in ascending order to clearly see which months are the coldest and hottest on Mars. 

4. Which months have the lowest and highest atmospheric pressure?

The dataframe is grouped by month and the average value in the 'pressure' column is calculated per month. This is then sorted in ascending order and plotted as a bar chart with month on the x-axis and average pressure on the y-axis to show which months have the lowest and highest atmospheric pressure on Mars.  


5. How many Earth days exist in a single year on Mars?

The values for the 'min_temp' column in the 'mars_dataframe' dataframe are extracted and plotted in a line graph. The index of this series are according to Terrestrial Dates from first landing on Mars, so it is the x-axis. This plot shows the peaks in minimum temperature throughout the time Curiousity has been on Mars, so comparing peak-from-peak provides the answer on how many Earth days exist in a single year on Mars.  

 
After these answers are attained, this DataFrame is exported and the browser is closed. 


