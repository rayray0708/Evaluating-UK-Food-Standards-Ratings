![Illustration of NoSQL](https://www.scnsoft.com/blog-pictures/business-intelligence/no-sql-databases.png)
# Evaluating-UK-Food-Standards-Ratings
## Description
The UK Food Standards Agency evaluates various establishments across the United Kingdom, and gives them a food hygiene rating. For this challenge, I've been contracted by the editors of a food magazine, Eat Safe, Love, to evaluate some of the ratings data in order to help their journalists and food critics decide where to focus future articles.

## Usage
To see the code for Part 1: Database and Jupyter Notebook Set Up and Part 2: Update the Database, please navigate to the NoSQL_setup_starter.ipynb file.

To see the code for Part 3: Exploratory Analysis, please navigate to the NoSQL_analysis_starter.ipynb file.

## Installations
The following dependencies were imported to run the code:
1. `from pymongo import MongoClient`
2. `from pprint import pprint`
3. `import pandas as pd`

Make sure you have these libraries pre-installed:
1. `!pip install pymongo`
2. `!pip install pandas`

## UK food ratings analysis
A document in our `establishments` collection have the following field names:
![Alt text](<Screenshot 2023-12-18 at 2.39.48 pm.png>)

In the analysis section, I'll query the database to answer these questions:
1. Which establishments have a hygiene score equal to 20?
2. Which establishments in London have a RatingValue greater than or equal to 4?
3. What are the top 5 establishments with a RatingValue rating value of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
4. How many establishments in each Local Authority area have a hygiene score of 0? 
* For this question, I created a pipeline (code shown below) that (1) Matches establishments with a hygiene score of 0, (2) Groups the matches by Local Authority, (3) Sorts the matches from highest to lowest. Subsequently, I converted the results into a Pandas dataframe and displayed only the first 10 results (as shown in the dataframe below). 

![Alt text](<Screenshot 2023-12-18 at 2.45.12 pm.png>)

![Alt text](<Screenshot 2023-12-18 at 2.46.33 pm.png>)


## Credits
Special thanks to the following individuals for their contribution to this project:

-BCS learning assistants
