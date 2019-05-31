It's Dog Time

The purpose of this project was to successfully perform ETL on a series of data sets in a group setting. We took advantage of the variety of data sets available on Kaggle and chose to examine data available on dogs living in New York. The first data set included here is a csv file including a sample of 16,217 names of dogs living in NYC and the second data set includes 121,827 licensed dogs in NYC. All analysis was completed via Jupyter Notebook. 

The first step of our ETL process was to extract the original CSV files from Kaggle,import the CSV files into a jupyter notebook and create two seperate dataframes using Pandas. This is crucial for any future cleaning or analysis.

The second step of our ETL process was to transform our data into a clean and best organized form. This involves renaming columns, sorting values in several columns, and dropping any unnessecary rows we do not forsee using in our analysis (repeats, NA, etc.). After transforming the first data frame, we were able to 
create a table with the most popular dog names in NYC. The winner is Bella, followed by Max and Charlie! Next, we transformed the second data frame to determine the breeds with the most licensed dogs categorized under each breed. This is displayed in a table showing the top 10 most popular breeds. Our analysis showed Yorkshire Terrierto be the most popular, with 7,359 licensed dogs. To take it one step further, we created a dataframe to show the most popular name for each breed. This was by far the most extensive of the dataframes, involving several group by's, ranking and loc functions. For futher analysis, we merged the two CSV files into one dataframe. This allows further examination of the current dog popularity in NYC. Our last table shows which buroughs currently have the most licensed dogs, with Manhattan ranking at number one. 

The second major step  of our transformation process was to scrape the internet for dogs images that we could match to the breeds included in the original CSV files. This is completed by importing splinter, launching the url to be scraped, and creating a dictionary containing the breed's with their corresponding urls. By looping through our data, we came up with 298 unique breeds and their images. 

For the third step of our ETL process, we loaded our data into a MySQL database using SQL Alchemy. We took the databases that was created through Pandas and make them into SQL Database tables through SQLAlchemy. We also joined two tables, the table containing the image URLs and out Breed Ranking using SQLAlchemy. While joining we decided to transform the missing BreedName values to suit our DB.


- - -

### Copyright

Trilogy Education Services © 2017. All Rights Reser
