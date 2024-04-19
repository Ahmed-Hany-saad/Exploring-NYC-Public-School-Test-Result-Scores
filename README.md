# NYC Schools SAT Performance Analysis README

## Overview
This project provides a Python script to analyze the SAT performance of schools in New York City. The analysis focuses on determining the best schools based on SAT math scores, the top 10 performing schools based on total SAT scores, and the borough with the highest standard deviation for total SAT scores.

## Dependencies
- Python 3.x
- pandas

## Dataset
The dataset, `schools.csv`, should contain the following columns:
- school_name: Name of the school.
- average_math: Average SAT math score for the school.
- average_reading: Average SAT reading score for the school.
- average_writing: Average SAT writing score for the school.
- borough: The borough in which the school is located.

The dataset should be placed in the root directory of the project.

## Usage

1. Place the `schools.csv` data file in the root directory.
2. Run the script. The script will:
   - Read the data.
   - Determine the best schools for math.
   - Calculate the total SAT score for each school.
   - Identify the top 10 performing schools based on the total SAT score.
   - Determine which NYC borough has the highest standard deviation for total SAT scores.
3. Analyze the results.

## The Goal is answer this questions :
1. Which NYC schools have the best math results?
   - The best math results are at least 80% of the *maximum possible score of 800* for math. Save your results in a pandas DataFrame called best_math_schools, including "school_name" and "average_math" columns, sorted by "average_math" in descending order.

2. What are the top 10 performing schools based on the combined SAT scores?
   - Save your results as a pandas DataFrame called top_10_schools containing the "school_name" and a new column named "total_SAT", with results ordered by "total_SAT" in descending order.

3.Which single borough has the largest standard deviation in the combined SAT score?
   - Save your results as a pandas DataFrame called largest_std_dev.
   - The DataFrame should contain one row, with:
        - "borough" - the name of the NYC borough with the largest standard deviation of "total_SAT".
        - "num_schools" - the number of schools in the borough.
        - "average_SAT" - the mean of "total_SAT".
        - "std_SAT" - the standard deviation of "total_SAT".
   - Round all numeric values to two decimal places.

## Analysis Results

- `best_math_schools`: A DataFrame containing schools with an average math score of 640 or higher, sorted in descending order.
- `top_10_schools`: A DataFrame containing the top 10 schools based on the mean total SAT score.
- `largest_std_dev`: A DataFrame containing the borough with the highest standard deviation for total SAT scores.

