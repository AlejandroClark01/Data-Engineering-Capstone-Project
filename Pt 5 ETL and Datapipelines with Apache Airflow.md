**Prepare the lab environment
Before you start the assignment:**

Step 1: Start MySQL server

Step 2: Create a database named sales

Step 3: Download the file below
https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0321EN-SkillsNetwork/ETL/sales.sql

Step 4: Import the data in the file sales.sql into the sales database.

Step 5: Verify that you can access your cloud instance of IBM DB2 server.

Step 6: Download the mysqlconnect.py python programs from link below.

https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0321EN-SkillsNetwork/ETL/mysqlconnect.py

Step 7: mysqlconnect.py has the sample code to help you understand how to connect to MySQL using Python.

Step 8: Modify mysqlconnect.py suitably and make sure you are able to connect to the MySQL server instance on the Theia environment.

Step 9: Download the db2connect.py python programs from link below.

https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0321EN-SkillsNetwork/ETL/db2connect.py

Step 10: db2connect.py has the sample code to help you understand how to connect to the cloud instance of IBM DB2 using Python.

Step 11: Modify db2connect.py suitably and make sure you are able to connect to your cloud instance of IBM DB2 from the Theia environment.

Step 12: Download the file below

https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0321EN-SkillsNetwork/ETL/sales.csv

Step 13: Load sales.csv into a table named sales_data on your cloud instance of IBM DB2 database.

**Exercise 1 - Automate loading of incremental data into the data warehouse
One of the routine tasks that is carried out around a data warehouse is the extraction of daily new data from the operational database and loading it into the data warehouse. In this exercise you will automate the extraction of incremental data, and loading it into the data warehouse.**
**Task 1 - Implement the function get_last_rowid()
In the program automation.py implement the function get_last_rowid()**
This function must connect to the DB2 data warehouse and return the last rowid.

![get_last_rowid](https://user-images.githubusercontent.com/121275064/233769377-6da41dfc-2fa0-4b11-8549-7c3328b7540a.jpg)

Name the screenshot get_last_rowid.jpg. (Images can be saved with either the .jpg or .png extension.)

**Task 2 - Implement the function get_latest_records()
In the program automation.py implement the function get_latest_records()**
This function must connect to the MySQL database and return all records later than the given last_rowid.
Take a screenshot of the python code clearly showing the implementation of the function get_latest_records().

![get_latest_records](https://user-images.githubusercontent.com/121275064/233769372-2db3256f-7166-48ec-8d9f-2427aad6e791.jpg)

**Task 3 - Implement the function insert_records()
In the program automation.py implement the function insert_records()**
This function must connect to the DB2 data warehouse and insert all the given records.
Take a screenshot of the python code clearly showing the implementation of the function insert_records().

![insertrecords](https://user-images.githubusercontent.com/121275064/233769368-4f2ed82b-a035-4e05-b5ae-83466c54e389.jpg)

**Exercise 1 - Prepare the lab environment
Before you start the assignment:
Start Apache Airflow.
Download the dataset from the source to the destination mentioned below.**
Source : https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0321EN-SkillsNetwork/ETL/accesslog.txt

Destination : /home/project/airflow/dags/capstone

**Exercise 2 - Create a DAG
Task 1 - Define the DAG arguments
Create a DAG with these arguments.**

owner
start_date
email
You may define any suitable additional arguments.

Take a screenshot of the code you used clearly showing the above arguments.

![dag_args](https://user-images.githubusercontent.com/121275064/233769622-d706f908-97f7-4542-b069-5e3ef95e7396.jpg)

**Task 2 - Define the DAG
Create a DAG named process_web_log that runs daily.**

Use suitable description.

Take a screenshot of the code you used to define the DAG.

![dag_definition](https://user-images.githubusercontent.com/121275064/233769627-c9fbaf1e-35a5-43c4-94e9-953dee72038a.jpg)

**Task 3 - Create a task to extract data
Create a task named extract_data.
This task should extract the ipaddress field from the web server log file and save it into a file named extracted_data.txt**

Take a screenshot of the task code.

![extract_data](https://user-images.githubusercontent.com/121275064/233769635-fa26b45d-efef-457d-9c4b-b07267933ccd.jpg)

**Task 4 - Create a task to transform the data in the txt file**
Create a task named transform_data.

This task should filter out all the occurrences of ipaddress “198.46.149.143” from extracted_data.txt and save the output to a file named transformed_data.txt.

Take a screenshot of the task code.

![transform_data](https://user-images.githubusercontent.com/121275064/233769661-d878f872-29d4-4396-8032-90b304eaaa07.jpg)

**Task 5 - Create a task to load the data**
Create a task named load_data.

This task should archive the file transformed_data.txt into a tar file named weblog.tar.

Take a screenshot of the task code.

![load_data](https://user-images.githubusercontent.com/121275064/233769666-1739af73-7cd6-40ed-8cfe-ccffd260487a.jpg)

**Task 6 - Define the task pipeline**
Define the task pipeline as per the details given below:

Task	Functionality
First task	extract_data
Second task	transform_data
Third task	load_data
Take a screenshot of the task pipeline section of the DAG.

![pipeline](https://user-images.githubusercontent.com/121275064/233769674-15ad2027-847b-4167-9872-e573e73ab622.jpg)

**Exercise 3 - Getting the DAG operational.**
Save the DAG you defined into a file named process_web_log.py.

**Task 7 - Submit the DAG**
Take a screenshot of the command you used and the output.

![submit_dag](https://user-images.githubusercontent.com/121275064/233769678-75b9f6aa-b2d7-45e4-b95a-e58da52114c4.jpg)

**Task 8 - Unpause the DAG**
Take a screenshot of the command you used and the output.

![unpause_dag](https://user-images.githubusercontent.com/121275064/233769707-f1c3ce98-e902-4579-9aab-90971a3c2444.jpg)

**Task 9 - Monitor the DAG**
Take a screenshot of the DAG runs for the Airflow console.

![dag_runs](https://user-images.githubusercontent.com/121275064/233769711-ab389422-034e-4e4a-b279-0662a062dfe9.jpg)

End of the assignment.
