# UK Food Establishment Analysis  
By Kiana Navarre

**Programming Language/Libraries Used: NoSQL, PyMongo, Pretty Print, Python**

## Description
The goal of this project is to evaluate food hygeine ratings given by the UK Food Standard Agency to various establishments across the UK.  The purpose of this evaluation is to help journalists and food critics for the fictional food magazine "Eat Safe, Love" decide where to focus future articles. The project is divided into the following sections: 
1. Database and Jupyter Notebook Set Up 
2. Update the Database
3. Exploratory Analysis

## Database and Jupyter Notebook Set Up 
In this section, the uk_food database is created by importing the data provided in the establishments.json file located in the Resources folder.  Following the creation of this database, following actions are performed using a Jupyter notebook: 
- Confirm the uk_food database has been created
- Ensure that the establishments collection is present
- Find and display one document in the establishments collection using find_one and display with pprint

## Update the Database
The following modifications to the database were required:
- Add restaurant data for the resaurant Penang Flavours to the database
- Find and BusinessTypeID for "Restaurant/Cafe/Canteen", returning the BusinessTypeID and Business Type
- Update the BusinessTypeId for the newly inserted resaurant (Penang Flavours)
- Remove establishments within the Dover Local Authority from the database
- Convert latitude and longitude from strings to decimal numbers

## Exploratory Analysis
In this section, an analysis is performed to answer the following questions: 
1. Which establishments have a hygiene score equal to 20? 
2. Which establishments in London have a RatingValue greater than or equal to 4? 
3. What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
4. How many establishments in each Local Authority area have a hygeine score of 0?