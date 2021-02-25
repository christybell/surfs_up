# Surf's Up with Advanced Data Storage and Retrieval

## Project Overview
While I was on vacation in Hawaii last year, I discovered a new-found passion for surfing. I've been trying to come up with a plan so that I can live in Hawaii forever. I have an idea that I think is fool-proof: a Surf n' Shake shop, serving surf boards and ice cream to locals and tourists alike. I have some savings that I plan to invest but need some real investor backing to get the venture off the ground. So, after putting together a strong business plan, I've reached out to an investor, W. Avy, who is famous for his love of surfing. Our first meeting went very well but he has some major concerns about the weather. Apparently he invested in a similar venture earlier in his career, however he didn't ask for any weather analysis and the shop was quickly rained out of business. So, W. Avy has asked that I run some analytics on a weather dataset he has from the beautiful island of Oahu.

## Resources
- **Data Sources**: SQLite Database `hawaii.sqlite`
- **Software and Tools**: Python, Pandas, SQLAlchemy, Jupyter Notebook & Git Bash 

## Challenge Overview
W. Avy likes my analysis but wants more information about temperature trends before opening the surf shop. Specifically, he wants temperature data for the months of June and December in Oahu, in order to determine if the surf and ice cream shop business is sustainable year-round.

## Challenge Results
### Deliverable 1: Determine the Summary Statistics for June
Using Python, Pandas functions and methods, and SQLAlchemy, I wrote a `for loop` to filter the date column of the Measurements table in the `hawaii.sqlite` database to retrieve all the temperatures for the month of June and append them to a list. Then, I created a DataFrame from the list, generated the summary statistics, and confirmed that they matched the image in the challenge assignment.

<img src="images/Delv 1_sum stats.PNG">

### Deliverable 2: Determine the Summary Statistics for December
Using Python, Pandas functions and methods, and SQLAlchemy, I refactored the `for loop` I wrote for the first deliverable, this time to filter the date column of the Measurements table in the `hawaii.sqlite` database to retrieve all the temperatures for the month of December and append them to a list. Then, I created a DataFrame from the list, generated the summary statistics, and confirmed that they matched the image in the challenge assignment.

<img src="images/Delv 2_sum stats.PNG">

### Three Major Points from the Analysis Deliverables
- The average temperature in June is 74.94 degrees, whereas the average temperature in December is 71.04 degrees. Therefore, the difference between June and December average temperatures is less than 4 degrees.
- The minimum temperature in June is 64 degrees, whereas the minimum temperature in December is 56 degrees. Therefore, the difference between June and December minimum temperatures is 8 degrees.
- The maximum temperature in June is 85 degrees, whereas the maximum temperature in December is 83 degrees. Therefore, the difference between June and December maximum temperatures is 2 degrees.

## Challenge Summary
Based on the summary statistics for June and December temperatures, there is very little difference between average, minimum and maximum temperatures throughout the year. So, based on this analysis, the beautiful island of Oahu seems like a very good place for a surf and ice cream shop.

Sustainable temperatures throughout the year is a great start, but we need to do some additional analysis to find out if the weather is ideal for a surf and ice cream shop. Two additional queries we can perform to gather more weather data:
1. We can perform other queries to find out the average precipitation amounts for the month of June and December, or other months, to see if there are big differences throughout the year.
2. Since finding out the average precipitation amounts won't tell us the whole rainfall story, we should perform other queries to find out how frequently it rains in Oahu, such as how many days per month. 

