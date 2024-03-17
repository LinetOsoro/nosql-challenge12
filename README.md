Eat Safe, Love


The UK Food Standards Agency evaluates various establishments across the United Kingdom, and gives them a food hygiene rating. You've been contracted by the editors of a food magazine, Eat Safe, Love, to evaluate some of the ratings data in order to help their journalists and food critics decide where to focus future articles.



Part 1: Database and Jupyter Notebook Set Up

Import the data provided in the establishments.json file from your Terminal. Name the database uk_food and the collection establishments. Use PyMongo and Pretty Print (pprint).

Create an instance of the Mongo Client and confirm that you created the database and loaded the data properly:

List the databases you have in MongoDB. Confirm that uk_food is listed. List the collection(s) in the database to ensure that establishments is there. Find and display one document in the establishments collection using find_one and display with pprint.



Part 2: Update the Database

Use NoSQL_setup_starter.ipynb for this section of the challenge.

The magazine editors have some requested modifications for the database before you can perform any queries or analysis for them. 

An exciting new halal restaurant just opened in Greenwich, but hasn't been rated yet. The magazine has asked you to include it in your analysis. Update the new restaurant, check for Dover and delete that. Some numbers values will need to be changed to strings.



Part 3: Exploratory Analysis

Eat Safe, Love has specific questions they want you to answer, which will help them find the locations they wish to visit and avoid.

Use NoSQL_analysis_starter.ipynb for this section of the challenge.

Some notes to be aware of while you are exploring the dataset:

RatingValue refers to the overall rating decided by the Food Authority and ranges from 1-5. The higher the value, the better the rating.

Note: This field also includes non-numeric values such as 'Pass', where 'Pass' means that the establishment passed their inspection but isn't given a number rating. We will coerce non-numeric values to nulls during the database setup before converting ratings to integers.

The scores for Hygiene, Structural, and ConfidenceInManagement work in reverse. This means, the higher the value, the worse the establishment is in these areas.



Questions to be answered: 

1--Which establishments have a hygiene score equal to 20?

2--Which establishments in London have a RatingValue greater than or equal to 4?

3--What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?

4--How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.
