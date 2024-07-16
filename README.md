# pandas-challenge
# PyCitySchools Analysis

## Overview

This project involved using Pandas DataFrames to analyze school and standardized test data for a city school district. The goal was to help the school board and mayor make strategic decisions regarding future school budgets and priorities based on district-wide standardized test results.

## Background

As the Chief Data Scientist for the city's school district, the task was to aggregate and analyze data to showcase trends in school performance. The analysis included every student's math and reading scores, as well as various information about the schools they attended.

## Project Setup

1. A new repository called `pandas-challenge` was created.
2. The repository was cloned to a local machine.
3. Inside the local Git repository, a folder named `PyCitySchools` was created.
4. A Jupyter notebook was added to this folder, serving as the main script for analysis.
5. These changes were pushed to GitHub.

## Files

The necessary files were downloaded to begin the analysis.

## Analysis Steps

Using Pandas and Jupyter Notebook, a report was created that included the following data:

### District Summary

Performed calculations to create a high-level snapshot of the district's key metrics in a DataFrame. This included:

- Total number of unique schools
- Total students
- Total budget
- Average math score
- Average reading score
- % passing math
- % passing reading
- % overall passing

### School Summary

Performed calculations to create a DataFrame summarizing key metrics about each school. This included:

- School name
- School type
- Total students
- Total school budget
- Per student budget
- Average math score
- Average reading score
- % passing math
- % passing reading
- % overall passing

### Highest-Performing Schools (by % Overall Passing)

Sorted the schools by % Overall Passing in descending order and displayed the top 5 rows in a DataFrame called `top_schools`.

### Lowest-Performing Schools (by % Overall Passing)

Sorted the schools by % Overall Passing in ascending order and displayed the top 5 rows in a DataFrame called `bottom_schools`.

### Math Scores by Grade

Performed calculations to create a DataFrame listing the average math score for students of each grade level (9th, 10th, 11th, 12th) at each school.

### Reading Scores by Grade

Created a DataFrame listing the average reading score for students of each grade level (9th, 10th, 11th, 12th) at each school.

### Scores by School Spending

Created a table breaking down school performance based on average spending ranges (per student). Four bins were created to group school spending and `pd.cut` was used to categorize spending based on these bins. Mean scores per spending range were calculated and included in a DataFrame called `spending_summary`.

### Scores by School Size

Binned the `per_school_summary` DataFrame by school size and created a DataFrame called `size_summary` that broke down school performance based on school size (small, medium, or large).

### Scores by School Type

Grouped the `per_school_summary` DataFrame by "School Type" and averaged the results. A new DataFrame called `type_summary` was created to show school performance based on the "School Type".

## Conclusion

The analysis revealed several trends, including:
- Higher spending per student did not necessarily correlate with better performance.
- Smaller schools tended to perform better than larger schools.
- Charter schools consistently outperformed district schools across all metrics.

These findings provide valuable insights for making strategic decisions regarding school budgets and priorities.
