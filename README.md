Overview

Maria has gotten a new version of the student data with several changes. This includes an additional column: "school budget". She wants you to rework part of your analysis by using the new dataset.

What You're Creating
This new assignment consists of five technical analysis deliverables and a written report to deliver the results. You will submit the following deliverables:

Deliverable 1: Collect the student data into a DataFrame.

Deliverable 2: Prepare a cleaned version of the DataFrame.

Deliverable 3: Summarize key pieces of the data.

Deliverable 4: Drill down into the data to analyze specific subsets.

Deliverable 5: Compare and contrast the data through grouping and aggregation functions.

Deliverable 6: A written analysis of your results (README.md).

Files

Instructions
Deliverable 1: Collect the Data
Import the data from the new_full_student_data.csv file into a DataFrame named student_df by using the Pandas read_csv function and the os module.

Confirm that Pandas correctly imported the data by using the head function, as the following image shows:

![image](https://user-images.githubusercontent.com/119356389/228350121-1630a7dc-77d8-403d-b34a-e16990b8c1e7.png)

Deliverable 2: Prepare the Data
In the student DataFrame, check for rows that have NaN (or missing) values, and remove those rows, as the following image shows:

A screenshot depicts each column name with a zero.

In the student DataFrame, check for duplicate rows, and remove them.

Check the data types of the columns by using the dtypes property, as the following image shows:
![image](https://user-images.githubusercontent.com/119356389/228365080-ce6de1d9-d720-4d5c-85c3-4bb246e7380a.png)

A screenshot depicts the name and type of each column. The "grade" column is of type object.
![image](https://user-images.githubusercontent.com/119356389/228365239-3765d5b3-831c-4a07-9271-906f478c3cde.png)


In the grade column, remove the "th" suffix from every value by using str and replace, as the following image shows:

A screenshot depicts the "grade" column without the "th" suffixes.

Change the "grade" column to the int type, and then verify the column types, as the following image shows:

A screenshot depicts each column name and type. The "grade" column has a type of int64.
![image](https://user-images.githubusercontent.com/119356389/228365351-aeb5178c-4913-4772-84c1-aea34d7d5e25.png)

Deliverable 3: Summarize the Data
Generate the summary statistics for the student DataFrame by using the describe function, as the following image shows:

A screenshot depicts the summary statistics.

Display the mean math score by using the mean function.

Store the minimum reading score in min_reading_score.

Deliverable 4: Drill Down into the Data
Display the grade column by using loc, as the following image shows:

A screenshot depicts the "grade" column.

Display the first three rows of Columns 3, 4, and 5 by using iloc, as the following image shows:

![image](https://user-images.githubusercontent.com/119356389/228365601-8b7a03a0-a8fa-40b0-bff8-cd42cf8cce18.png)

Select the rows for Grade 9, and display their summary statistics by using loc and describe, as the following image shows:


Store the row with the minimum overall reading score in min_reading_row by using loc and the min_reading_score variable from Deliverable 3, as the following image shows:

![image](https://user-images.githubusercontent.com/119356389/228365737-c8e23a66-03d4-42ec-87e8-d22f08f89d43.png)

Select all the reading scores from the 10th graders at Dixon High School by using loc with conditionals, as the following image shows:

![image](https://user-images.githubusercontent.com/119356389/228365974-e0c59da8-32e6-4e6b-9098-44ca6a6ed381.png)

Find the mean reading score for all the students in Grades 11 and 12 combined by using conditional statements and loc or iloc.

Deliverable 5: Compare the Data
Display the average budget for each school type by using the groupby and mean functions, as the following image shows:

![image](https://user-images.githubusercontent.com/119356389/228366104-e4886029-8800-492f-9b97-1fd5db7130aa.png)

Find the total number of students at each school, and sort those numbers from largest to smallest by using the groupby, count, and sort_values functions, as the following image shows:

![image](https://user-images.githubusercontent.com/119356389/228366220-a0f319dc-f9c8-43ee-adc2-101d5a6f2b37.png)

Find the average math score by grade for each school type by using the groupby and mean functions, as the following image shows:

![image](https://user-images.githubusercontent.com/119356389/228366339-c5d1ccd9-d2ab-4dc8-b770-e58085b6f528.png)

Deliverable 6: Report Findings
Using the provided cell, write a brief summary of your findings as follows: Write a few sentences to describe any discoveries that you made while performing your analysis. Include any additional analysis that you believe would be worthwhile. School_District_Analysis
