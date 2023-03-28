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

A screenshot depicts the name and type of each column. The "grade" column is of type object.

In the grade column, remove the "th" suffix from every value by using str and replace, as the following image shows:

A screenshot depicts the "grade" column without the "th" suffixes.

Change the "grade" column to the int type, and then verify the column types, as the following image shows:

A screenshot depicts each column name and type. The "grade" column has a type of int64.

Deliverable 3: Summarize the Data
Generate the summary statistics for the student DataFrame by using the describe function, as the following image shows:

A screenshot depicts the summary statistics.

Display the mean math score by using the mean function.

Store the minimum reading score in min_reading_score.

Deliverable 4: Drill Down into the Data
Display the grade column by using loc, as the following image shows:

A screenshot depicts the "grade" column.

Display the first three rows of Columns 3, 4, and 5 by using iloc, as the following image shows:

A screenshot depicts the first three rows of the "school_name", "reading_score", and "math_score" columns.

Select the rows for Grade 9, and display their summary statistics by using loc and describe, as the following image shows:

A screenshot depicts the summary statistics for Grade 9.

Store the row with the minimum overall reading score in min_reading_row by using loc and the min_reading_score variable from Deliverable 3, as the following image shows:

A screenshot depicts Row 3706.

Select all the reading scores from the 10th graders at Dixon High School by using loc with conditionals, as the following image shows:

A screenshot depicts a "school_name" column with "Dixon High School" in each row and a corresponding "reading_score" column.

Find the mean reading score for all the students in Grades 11 and 12 combined by using conditional statements and loc or iloc.

Deliverable 5: Compare the Data
Display the average budget for each school type by using the groupby and mean functions, as the following image shows:

A screenshot depicts the average budget for charter schools and for public schools.

Find the total number of students at each school, and sort those numbers from largest to smallest by using the groupby, count, and sort_values functions, as the following image shows:

A screenshot depicts the total number of students at each school in descending order.

Find the average math score by grade for each school type by using the groupby and mean functions, as the following image shows:

A screenshot depicts the average math score for each grade, separated by school type.

Deliverable 6: Report Findings
Using the provided cell, write a brief summary of your findings as follows: Write a few sentences to describe any discoveries that you made while performing your analysis. Include any additional analysis that you believe would be worthwhile. School_District_Analysis
