# Overview of the analysis
This analysis gives a 360 view of a CitiBikeNYC data set acquired from  https://www.citibikenyc.com/system-data. A customer would like to see a full scale analysis to aid the decision to begin a Citi Bike program in Des Moines, Iowa. 

## Results
### Python
Adjusting the data set in Python was a first step to making the data easy to use in Tableau. In Python, I chose to add a column called tripduration_Long. This took the tripduration column (which was an iteger with the unit of seconds) and adjusted it to Hours:Minutes:Seconds. This anabled a micro analysis of ride length while still keeping the seconds for easy aggregate KPIs. 

<img width="1096" alt="Screen Shot 2021-07-13 at 11 35 54 AM" src="https://user-images.githubusercontent.com/14239715/125642673-0b3c55ca-1f90-4e64-9004-b41bde53e4b4.png">


### Tableau_bikesharing

https://public.tableau.com/app/profile/luegreen/viz/Module_14_challenge/Story1

### Page 1 of Story
<img width="961" alt="Screen Shot 2021-07-14 at 11 04 17 AM" src="https://user-images.githubusercontent.com/14239715/125645722-5508554a-4658-454a-9945-8c13ee69efa7.png">

This analysis shows 1) the huge discrepancy between rides that are three hours or less vs all other lengths and 2) that there still are rides of all lengths, although not many. This viz shows a distribution of the data set in a way that is very consumable as opposed to a histogram or regular bar. 

<img width="971" alt="Screen Shot 2021-07-14 at 11 05 09 AM" src="https://user-images.githubusercontent.com/14239715/125645733-21da6745-66e0-4d25-9307-a700018db721.png">

These high level KPIs would normally go on the top of a dashboard but they seemed to take second place to the above viz. Also, Tableau Public's height leaves the viewer on a laptop scrolling down to see the full aspect so these vizualizations seemed ok to be 'below the fold'. They show the high level veiw of the ridership. However, with no unique customer identifier in the data set, the analysis by type and customer are not as useful as one would hope. Each repeat customer is double counted, leaving the gender and type analysis skewed toward repeat customers. (a male using two rides is counted as two males.)


### Page 2 of Story

<img width="1062" alt="Screen Shot 2021-07-14 at 11 05 37 AM" src="https://user-images.githubusercontent.com/14239715/125645746-c7b57009-58f1-4afa-94b0-00126c587cd3.png">
<img width="1026" alt="Screen Shot 2021-07-14 at 11 05 42 AM" src="https://user-images.githubusercontent.com/14239715/125645756-c8457d3c-ff03-4664-93fc-073c8be9cd1d.png">
<img width="545" alt="Screen Shot 2021-07-14 at 11 05 48 AM" src="https://user-images.githubusercontent.com/14239715/125645807-1fdc0193-fc43-4f99-bae7-d7f451969d07.png">

<img width="495" alt="Screen Shot 2021-07-14 at 11 05 52 AM" src="https://user-images.githubusercontent.com/14239715/125645809-69053573-038e-49c4-b09a-a789dd4f1576.png">

### Page 3 of Story

<img width="477" alt="Screen Shot 2021-07-14 at 11 06 13 AM" src="https://user-images.githubusercontent.com/14239715/125645841-2902b62d-9ed2-4fb5-9621-cb75ee7eb539.png">
This heatmap shows utilization by most common days of week. Again, keep in mind the potential double counting of Gender and Type. From this chart, both Thursday and Friday show the highest utilization by the highest use group, male subsribers. 


<img width="390" alt="Screen Shot 2021-07-14 at 11 06 07 AM" src="https://user-images.githubusercontent.com/14239715/125645847-7efd5b21-f721-4ca3-96fa-0d6de0b7cd90.png">
The above chart shows peak riding time by the minute. This shows more detail than the by the hour bar chart (which is still available by clicking the 'plus' sign on the unit title). Commuting times appear to be the highes utlization windows, at 8 a.m. and 4-5 p.m. 

<img width="1101" alt="Screen Shot 2021-07-14 at 11 06 19 AM" src="https://user-images.githubusercontent.com/14239715/125645856-72ccd1e3-30a2-411a-ba12-f1bd82d3b1dd.png">
These final heatmaps show a further breakdown of utilization. The two charts match, but the one on the right is filterable by gender. One can use the chart on the left to compare any filtered selection to the population as a whole. 


## Summary:
To submit a recommendation for the Des Moines buisiness, I would include the following Future Analysis. 

Future analysis:
It would be good to compare the populations of Des Moines to NYC, particular the city density, seasonal viablity of bike riding, and relative distances of the city limits as compared to NYC. 

For this data set, I would like to analysis which CitiBike stations had what action: I would break the stations into three groups: most popular pick-up AND drop-off stations, most popular pick-up stations only, most popular drop-off stations only. Then I would like to draw a lined map of the infrastructure needed to get the bikes at the most likely drop off stations BACK to the most likely pick-up stations, and the distance needed to be covered in between. 
