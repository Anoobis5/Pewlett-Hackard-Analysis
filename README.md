# Pewlett-Hackard-Analysis

## Project Overview
The purpose of this project, was to perfom an analysis on a large-scale collection of a company's employe data, to help review staffing based on certain criteria. Pewlett-Hackard wished to review its over 300,000 employees', and determine who may be elegible for retirement. We used postgreSQL to help create data tables to easily organize and visualize employee elegibility. 


## Results:

* Our first step was to create a Retirement Titles table, that could hold all of the titles of current employees who were born between Jan 1, 1952 and Dec 31, 1955 .We needed to determine which employees are elegible for retirement based on age. However, shown in our table below, there are some duplicate names due to the fact that some employees have switched titles over the years.  See the table below:
![retirement_titles](https://user-images.githubusercontent.com/84881187/126879678-5edf309c-bb3e-4164-ad08-227cff20ae2d.PNG)

* So, in order to get a more concise and accurate depiction of elegible unique employees, we created a table using a **DISTINCT ON** statement to show the most recent title for employees of retirement age. Please reference the code for unique_titles and the table example below:
![unique_titles](https://user-images.githubusercontent.com/84881187/126880129-03b360ed-3fa3-49e0-9dc7-f16b2837769f.PNG)

* Our retriement_titles table allows us to see the count of how many employees are elegible for retirement by job title. So, we wrote a query to retrieve the number of employees by their most recent job title who are elegible for retirement. Our analysis shows that of the over 300,000 employees within the company, 90,398 (30.13%) are elegible for retirement. We can see in our analysis that the majority of employees elegible for retirement are those within Senior Staff and Senior Engineer positions. Please see the table below:

![Capture](https://user-images.githubusercontent.com/84881187/126879398-5f07d5f5-abf5-4aa7-b0bc-d1dd3cfe6e5e.PNG)

* The final section of our analysis enables us to see which employees are elegible to participate in the mentorship program. We filtered the data on employees whose birthdates are between Jan 1, 1965 and Dec 31, 1965 across the Employees and Titles tables, we were able to creeate a table named mentorship_eligibility.csv. Our analysis shows that most employees elegible for the mentorship program have senior titles. See an excerpt of the table below:
![mentorship_eligbility](https://user-images.githubusercontent.com/84881187/126880342-bc8b89fa-d57b-428d-930b-9a2c839b5d91.PNG)




## Summary: 

Our task was to help Pewlett-Hackard, by analyzing their employee database to determine how many members of their staff are elegible for retirement to prepare for the "silver tsunami" to come. Our analysis shows that Pewlett-Hackard stand to lose a considerable amount of their workforce to retirement. They will need to potentially fill 90,398 roles, with 57,668 of those positions being Senior position, 2 in Managerial positions, and 4502 Technique Leaders.  The results of our analysis show that a considerable amount of employees will potentially be retiring, with only 1,549 (1.7%) of the retirees being able to apply for the Mentorship Program to help train the next generation of employees. Of those elegible for retirement and elegible for the Mentorship Program, most of the employees elegible for the Mentoship program are Senior Staff members, followed by Engineers. Please see below for a table and the query used to analyze the Mentorship Elegibility spread across Employee Titles:



![employee_mentorship_elegiblity](https://user-images.githubusercontent.com/84881187/126882291-a8f64c97-73c5-4294-a6c3-ef91cb2e0297.PNG)

![elegible_retirement_titles](https://user-images.githubusercontent.com/84881187/126882313-3adb17bd-43f5-46b4-8d49-fb2a2bbceaa3.PNG)



Another variable Pewlett-Hackard will need to consider is not just what kind of staff are elegible for retirement, but also from which departments will they begin to see a draingage of employees. Another refactored analysis shows us the count of each Retirement Elegible staff member from each department. We can see in the table below, that we will see the most significant staff loss in both the Development and Production departments, followed by Sales. Please see below for our query and table on how many employees are elegible for retirement by department:


![dept_retirement_elegiblity](https://user-images.githubusercontent.com/84881187/126882356-d3251bf5-b76d-494c-9025-c3eb7caaeafd.PNG)
![dept_retirement_query](https://user-images.githubusercontent.com/84881187/126882495-4b26405a-ef71-4528-b0a1-aa1690f45b55.PNG)

Pewlwett-Hackard will soon face a "silver tsunami" leaving them with a potential 30% reduction in their total workforce, with only about 1.7% of those elegible for retiring elegible for the Mentorship Program that will traing the next generation of employees. They will need to allocate resources to find suitabale prompotions within with the help of the mentors so continue to see growth within the company. It is advised that Pewlett-Hackard concentrate their efforts in helping regrow their Development and Production departments, as well as their Sales teams. 


