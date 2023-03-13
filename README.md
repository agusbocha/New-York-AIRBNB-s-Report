# New-York-AIRBNB-s-Report

#### Project Goal:
The idea of the project is to analize information about NYC Airbnb's obtaining important insights about prices, reviews, difference by neighborhood, difference by their location, among other.

#### Data acquisition:
- NYC Airbnb's information was obtained by a kaggle dataset (https://www.kaggle.com/datasets/dgomonov/new-york-city-airbnb-open-data).
- NYC subway stations geolocation was also obtained by a kaggle dataset (https://www.kaggle.com/datasets/new-york-state/nys-nyc-transit-subway-entrance-and-exit-data)

#### Data Wrangling:
Both datasets were load in python and wrangled using pandas library.

First, I created the price - grouped column and reviews - grouped column from the price and reviews columns respectively. 

Then, I collected information about the 12 most iconic NYC attraction. I created a new column for each attraction with the distance between the AIRBNB and the attraction.
The next step was to work with the subway stations information. I used the BallTree algorithm from the sklearn library which uses the haversine method to calculate the distances using geolocation. 

The final step was to drop the rows that contained outliers in the price column because they were making noise to the report.

#### Power Bi
Next, I loaded the final dataset in power bi and add some other columns and created some new tables that helped me in developing the report.

#### Insights
