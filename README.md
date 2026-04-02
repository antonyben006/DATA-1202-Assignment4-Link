Assignment 4 Report – Data Transformations
Name: Antony Ben | Student ID: 101005963 | Course: Data Analytics, Durham College | Date: March 27, 2026

Assignment 4 code Link: https://antonyben006.github.io/DATA-1202-Assignment4-Link/ 

What I Did

For this assignment, I used the video game sales dataset which we have used for our MySQL classes, to answer the questions, both in Pandas and MySQL through Python.
Before we start with the answers, I initially cleaned the data by dropping the rows where year was missing in order to keep the integrity of the data, and not to ruin further calculations, hence dropped 271 rows.

Question 1:
For this, I split the data into two groups, one before 2005 and one after 2005 and use the mean function to compare the average global sales. 
Pre-2005 came out at 0.6499 million and post-2005 at 0.4894 million which shows that the pre-2005 was higher. 
Then I ran the same logic in MySQL using CASE/WHEN, GROUP BY, and AVG(), to confirm the information, and I got the exact same data.

Question 2:
For this, I applied a lambda function with .apply() to create a new column called “Period” which stores the value for each row as pre-2005 or post-2005. In MySQL, I did the same thing using a CASE WHEN inside a SELECT statement.

Lessons Learned

•	Pandas boolean filtering works analogues to SQL, which is, both filter rows prior to any computation being performed.

•	A lambda in .apply() is Python's version of CASE/WHEN, it’s the same logic, but different syntax.

•	.groupby().mean() in Pandas is the same as GROUP BY with AVG() in SQL.

•	Cleaning null values first is important as dirty data leads to wrong conclusions.

•	Connecting Python to MySQL with mysql-connector-python brought both tools together into one workflow, which made it easy to cross-check results.

