# Writing Functions for Product Analysis
## Description
Have you ever started your data analysis and ended up with repetitive code? Repetitive code is a sign that functions are needed. Functions help keep our code flexible, maintainable, and interpretable.

Our colleague Brenda, a product analyst, has written a script to pull Net Promotor Score (NPS) survey data from multiple sources to calculate the NPS score. This code works well, but it violates coding best practices, including Don't Repeat Yourself (DRY). Let's take a look at her code and write some functions for Brenda! 
## Contents
1. **DRY: Don't repeat yourself:** Write a function that takes an NPS CSV file and the source type to create a DataFrame with a column specifying the source type.
2. **Verifying the files with the "with" keyword:** Write a function to check if a CSV file has these three columns: `response_date`, `user_id`, and `nps_rating`.
3. **Putting it together with nested functions:** Write a function that uses `check_csv()` and `convert_csv_to_df()` to convert valid files into DataFrames and combines the resulting DataFrames into one DataFrame.
4. **Detractors, Passives, and Promoters:** Write a function `categorize_nps` that classifies a rating, `x`, into one of four categories: detractor, passives, promoters, and invalid.
5. **Applying our function to a DataFrame:** Write a new line of code to `convert_csv_to_df()` so that there is a column for each rating's NPS category.
6. **Calculating the Net Promoter Score:** Write a new function called `calculate_nps()` that calculates the NPS score of a DataFrame with the column `nps_group`.
7. **Breaking down NPS by source:** Write a function that calculates the individual NPS score for each source type in the column `source`.
8. **Adding docstrings:** Add docstrings to the functions: `combine_nps_csvs()`, `calculate_nps()`, and `calculate_nps_by_source()`.
