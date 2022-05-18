# Overview of Analysis 

The purpose of this analysis was to analyze temperature data for June and December in Oahu to determine if the surf and ice cream shop will be sustainable year-round. 

## Results 

After performing the analysis using pandas and python, below are the overall summary statistics for June and December weather data. 

June Data:

<img width="359" alt="June_Summary" src="https://user-images.githubusercontent.com/101602688/168943289-45868f44-90b3-412b-bc08-8343e63495bf.png">

December Data:

<img width="314" alt="December_df" src="https://user-images.githubusercontent.com/101602688/168943295-709a2bd5-dd9b-48eb-9b46-29dcfe049b96.png">


From the above, below are 3 main takeways garnered from the analysis:

* The average temperatures in June and Decemeber are only 3.9 degrees apart, indicating the weather does not fluctuate that greatly in Decemeber which indicates the shop will not be impacted by colder temperatures typically expected in Decemeber 

* The max temperature in December and June are only 2 degrees apart, with June being slightly higher. This further shows the temperature does will not vary in Decemeber and June. 

* The standard deviation of temperatures in June and Decemeber are each small, indicating the temperature does not have any severe outliers and is generally consistent. 

## Summary 

Overall, opening the Surf and Ice Cream shop is feasible as the weather in Decemeber which is typically regarded as a colder month does not vary from the temperature in June. This shows the weather remains consistent and will not be a limiting factor for the business. 

Two additional queries that could have been performed to gather more weather data for June and December should include precipitation data as rain can be a crucial factor in customers wanting to surf. In addition, we can compare March and April as these months are usually when tourists travel to Hawaii. Below are the queries: 

* This query finds the the precipitation scores for the months of June and December 

    * results = session.query(Measurement.date, Measurement.prcp).filter(extract('month',Measurement.date==6).all()

    *  results = session.query(Measurement.date, Measurement.prcp).filter(extract('month',Measurement.date==12).all()

* This query finds the March and April temperature data 

    * results = session.query(Measurement.date, Measurement.prcp).filter(extract('month',Measurement.date==3).all()

    *  results = session.query(Measurement.date, Measurement.prcp).filter(extract('month',Measurement.date==4).all()



