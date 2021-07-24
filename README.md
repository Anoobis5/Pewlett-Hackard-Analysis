# Pewlett-Hackard-Analysis

## Project Overview
The purpose of this project, was to perfom an analysis on a large-scale collection of a company's employe data, to help review staffing based on certain criteria. Pewlett-Hackard wished to review its over 300,000 employees', and determine who may be elegible for retirement. We used postgreSQL to help create data tables to easily organize and visualize employee elegibility. 


## Results:

* Our first task was to create a Retirement Titles table, that could hold all of the titles of current employees who were born between Jan 1, 1952 and Dec 31, 1955 .We needed to determine which employees are elegible for retirement based on age. However, shown in our table below, there are some duplicate names due to the fact that some employees have switched titles over the years.  See the table below:
![retirement_titles](https://user-images.githubusercontent.com/84881187/126879678-5edf309c-bb3e-4164-ad08-227cff20ae2d.PNG)

* So, in order to get a more concise and accurate depiction of elegible unique employees, we created a table using a **DISTINCT ON** statement to show the most recent title for employees of retirement age. Please reference the code for unique_titles and the table example below:
![unique_titles](https://user-images.githubusercontent.com/84881187/126880129-03b360ed-3fa3-49e0-9dc7-f16b2837769f.PNG)

* Our retriement_titles table allows us to see the count of how many employees are elegible for retirement by job title. So, we wrote a query to retrieve the number of employees by their most recent job title who are elegible for retirement. Our analysis shows that of the over 300,000 employees within the company, 90,398 (301.13%) are elegible for retirement. Please see the table below:

![Capture](https://user-images.githubusercontent.com/84881187/126879398-5f07d5f5-abf5-4aa7-b0bc-d1dd3cfe6e5e.PNG)

* The final section of our analysis enables us to see which employees are elegible to participate in the mentorship program. We filtered the data on employees whose birthdates are between Jan 1, 1965 and Dec 31, 1965 across the Employees and Titles tables, we were able to creeate a table named mentorship_eligibility.csv. Our analysis shows that most employees elegible for the mentorship program have senior titles. See an excerpt of the table below:
![mentorship_eligbility](https://user-images.githubusercontent.com/84881187/126880342-bc8b89fa-d57b-428d-930b-9a2c839b5d91.PNG)




## Summary: 
Provide high-level responses to the following questions, then provide two additional queries or tables that may provide more insight into the upcoming "silver tsunami."
How many roles will need to be filled as the "silver tsunami" begins to make an impact?
Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?

Our task was to help Pewlett-Hackard, by analyzing their employee database to determine how many members of their staff are elegible for retirement to prepare for the "silver tsunami" to come. 
