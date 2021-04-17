# Berlin Venues Project

## 1. Introduction 
### 1.1 Background
Berlin is the largest city in Germany and becoming more popular day by day. Berlin has more than 3.6 million population and 55 percent of the population is younger than 45 years of age, the average age was 42.7. [2] So we can say that Berlin is a young city.
Berlin has 12 boroughs and all of them have some characteristic places. Some of them are becoming more popular than others because of these characteristic places. [1] As we can see 80000 jobs were created by start- ups in Berlin in 2020. (Figure 1) Also, we can see that almost 35% of all German fintech start-ups locate in Berlin. (Figure 2)
Berlin is a living city and has so many different places like shopping centers, restaurants, coffee shops, offices, etc. All of these are some reasons for attracting people including expats and newbie startups.

### 1.2 Business Problem
As I mentioned, there are a lot of demands for living in Berlin. It has so many places to attract young people, job seekers, startups.
If you are looking for a place to set up your office, popularity is not enough to decide and you need to explore the real-world data. We always hear some complaints from people about the location of the office, or even in reviews on sites like Glassdoor, people consider the location of offices a minus or plus. Sometimes because of the distance or lack of transportation, they even quit their job. So this particular decision, with other plus features of your small company, of course, might attract more people to work with.
In this project, we will be answering the below questions:
1 - Which neighborhoods have more social places like restaurants, Coffee shops, and bars?
2 - In which neighborhoods the offices/workplaces are more common?
3 - Which neighborhoods have more common transportation centers?
4 - Which places are more attractive for people who are working in offices?
By answering these questions and combining them, we will be finding our final question:
Where should we open office of our startup to attract new workers?
We will be exploring the boroughs and venues of Berlin to find out where is the best place to locate your new office. At the end of the project, we will be giving suggestions of locations to CEOs or Managers of startups for setting up their new offices.

## 2. Data Description
In this project, the data will be related to the Berlin location. I have three different data sets. I will clean the data, make some preparations and then combine all of them to get the final data set.
The first data set was extracted online from geonames.org and in the form of a CVS file. [4] It is composed of the information of Berlin Postal Codes, and Location (Latitude/Longitude). In this data, each postal code has its unique coordinate data in the Location column. The location column will be dividing two different columns in the data preparation phase since the column contains two different data and we will be using them separately in the project. Postal Codes are numeric data with five figures(e.g. 10115), and the Location column is Varchar data type with latitude and longitude information (e.g. ‘52.532/13.385’).
The second data set was also extracted online from geonames.org. [4] It is in CSV file format and contains Postal Codes and Boroughs of Berlin. In data each Postal Code corresponds to a borough, so we are expecting that some postal codes are in the same borough. Postal codes are numeric (integer) with five figures like 10115 and the Borough column is Varchar data type (e.g. ‘Berlin-Mitte’). This data set will be combining with others later based on the Postal Code column.
The third data set is extracting from foursquare by using Foursquare API for getting the most common venues in Berlin. The API is returning us the most common venues in Berlin, neighborhoods, latitude/longitude information, venue names, and venue categories. After getting and combining data sets, I will be using the Folium library for map rendering. I will give details in the methodology section.
By combining these three data sets I will be exploring, clustering, and make data analysis based on combined data.
