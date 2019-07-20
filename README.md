# Team-16-ETL-Project



Extract: Our data was taken from Kaggle [https://www.kaggle.com/benhamner/2016-us-election/]. Data was on the 2016 Presidential Primary results from across the US. 
It contained “primary_results.csv” which was a dataset of primary voter results. We also used “county_fact.csv,” a dataset containing demographics of every county in the Federal Information Processing Standards. The two datasets were initially loaded and formatted in Pandas.


Transform: We transformed the data in Pandas by:
•	The column headers in the Demographics table were coded.  These headers were renamed in pandas.  
•	Only the required columns were brought into the final dataframe.
•	The demographic columns included FIPS code, gender, ethnicity, household income
•	Primary results table was also imported into Pandas as a csv file.
•	The only the required columns were brought into the final dataframe.
•	The columns included were FIPS Code, state, county, vote count, political party, and candidate.


Load: We loaded and joined the final pandas dataframes into Postgres.  The two datasets can be relationally joined on the primary key FIPS code to start the analysis. We choose Portgres to allow for new datasets and clear segmentation of data.




