# Predicting tennis matches using machine learning
In this project, I scraped tennis match data from the web and used it as part of a machine learning model to predict the outcome of new matches.

### Scraping.ipynb
This file contains the code used to extract the desired data from the web and load it into a SQL database.
The data was extracted from the [tennis explorer](https://www.tennisexplorer.com/) website, and contains every top level mens singles match form 2000-2021. The raw HTML was parsed and 25 unique features were extracted and loaded into 5 different tables.

The final data extracted totaled 59,715 matches, 1,461 unique players and 155 unique tournaments. 

### Transformation.ipynb
Code in this file transforms the separate tables in the SQL database in order to engineer features to be used in the machine learning model. K-means clustering was applied to multiple features in order to sort data into buckets.
