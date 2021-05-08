# Aid Data Visualization in D3.js

 Exploratory data analysis of AidData of aids exchanged between countries in D3.js. This data was collected from https://www.aiddata.org/ and the data is as follows:
 
![alt text](https://github.com/KshitijaSAPatel/Aid-Data-Visualization-in-D3js/blob/main/Data_sample.png)

----
### Notebooks and Code :
Observable notebooks were used to write and run the codes.
<ul>
 <li> Part 1 : </li>
 <li> Part 2 : https://observablehq.com/d/3bcb72339a5a731c </li>
 <li> Part 3 : https://observablehq.com/d/921e44ea01c02a89 </li>
</ul>

----
### Questions and Visualizations :

#### 1.
a) Who are the major donors and to which countries do they donate the most and how much? 
b) Who are the major receivers and which countries do they receive from the most and how much?

![alt text](https://github.com/KshitijaSAPatel/Aid-Data-Visualization-in-D3js/blob/main/donor_receiver_relationship.png)

I chose a sankey diagram with donor countries on left and recipients on the right. The width of each band going from a donor country to a recipient country represents the amount in USD being sent between these countries.

#### 2.
a) Considering only the top 5 purposes of donation, how does the relationship between countries look like in terms of purposes? 
b) What composition (distribution) of purposes do the donations between each pair of countries have? 
c) Are there countries that donate to a given country using multiple purposes? Or do counties always donate using one single purpose when donating to another country?

![alt text](https://github.com/KshitijaSAPatel/Aid-Data-Visualization-in-D3js/blob/main/donor_receiver_relation_wrt_purpose.png)

Similar sankey diagram where bridging the donors and recievers are the purposes. It is easy to see that Air Transport is top purpose and USA is the top donor to it. Similarly Japan is the top donor for Rail transport and India is it's largest receiver. And Germany donates to Brazil only for the purpose of Rescheduling and Refinancing

#### 3.
What are the top 10 purposes of disbursements (in terms of total amount of disbursement) and how does their relative amount compare over time?

![alt text](https://github.com/KshitijaSAPatel/Aid-Data-Visualization-in-D3js/blob/main/purposes_vs_time.png)

Having 10 lines on a line chart was getting too crowded, even though it is more intuitive. Thus I choose to plot time vs the 10 purposes using heat map. Color encodes the amount of money.

#### 4.
a) Focusing exclusively on countries that receive donations, how do donations shift geographically over time? 
b) Do donations tend to be always in the same regions of the world over the years or they have been shifting over time?

![alt text](https://github.com/KshitijaSAPatel/Aid-Data-Visualization-in-D3js/blob/main/geographical_donations.png)

I chose to use interaction in this visualization where year can be selected using the drop-down, and I depicted the change wrt to time through different choropleth maps.

#### 5.
a) How do the countries compare in terms of how much they receive and donate? 
b) Are there countries that donate much more than they receive or receive much more than they donate?

![alt text](https://github.com/KshitijaSAPatel/Aid-Data-Visualization-in-D3js/blob/main/receive_vs_donate_1.png)

![alt text](https://github.com/KshitijaSAPatel/Aid-Data-Visualization-in-D3js/blob/main/receive_vs_donate_2.png)

I chose the grouped bar chart and spine chart for this visualization because it is easy to compare amount donated and received within a country as well as with other countries because of the sorted order. The contrasting color scale also make it easy to identify the same.

#### 6.
a) Do the countries that mostly receive or mostly donate tend to cluster around specific geographical areas of the world? 
b) Are there neighboring countries that have radically different patterns in terms of how much they receive vs. how much they donate?

![alt text](https://github.com/KshitijaSAPatel/Aid-Data-Visualization-in-D3js/blob/main/net_graphical.png)

I chose choropleth visualization because it makes it very easy to compare countries with the coutries geographically close to it, i.e neighboring countries. I chose to represent the net amount for each country (donated - received) on a diverging color scale to make it intuitive to compare countries that mostly donate with countries that mostly recieve. Size is used as a channel by using bubble chart. I had earlier tried heat map but the small European countries where net is close to 0 are very difficult to comprehend

#### 7.
a) Are there any major differences in how the top 5 most frequent purposes of disbursements (across all countries) distribute geographically in terms of countries that receive donations? 
b) Are there countries that tend to receive more of certain types of donations than others?

![alt text](https://github.com/KshitijaSAPatel/Aid-Data-Visualization-in-D3js/blob/main/Purposes_vs_countries.png)

#### 8.
a) How does the amount donated vs. amount received change over time for each country? 
b) Are there countries that mostly send or mostly receive and countries that have a similar amount of donations they receive and send? 
c) Are there countries that change their role over time? 
d) Are there countries in which you can find a sudden increase ("peak") or a sudden decrease ("valley")?

![alt text](https://github.com/KshitijaSAPatel/Aid-Data-Visualization-in-D3js/blob/main/receive_donate_vs_time.png)

----

# Other Projects in D3.js

## Unemployment rate data for each US state for December 2019

Grid Cartogram
![alt text](https://github.com/KshitijaSAPatel/Aid-Data-Visualization-in-D3js/blob/main/Unemploment_Rate_Dec_2019/Grid%20Cartogram.png)

Speedometer Chart
![alt text](https://github.com/KshitijaSAPatel/Aid-Data-Visualization-in-D3js/blob/main/Unemploment_Rate_Dec_2019/Speedometer%20Chart.png)

Bubble Chart
![alt text](https://github.com/KshitijaSAPatel/Aid-Data-Visualization-in-D3js/blob/main/Unemploment_Rate_Dec_2019/Bubble%20Chart.png)

Donut Chart
![alt text](https://github.com/KshitijaSAPatel/Aid-Data-Visualization-in-D3js/blob/main/Unemploment_Rate_Dec_2019/Donut%20Chart.png)

## NYC Film Permits Data 
Source Code : https://observablehq.com/d/b24a370433b5fe15

Q. What is the relationship between the duration of the permit and the permit category?
![alt text](https://github.com/KshitijaSAPatel/Aid-Data-Visualization-in-D3js/blob/main/NYC%20Film%20Permits/cat%20vs%20duration.png)

Q. How are the film permits distributed across zip codes? Are there areas where the permits concentrate?
![alt text](https://github.com/KshitijaSAPatel/Aid-Data-Visualization-in-D3js/blob/main/NYC%20Film%20Permits/zipcode%20distribution.png)

Q. What is the distribution of permit categories for each borough? 
![alt text](https://github.com/KshitijaSAPatel/Aid-Data-Visualization-in-D3js/blob/main/NYC%20Film%20Permits/borough%20distribution.png)

Q. How does the number of permits that start per month change seasonally (across the months of a year)?
![alt text](https://github.com/KshitijaSAPatel/Aid-Data-Visualization-in-D3js/blob/main/NYC%20Film%20Permits/seasonal.png)
