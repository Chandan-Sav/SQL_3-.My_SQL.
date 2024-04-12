# Swiggy Dataset SQL_queries
## About

This project aims to explore the Swiggy data to understand top performing restaurants and menus, cuisines of different types, customer behaviour. The aims is to study how some of the queries were solved using SQL Queries. The dataset is [Swiggy_Dataset](https://www.kaggle.com/datasets/chandansav/swiggy-dataset).

These markdowns are known to affect some of the, but it is challenging to predict which departments are affected and the extent of the impact." [source](https://www.kaggle.com/datasets/chandansav/swiggy-dataset)

## Purposes Of The Project

The major aim of thie project is to do the  case study for data of Swiggy to understand the different factors that affect customer.

## About Data

The dataset was obtained from the [Swiggy_Dataset](https://www.kaggle.com/datasets/chandansav/swiggy-dataset). This dataset contains all customer transactions from a three different categories of swiggy, respectively. The data contains 12 columns and 50K+ rows:

| Column                  | Description                             | Data Type      |
| :---------------------- | :-------------------------------------- | :------------- |
| restaurant_no             | Number's of Restaurant              | INTEGER    |
| restaurant_name                 | Name of a Restaurant        | VARCHAR(50)     |
| city                  | city's name          | VARCHAR(9)    |
| address         | Address of a restaurants              | VARCHAR(204)   |
| rating                  | Restaurant rating's   |NUMERIC(3,1)   |
| cost_per_person         | The price of each person in restaurants       | INTEGER   |
| cuisine            | Cuisine name               | VARCHAR(49) |
| restaurant_link              | Restaurant's restaurant official link          | VARCHAR(136)          |
| menu_category                 | Menu category       | VARCHAR(66)    |
| item                 | Other item's in Restaurant          | VARCHAR(188) |
| price                  |Price of each cuisine | VARCHAR(12)        |
| veg_or_nonveg                 |Food categorised in veg/non-veg| VARCHAR(7)           |


## Case Study Queries to find

### Queries

1. HOW MANY RESTAURANTS HAVE A RATING GREATER THAN 4.5?
2. WHICH IS THE TOP 1 CITY WITH THE HIGHEST NUMBER OF  RESTAURANTS?
3. HOW MANY RESTAURANTS HAVE THE WORD "PIZZA" IN THEIR NAME?
4. WHAT IS THE MOST COMMON CUISINE AMONG THE RESTAURANTS IN THE DATASET?
5. WHAT IS THE AVERAGE RATING OF RESTAURANTS IN EACH CITY?
6. WHAT IS THE HIGHEST PRICE OF ITEM UNDER THE 'RECOMMENDED' MENU CATEGORY FOR EACH RESTAURANT?
7. FIND THE TOP 5 MOST EXPENSIVE RESTAURANTS THAT OFFER CUISINE OTHER THAN INDIAN CUISINE.
8. FIND THE RESTAURANTS THAT HAVE AN AVERAGE COST WHICH IS HIGHER THAN THE TOTAL AVERAGE COST OF ALL RESTAURANTS TOGETHER.
9. RETRIEVE THE DETAILS OF RESTAURANTS THAT HAVE THE SAME NAME BUT ARE LOCATED IN DIFFERENT CITIES.
10. WHICH RESTAURANT OFFERS THE MOST NUMBER OF ITEMS IN THE 'MAIN COURSE'CATEGORY?
11. LIST THE NAMES OF RESTAURANTS THAT ARE 100% VEGEATARIAN IN ALPHABETICAL ORDER OF RESTAURANT NAME.
12. WHICH IS THE RESTAURANT PROVIDING THE LOWEST AVERAGE PRICE FOR ALL ITEMS? 
13. WHICH TOP 5 RESTAURANT OFFERS HIGHEST NUMBER OF CATEGORIES?
14. WHICH RESTAURANT PROVIDES THE HIGHEST PERCENTAGE OF NON-VEGEATARIAN FOOD?


## Code

For the rest of the code, check the [SQL_queries.sql](https://github.com/Chandan-Sav/SQL_3-.My_SQL./blob/main/Swiggy_Query.sql) file

```sql
-- Create database
CREATE DATABASE IF NOT EXISTS swiggydb;

-- Create table
CREATE TABLE swiggy(
   restaurant_no   INTEGER  NOT NULL,
  restaurant_name VARCHAR(50) NOT NULL,
  city            VARCHAR(9) NOT NULL,
  address         VARCHAR(204),
  rating          NUMERIC(3,1) NOT NULL,
  cost_per_person INTEGER ,
  cuisine         VARCHAR(49) NOT NULL,
  restaurant_link VARCHAR(136) NOT NULL,
  menu_category   VARCHAR(66),
  item            VARCHAR(188),
  price           VARCHAR(12) NOT NULL,
  veg_or_nonveg   VARCHAR(7)
);
```
