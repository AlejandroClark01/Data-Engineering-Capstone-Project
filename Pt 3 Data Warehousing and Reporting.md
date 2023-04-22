**Exercise 1 - Design a Data Warehouse
The ecommerce company has provied you the sample data.**

You will start your project by designing a Star Schema for the warehouse by identifying the columns for the various dimension and fact tables in the schema. Name your database as softcart

**Task 1 - Design the dimension table softcartDimDate
Using the ERD design tool design the table softcartDimDate. The company is looking at a granularity of a day. Which means they would like to have the ability to generate the report on yearly, monthly, daily, and weekday basis.**

Here is a partial list of fields to serve as an example:

dateid

month

monthname

…

…

Take a screenshot of the table softcartDimDate in the ERD tool clearly showing all the fieldnames and data types.

![softcartDimDate](https://user-images.githubusercontent.com/121275064/233768873-78c8b67d-e518-41a2-a976-f68b92072b67.jpg)

**Task 2 - Design the dimension table softcartDimCategory
Using the ERD design tool design the table softcartDimCategory.**

**Task 3 - Design the dimension table softcartDimItem
Using the ERD design tool design the table softcartDimItem.**

**Task 4 - Design the dimension table softcartDimCountry
Using the ERD design tool design the table softcartDimCountry.**

![dimtables](https://user-images.githubusercontent.com/121275064/233768890-da4ca066-2d7f-4331-970a-4fcfbc660eca.jpg)

**Task 5 - Design the fact table softcartFactSales
Using the ERD design tool design the table softcartFactSales.**
Take a screenshot of the table softcartFactSales in the ERD tool clearly showing all the fieldnames and data types.

![softcartFactSales](https://user-images.githubusercontent.com/121275064/233768906-1e6e8204-e6a6-44af-a494-9b3ce58ebbca.jpg)

**Task 6 - Design the relationships
Using the ERD design tool design the required relationships(one-to-one, one-to-many etc) amongst the tables.**
Take a screenshot of the entire ERD clearly showing all the relationships amongst the tables.

![softcartRelationships](https://user-images.githubusercontent.com/121275064/233768915-19047b2c-aaf5-4d9a-9290-c7e837e5f679.jpg)

**Exercise 2 - Create the schema
In this exercise you will create the schema of the data warehouse.**

**Task 7 - Create the schema.**
Download the schema sql from ERD tool and create the schema in a database named staging.
Take a screenshot showing the success of the schema creation.

![createschema](https://user-images.githubusercontent.com/121275064/233768924-13a09261-0788-4132-82be-95b96c72b1d2.jpg)

End of the assignment.

**Exercise 1 - Load data into the Data Warehouse
In this exercise you will load the data into the tables.**
You will load the data provided by the company in csv format.

**Task 1 - Load data into the dimension table DimDate**
Download the data from this link
Load this data into DimDate table.
Take a screenshot of the first 5 rows in the table DimDate.

![DimDate](https://user-images.githubusercontent.com/121275064/233769123-b28607fe-9bb5-4c6d-bb58-48099b8fa556.jpg)

**Task 2 - Load data into the dimension table DimCategory**
Download the data from this link
Load this data into DimCategory table.
Take a screenshot of the first 5 rows in the table DimCategory.

![DimCategory](https://user-images.githubusercontent.com/121275064/233769129-3f28546f-2f3a-40c3-a7f9-62b097971624.jpg)

**Task 3 - Load data into the dimension table DimCountry**
Download the data from this link
Load this data into DimCountry table.
Take a screenshot of the first 5 rows in the table DimCountry.

![DimCountry](https://user-images.githubusercontent.com/121275064/233769136-cbe6e57d-5a0c-41f9-9da8-0706b594b193.jpg)

**Task 4 - Load data into the fact table FactSales**
Download the data from this link
Load this data into FactSales table.
Take a screenshot of the first 5 rows in the table FactSales.

![DimCountry](https://user-images.githubusercontent.com/121275064/233769139-6c849a58-9cb1-4ec5-97f7-2cdc5165adaa.jpg)

**Exercise 2 - Queries for data analytics
In this exercise you will query the data you have loaded in the previous exercise.**

**Task 5 - Create a grouping sets query**
Create a grouping sets query using the columns country, category, totalsales.
Take a screenshot of the sql and the output rows.

![groupingsets](https://user-images.githubusercontent.com/121275064/233769088-1f1d7c70-72e8-41c4-854e-e660e10b75b8.jpg)

**Task 6 - Create a rollup query**
Create a rollup query using the columns year, country, and totalsales.
Take a screenshot of the sql and the output rows.

![rollup](https://user-images.githubusercontent.com/121275064/233769070-a50d7bd8-69f5-48bf-b437-d149f40eaa40.jpg)

**Task 7 - Create a cube query**
Create a cube query using the columns year, country, and average sales.
Take a screenshot of the sql and the output rows.

![cube](https://user-images.githubusercontent.com/121275064/233769109-7d716538-13e3-469e-aaf9-d3b530edc68f.jpg)

**Task 8 - Create an MQT**
Create an MQT named total_sales_per_country that has the columns country and total_sales.
Take a screenshot of the sql.

![mqt](https://user-images.githubusercontent.com/121275064/233769051-2c11049d-0567-453a-9710-98fa1099860b.jpg)

End of the assignment.
