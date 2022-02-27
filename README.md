# Installations
- Python version 3.8.5
- All packages were installed with the Anaconda distribution
- Packages used:
	- pandas
	- numpy
	- nltk
	- datetime
	- matplotlib
	- statsmodels


# Project Motivation
- This goal of this project is to apply the CRISP-DM process to a dataset for the Udacity Data Science Nanodegree program's first project.  A dataset needed to be selected, explored, prepared, and analyzed using data science techniques.  I chose cardio fitness activities data that I had recorded via the [RunKeeper app](https://runkeeper.com/cms/) starting in 2011.  Runners often ask
themselves if they are improving over time, and I had a unique opportunity to explore that in this project. 


# File descriptions

| Name| Description |
| ----------- | ----------- |
| cardioActivities.csv| The cardio activities data were pulled from the RunKeeper app which allows users to download their data.  Users must request their data, and it is accessible via a Runkeeper account within 2 business days.  |
| minneapolis_st_paul_weather_data.csv| Daily [temperature data](https://www.dnr.state.mn.us/climate/historical/daily-data.html?sid=mspthr&sname=Minneapolis/St%20Paul%20Threaded%20Record&sdate=2010-01-01&edate=por) in the Minneapolis/St. Paul, MN area |
| madison_wi_temp.csv| Daily [temperatuare data](https://dev.nceas.ucsb.edu/view/urn%3Auuid%3A9fc1a36b-cca5-4c02-90df-3c224349bc97) in the Madison, WI area|
| cardio_analysis.ipynb | Associated jupyter notebook that shows the detailed analysis|

- Temperature data was pulled from two different sites to match the temperature in the main two locations that the activities were logged.

# How to interact with this project
The jupyter notebook within the repository was designed for others to replicate the analysis if desired.  The associated blog post with the questions, data preparation, and results can be found in this medium [link](https://medium.com/@mark.golob.j/analyzing-runkeeper-data-to-help-with-fitness-training-200b1f172e4d).  

## Data preparation summary.  
- Temperature data were joined with the activities data based on the date.  
- Data with the majority of values missing were removed.  Heart rate had a high percent (92%) of missing values, but was kept to gauge accuracy of the measurements.  
- Month, year, and season were extracted from the date to determine if those factors impacted performance. 
- Several records with low temperatures were removed since those were likely errors while I was walking inside.   

## Results summary
- Comments from the activities data regarding hot days were checked against the temperature data
as a validation that the join was accurate.  
- Performance metrics did not have a drastic improvement over time, but performance was maintained throughout the time period. 
- With the 2020 pandemic, that allowed for more activities and subsequently increased performance.

# Licensing, Authors, Acknowledgements
Thank you to RunKeeper for making the data accessible, the MN Department of Natural resources for allowing public access to temperature data, and to Paloma Cartwright and Joe DeCesaro for the 
Madison temperature data.  Thank also to you to stack overflow for help with vectorizing the text within the Notes column.  




