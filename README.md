# GreenHouseGas-Emissions-EU
Software related to Data related to GreenHouseGas emissions-EU

I subscribed to "Eurostat - Greenhouse Gas Emissions Intensity of Energy Consumption" delivered by CRUX using Amazon AWS Data Exchange. New datasets are added once a year for this product, so I took the latest revision of data set available in AWS Data Exchange and stored it in AWS S3. I extracted the data from  .CSV and .GeoJSON datasets in S3 and created the tables using Extract, Transform, Load function and crawlers in AWS Glue. I created table "greenhouse_eucx05564", that can be used in AWS Athena to create queries, group queries based on a condition and to filter data. 
For data visualization, interpretation and calculations for predictions, I used AWS QuickSight. The input data for generating visualizations in QuickSight is from Athena.
The data in these reports are generated using AWS - Quicksight with the Visual type - Line chart, Pivot table, Vertical Bar Chart using Quick Sight filters and 
calculations based on a new parameter value. The data is taken from the table "greenhouse_eucx05564" in AWS Athena.
