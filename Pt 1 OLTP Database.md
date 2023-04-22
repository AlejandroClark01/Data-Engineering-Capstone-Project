**Task 1 - Create a database.**

Create a database named sales.

**Task 2 - Design a table named sales_data.
Design a table named sales_data based on the sample data given.**

![image](https://user-images.githubusercontent.com/121275064/233768169-c66e53fd-be02-429b-9acd-277b36549c98.png)

Create the sales_data table in sales database.

Take a screenshot of the sql statement you used and the output.

![createtable](https://user-images.githubusercontent.com/121275064/233768188-37f5a591-876f-4c54-8cd9-9c4ef5e89e82.JPG)

**Exercise 3 - Load the Data
Task 3 - Import the data in the file oltpdata.csv**
Download the file oltpdata.csv from https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0321EN-SkillsNetwork/oltp/oltpdata.csv

**Import the data from oltpdata.csv into sales_data table using phpMyAdmin.**

Take a screenshot of the phpMyAdmin import status.

![importdata](https://user-images.githubusercontent.com/121275064/233768218-68bf8487-9906-413a-b459-fc940638ab1b.JPG)

**Task 5. Write a query to find out the count of records in the tables sales_data.**
Take a screenshot of the command you used and the output.

![salesrow](https://user-images.githubusercontent.com/121275064/233768268-4d2740df-f751-46e0-a197-8229b37fe699.JPG)

Exercise 4 - Set up Admin tasks
Task 6 - Create an index
Create an index named ts on the timestamp field.

**Task 7 - List indexes
List indexes on the table sales_data.**

Take a screenshot of the command you used and the output.

![lintindexes](https://user-images.githubusercontent.com/121275064/233768301-f48bb422-0754-4ddd-a813-c3f05e3d036d.JPG)

**Task 8 - Write a bash script to export data.
Write a bash script named datadump.sh that exports all the rows in the sales_data table to a file named sales_data.sql**

Take a screenshot of the contents of the datadump.sh bash file command you used and the output.

![exportdata](https://user-images.githubusercontent.com/121275064/233768345-2d39dd8f-4bae-4af1-93d8-341607fcffe1.JPG)

End of assignment.
