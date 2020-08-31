# Analyzing a drug-treatment study using Matplotlib and Pandas 

## Background

In this assignment, I analyze data resulting from an animal study for a company called Pymaceuticals Inc. This company specializes in anti-cancer pharmaceuticals. In its most recent efforts, it began screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer.

In this study, 250 mice identified with SCC tumor growth were treated through a variety of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals' drug of interest, Capomulin, versus the other treatment regimens.

## Analysis

* Generated a statistical summary table consisting of the mean, median, variance, standard deviation, and SEM of the tumor volume for each drug regimen
   * **STEPS**
    1) Imported both CSV files and stored into dataframes via Pandas
    2) Merged both dataframes
    3) Grouped dataframes by Drug Regimine and used statistical functions to create the summary table
    
![](/images/summary_table.jpg)

* Created a bar chart using both Pandas and Matplotlib showcasing the number of data points for each treatment regimen

<img src="/images/drug_regimen_counts.jpg" width="600" height="400">

* Generated a pie chart showcasing the distribution of mice by sex

<img src="/images/distribution_by_sex.jpg" width="600" height="400">

* Created a box and whisker plot of the final tumor volume for all four treatment regiments. 
   * **STEPS**
    1) Filtered the dataset where timepoint equals the max timepoint
    2) Grouped the dataframe by drug regimen and mouse id.
    3) Created seperate dataframes for each drug regimen
    4) Created a function to calculate quartiles and Inter-Quartile Range
    5) Created a function that checks for outliers
    6) Plot the box and whisker using Matplot Lib
    
<img src="/images/final_tumor_vol.jpg" width="600" height="400">

* Created a scatter plot of mouse weight versus average tumor volume for the Capomulin treatment regimen. Also calculated the correlation coefficient.

<img src="/images/weight_vs_vol.jpg" width="600" height="400">
