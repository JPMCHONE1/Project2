###### Project2

# When running this please run WH + ISO first
# We decided to focus on the World Happiness Report (WHR) & collect data points that would be of interest to review. Typically this is aggregated by country. 

# The WHR was downloaded from https://worldhappiness.report/ed/2021/ as a CSV which we converted into a data frame. 

# We then imported the ISO standardization for each country to act as a reference for all tables. This was imported from Kaggle. https://www.kaggle.com/datasets/juanumusic/countries-iso-codes

# We joined these two df together on the country name

# We created a dataframe with only the country & the 3 letter alpha code - this will be our join table

# We also created a seperate df from this data that included the country code with the relevant happiness report data - we eliminiated a couple of statistical columns that wouldn't be used for analysis

# These two dataframes were turned into tables for reference

# In order to interact with this data we went to World Bank:
### World Bank API Python library documentation
### Install using . pip install wbgapi. The install doesn't work in python files or jupyter notebook. Must be installed in terminal.
### Documentation is located at https://pypi.org/project/wbgapi/.
### Documentation states that the World Development Indicators database id is 2.

# WB has a large number of series topics which we downloaded using the above api calls to bring in for review. We scrubbed the list for metrics we felt might be influencers in the WHR & would need further analysis. 

# Once we had this list we called for the those data points by country 

# The data brought in then created a new dataframe that houses all of the country specific data. 

# When this was complete we created a database that had 3 tables created from these dataframes with a primary key of country in the join table & as a foreign key in the other tables. 

## Thank You!
