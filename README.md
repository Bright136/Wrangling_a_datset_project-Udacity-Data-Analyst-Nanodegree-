# WeRateDogs' Tweets Analysis

<div align='center'> 
    <img src="https://github.com/Bright136/Wrangling_a_datset_project-Udacity-Data-Analyst-Nanodegree-/blob/master/images/dogs%20(1).jpg"/>
</div>

## Introduction
This project was submitted as project two for Udacity's Data Analyst Nanodegree program. The goal of this project is to wrangle WeRateDogs Twitter data to create interesting and trustworthy analyses and visualizations. WeRateDogs is a Twitter account that rates people's dogs in a humorous way. The steps taken to complete this project were gathering data, assessing data, cleaning data, storing data, and analyzing and visualizing data.

## Gather
The data used for this project was gathered from three datasets:

- **Enhanced Twitter Archive**: This dataset contains basic tweet data given by Udacity.
- **text-json.txt**: This file contains retweet count and favorite count for each tweet.
- **Image Predictions File**: This file contains the predicted breeds of dogs for each tweet, given by Udacity.

## Data Wrangling

### Packages/Libraries
The following libraries were used in the project:

- pandas
- NumPy
- requests
- json
- datetime
- matplotlib
- seaborn

These libraries were used to read the files into DataFrames and perform various data wrangling tasks.

## Assessing Data
The datasets were assessed programmatically and visually. Several quality and tidy issues were identified during the assessment.

### Quality Issues
- There are missing values in columns such as `in_reply_to_status_id`, `in_reply_to_user_id`, `retweeted_status_id`, and `retweeted_status_user_id`.
- There are wrong rating numerators and denominators.
- The `timestamp` column has the wrong datatype.

### Tidy Issues
- The `doggo`, `floffer`, `pupper`, and `puppo` columns should be collapsed into a single column since they represent different observations.
- The three dog prediction algorithms (`p1`, `p2`, `p3`) should be collapsed into a single column.

## Cleaning Data
The identified quality and tidy issues were cleaned programmatically using the Define-Code-Test format:
- Define: Convert the assessments into defined cleaning tasks.
- Code: Convert those definitions into code and run that code.
- Test: Test the dataset, visually or with code, to ensure that the cleaning operations worked.

## Storing Data
The datasets were merged into a single DataFrame and stored as `twitter_archive_master.csv`.

## Analysis
The following questions were used in the analysis:
- Which breed had the highest average rating, favorite count, and retweet count?
- Do dogs with higher ratings have higher retweet counts?
- Do dogs with higher ratings have higher favorite counts?
- What are the top 10 most tweeted breeds?
- What is the relationship between retweet count and favorite count?
- What was the highest rating attained by a dog, and what was the impact of the number of images on the retweet and favorite counts of highly rated dogs?

## Deliverables
### Notebooks
- The analysis is found in the `wrangle_act.ipynb` notebook: [Wrangle Act Notebook](https://github.com/Bright136/Wrangling_a_datset_project-Udacity-Data-Analyst-Nanodegree-/blob/master/wrangle_act.ipynb)

### Reports
- Wrangle Report: A summary of the project was documented in the `wrangle_report.pdf` file: [Wrangle Report](https://github.com/Bright136/Wrangling_a_datset_project-Udacity-Data-Analyst-Nanodegree-/blob/master/reports/w