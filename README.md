# AWS DynamoDB Data Import & Query Project
 Overview
This project demonstrates a complete workflow of working with Amazon DynamoDB, including data migration, querying, and global replication using AWS services.
The implementation covers:
Uploading structured JSON data to Amazon S3
Importing data into DynamoDB
Verifying records
Querying using PartiQL
Configuring Global Table replication
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
This project showcases real-world cloud data handling and scalable NoSQL database operations.
 Objectives
Understand DynamoDB data import workflow
Learn integration between Amazon S3 and DynamoDB
Execute SQL-like queries using PartiQL
Implement multi-region replication using Global Tables
🛠️ Technologies Used
Amazon S3
Amazon DynamoDB
AWS Console
PartiQL (SQL-compatible query language)
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
⚙️ Project Workflow
1️⃣ Upload JSON File to Amazon S3
Created a structured JSON file (Mydb.json)
Uploaded it to an S3 bucket
S3 acts as a secure and durable storage layer
2️⃣ Import Data from S3 to DynamoDB
Used DynamoDB “Import from S3” feature
Defined schema with UserId as Partition Key
Automated bulk data import without manual entry
3️⃣ Verify Imported Data
Checked records using “Explore Table Items”
Confirmed successful import and correct schema mapping
4️⃣ Query Data using PartiQL
Used DynamoDB PartiQL editor
Executed SQL-like queries (e.g., filtering by Age)
Enabled easy and flexible data retrieval
5️⃣ Create Global Table Replica
Configured replication between regions (e.g., Oregon & Mumbai)
Verified both regions show Active status
Ensured high availability and fault tolerance
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
 Screenshots & Detailed Explanation
 Screenshot 1: Uploading JSON File to Amazon S3
Shows successful upload of the JSON dataset into an S3 bucket.
Brief Explanation:
The dataset file is uploaded to S3, acting as the source for DynamoDB import.
Detailed Description:
The file Mydb.json is visible in the S3 bucket
Confirms successful upload from local system to cloud
S3 ensures high durability and acts as an intermediary storage layer
Commonly used in real-world pipelines for staging data
<img width="1917" height="1023" alt="3rd ss" src="https://github.com/user-attachments/assets/f566eb5d-e023-4bd3-a1c6-47ec003ba6ea" />
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
Screenshot 2: Importing Data from S3 into DynamoDB
Displays the DynamoDB import configuration page with schema setup.
Brief Explanation:
Data is imported into DynamoDB using the S3 file with defined table schema.
Detailed Description:
S3 file is selected as input source
Table schema is configured with UserId as Partition Key
AWS handles automatic parsing and insertion
Eliminates manual data entry and reduces errors
<img width="1916" height="1023" alt="4th ss" src="https://github.com/user-attachments/assets/352bebc9-c878-4c68-8c00-9ad4bf111eb2" />
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
Screenshot 3: Verifying Records in DynamoDB
Shows the table items view confirming successful data import.
Brief Explanation:
Imported records are displayed in DynamoDB for validation.
Detailed Description:
Displays all inserted records (e.g., 5 items)
Confirms data integrity and correct attribute mapping
Provides a quick UI-based validation method
Useful for debugging and verification
<img width="1908" height="1026" alt="8th ss" src="https://github.com/user-attachments/assets/5d766ce7-d55d-428a-9ec9-873cba2fcee7" />
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
Screensht 4: Query Execution using PartiQL
Shows execution of a SELECT query in DynamoDB using PartiQL.
Brief Explanation:
SQL-like queries are executed on DynamoDB using PartiQL.
Detailed Description:
Query example: filtering users based on Age = 21
Enables structured querying on NoSQL data
Simplifies data access for developers familiar with SQL
Supports filtering, projection, and conditions
<img width="1917" height="1023" alt="9th ss" src="https://github.com/user-attachments/assets/92bf3cbe-a9ea-40b1-b9f9-7ef5ebef9d5a" />
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
Screenshot 5: Global Table Replica Configuration
Displays active multi-region replication setup.
Brief Explanation:
DynamoDB table is replicated across multiple AWS regions.
Detailed Description:
Shows regions like Oregon and Mumbai
Both regions display Active status
Ensures real-time data synchronization
Improves availability, fault tolerance, and performance for global users
<img width="1917" height="1017" alt="11th ss" src="https://github.com/user-attachments/assets/54a2d573-f158-4476-b4a6-732a67fcb9ce" />
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
Key Learnings-
Efficient data transfer between AWS services
Hands-on experience with DynamoDB operations
Understanding of NoSQL querying using PartiQL
Implementation of globally distributed databases
Real-World Applications-
E-commerce platforms (global inventory systems)
Social media applications (real-time data sync)
Financial systems requiring high availability
Cloud-native scalable applications
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
Project Structure-
AWS-DynamoDB-Project/
│── README.md
│── WORKING WITH DynamoDB IN AWS.pptx
│── images/
│   ├── s3_upload.png
│   ├── dynamodb_import.png
│   ├── dynamodb_verify.png
│   ├── partiql_query.png
│   └── global_table.png
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
Conclusion
This project demonstrates a complete end-to-end AWS data workflow, from storage to querying and global replication. It highlights how DynamoDB integrates with other AWS services to build scalable, reliable, and high-performance applications.
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
 Project Structure
