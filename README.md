## nosql-challenge

The UK Food Standards Agency evaluates various establishments across the United Kingdom, and gives them a food hygiene rating. 

#### Part 1: Database and Jupyter Notebook Set Up
In part 1, the data from the establishments.json file were imported. The database and the collection were named as uk_food and establishments, and the database and the data were checked to see if the data were loaded to the jupyther notebook properly. Below shows steps that were done in Part 1. 

- Import the libraries you need: PyMongo and Pretty Print (pprint).
- Create an instance of the Mongo Client.
- Confirm that you created the database and loaded the data properly:
- List the databases you have in MongoDB. Confirm that uk_food is listed
- List the collection(s) in the database to ensure that establishments is there
- Find and display one document in the establishments collection using find_one and display with pprint.
- Assign the establishments collection to a variable to prepare the collection for use.


#### Part 2: Update the Database
In part 2, changes to the establishments collection were made. Below are the steps that were done in Part 2.

- Find the BusinessTypeID for "Restaurant/Cafe/Canteen" and return only the BusinessTypeID and BusinessType fields.
- Update the new restaurant with the BusinessTypeID you found.
- Check how many documents contain the Dover Local Authority.
- Remove any establishments within the Dover Local Authority from the database, and check the number of documents to ensure they were deleted.
- Use update_many to convert latitude and longitude to decimal numbers.
- Use update_many to convert RatingValue to integer numbers.

- #### Part 3: Explorative Analysis
In part 3, Further analyzed the data. Below were the stpes done for the further analysis.

- Display the first document in the results using pprint.
- Convert the result to a Pandas DataFrame, print the number of rows in the DataFrame, and display the first 10 rows.
- Which establishments have a hygiene score equal to 20?
- Which establishments in London have a RatingValue greater than or equal to 4?-
- What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
- How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.
