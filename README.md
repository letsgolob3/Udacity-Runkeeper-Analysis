# Installations
- Python version 3.8.5
- All packages were installed with the Anaconda distribution
- Packages used:
	- pandas
	- numpy
	- nltk
	- datetime
	- matplotlib


# Project Motivation
- This goal of this project is to apply the CRISP-DM process to a dataset for the Udacity Data Science Nanodegree program's first project.  A dataset needed to be selected and then 
explored, preparred, and analyzed using data science techniques.  I chosen cardio activities data that I had recorded via the RunKeeper app starting in 2011.  Runners often ask
am I improving my fitness, and I had a unique opportunity to explore that here.  


# Data sources
The cardio activities data were pulled from the [RunKeeper app](https://runkeeper.com/cms/) which allows users to download their data.  Users must request their data, and it is
sent within 2 business days.  

Temperature data was pulled from two different sites to match the temperature in the main two locations that the activities were logged:
- Minneapolis/St. Paul, MN [temperature data](https://www.dnr.state.mn.us/climate/historical/daily-data.html?sid=mspthr&sname=Minneapolis/St%20Paul%20Threaded%20Record&sdate=2010-01-01&edate=por)
- Madison, WI [temperature data](https://dev.nceas.ucsb.edu/view/urn%3Auuid%3A9fc1a36b-cca5-4c02-90df-3c224349bc97)

# Data Preparation
Temperature data were joined with the activities data based on the date.  

Data with the majority of values missing were removed.  Heart rate had a high percent (92%) of missing values, but was kept to gauge accuracy of the measurements.  

Month and year were extracted from the date to determine if there were correlations with performance. 

Several records with low temperatures were removed since those were likely errors while I was walking inside.   

# Results
Comments from the activities data regarding hot days were checked against the temperature data
as a validation that the join was accurate.  





# File Descriptions
The XXX.ipynb file is included in this repository and shows the detailed analysis.  The associated blog post can be found in this medium link.  

# How to interact with this project
The jupyter notebook within the repository was designed for others to replicate the analysis if desired.  

# Licensing, Authors, Acknowledgements
Thank you to RunKeeper for making the data accessible, the MN Department of Natural resources for allowing public access to temperature data, and to Paloma Cartwright and Joe DeCesaro for the 
Madison temperature data.  




