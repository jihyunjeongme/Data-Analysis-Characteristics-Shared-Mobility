<h1 align="center">
  <br>
  <a href="https://bit.ly/3a37BIU"><img src="https://user-images.githubusercontent.com/43984584/201550450-8c125763-6c39-4e6d-9fb3-b0b44eb19dda.png" alt="Markdownify" width=""></a>
  <br>
  
  <br>
</h1>

<h1 align="center"> A Study on the Analysis of Use Characteristics of Shared Mobility: Focused on Gangnam-gu, Seocho-gu and Songpa-gu
</p>

# ABSTRACT
- With the recent revitalization of the sharing economy, shared mobility such as shared bicycles and shared mobility is in the spotlight.
This study investigated their use patterns, correlations of shared mobility, and the effect of corona on the usage of shared mobility, centered on Gangnam-gu, Seocho-gu, and Songpa-gu, in order to suggest efficient ways to use shared mobility. For the empirical study, log data of companies operating shared mobility were collected and usage patterns according to time, day of the week, and distance traveled were analyzed. As a result, the amount of use was the most during the commute time, and the amount of use at the time of departure was higher than that of the commute time. There was more usage on weekdays than on weekends, and there was a big difference between weekdays and weekends during rush hour. The frequency of use was high in the order of short distance, long-distance, and medium distance according to the distance traveled. Here, in the case of long distances, unlike short and medium distances, the amount of use during the last train hours of public transportation increased dramatically. In addition, we compared and analyzed the use of shared mobility according to the number of confirmed COVID-19 patients in Seoul. As a result, between March and May 2020, the use of shared mobility increased (+), while shared bicycles decreased (-).
These results fully demonstrate the possibility that the shared kickboard will serve as a secondary vehicle for public transport. However, currently, research on shared mobility has been conducted only in a limited range, and information such as the scope of service provision and usage history has not been provided.
This study is meaningful in that it provides information such as usage patterns in the efficient operation plan of the shared kickboard, and verifies the possibility of development in connection with other public transportation means.

## Data collection and preporcessing
- This study is conducted based on data from service providers that start their services first in Gangnam-gu, Seocho-gu, and Songpa-gu among major domestic and foreign electric kickboard service providers and expand them to all parts of Seoul. Therefore, this study is limited to a total of three districts: Gangnam-gu, Seocho-gu, and Songpa-gu, and data collected from January 1 to November 30, 2020 were used. The data for analysis is composed as follows.
- Data was collected in the designated area every 10 minutes using the cloud service and stored as a JSON file. And the distance travel distance was calculated by checking the change in latitude and longitude (using the geopy.distance package). In the data preprocessing process, movement of less than 300M for more than 10 minutes was excluded. In addition, the case of moving more than 3.6KM of travel distance of 10/10 based on the maximum speed of 25km/h was also considered as an outlier and excluded from the analysis.
For data collection, electric kickboard data is collected around Gangnam-gu, Seocho-gu, Songpa-gu (Samsung Station, Seolleung Station, Yeoksam Station, Gangnam Station, Jamsil Station, and Express Terminal Station), which are the most frequently serviced by shared kickboard companies. In addition, the daily average number of people getting on and off in 2019 (1st: Gangnam Station, 2nd: Jamsil Station, 6th: Express Terminal Station, 7th: Samseong Station) was referenced.

### data columns
<img width="648" alt="image" src="https://user-images.githubusercontent.com/43984584/201550753-789bc9d9-5215-4010-8ebc-5cb46d695e63.png">

## Analysis and Results
- EDA, Analysis, and Results - A Study on the Analysis of Use Characteristics of Shared Mobility.ipynb
