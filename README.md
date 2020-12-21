# School_District_Analysis
Analysis using Python

## Overview of Project
**Analyze school disctrict data on student funding and student standardized test scores to show trends and schools performance. The analysis and findings will be used by the school board to make strategic decisions regarding the school budget and priorities**

**The Analysis should include the following information:** 

1. Perform data cleaning to exclude reading and math grades for Thomas High School ninth graders due to possible academic dishonesty (records appear to have been altered)
A  High-level snapshot of the district's key metrics, presented in a table format 
2. An overview of the key metrics for each school, presented in a table format

**The analysis report will include tables presenting each of the following metrics:**

- Top 5 and bottom 5 performing schools, based on the overall passing rate
- The average math score received by students in each grade level at each school
- The average reading score received by students in each grade level at each school
- School performance based on the budget per student
- School performance based on the school size 
- School performance based on the type of school

## Resources
- Data Source: [schools_complete.csv](Resources/schools_complete.csv); [students_complete.csv](Resources/students_complete.csv)
- Source Code: [PyCitySchools_Challenge](PyCitySchools_Challenge.ipynb)
- Software: Python 3.7.9 64-bit (conda); jupyter-notebook : 6.1.4

## Summary
- #### *Note: Updated data analysis was performed on cleaned data set (reading and math grades for Thomas High School ninth graders were replaced with NaNs to account for data issues and excluded from aggregate calculations)*

- Code Example:

        # Step 2. Use the loc method on the student_data_df to select all the reading scores from the 9th grade at Thomas High School and replace them with NaN.
        student_data_df.loc[(student_data_df["grade"]=="9th")&(student_data_df["school_name"]=="Thomas High School"),"reading_score"]=np.nan
        student_data_df
        
![Scores_replaced_wNaN](Resources/Scores_replaced_wNaN.png)

- **The district summary DataFrame**
![district_summary_df](Resources/district_summary_df.png)

- **The school summary DataFrame**
![School_summary_df](Resources/School_summary_df.png)

- **The top 5 performing schools, based on the overall passing rate**
![High_performing_schools](Resources/High_performing_schools.png)

- **The bottom 5 performing schools, based on the overall passing rate**
![Low_performing_schools](Resources/Low_performing_schools.png)


- **The average math score for each grade level from each school**

![Math_average_scores_per_grade_by_school](Resources/Math_average_scores_per_grade_by_school.png)


- **The average reading score for each grade level from each school**

![Reading_average_scores_per_grade_by_school](Resources/Reading_average_scores_per_grade_by_school.png)


- **The scores by school spending per student**

![Scores_by_school_spending](Resources/Scores_by_school_spending.png)


- **The scores by school size**

![Scores_by_school_size](Resources/Scores_by_school_size.png)


- **The scores by school type**

![Scores_by_school_type](Resources/Scores_by_school_type.png)


## Results
- *How is the district summary affected?*
- *How is the school summary affected?*
- *How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?*

- **How does replacing the ninth-grade scores affect the following:**

- *Math and reading scores by grade*
- *Scores by school spending*
- *Scores by school size*
- *Scores by school type*
    
### School District Data Analysis Summary:
The four major changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.



