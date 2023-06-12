# WeRateDogs' Tweets Analysis
<div align='center'> 
    <img src="https://github.com/Bright136/Wrangling_a_datset_project-Udacity-Data-Analyst-Nanodegree-/blob/master/images/dogs%20(1).jpg"/>

</div>

## Introduction
> This project was submitted as project two for Udacity's Data Analyst Nanodegree program.
The goal of this Project is to wrangle WeRateDogs Twitter data to create interesting and 
trustworthy analyses and visualizations. WeRateDogs is a Twitter account that rates people’s 
dog in a humorous way. The steps taken to complete this project were: Gathering data, 
Assessing data, Cleaning data, Storing data and Analysing and visualizing data and reporting.
Gathering Data

> The data used for this project was gathered from three datasets, namely the 
twitter_acrhive_enhanced.csv, image_prediction.tsv which was downloaded 
programmatically from one of Udacity’s servers and a text-json.txt which was originaly suppose to be downloaded from twitter using the tweepy library. 

## Gather
>- Enhanced Twitter Archive data contains basic tweet data given by Udacity.
>- text-json.txt contains retweet count and favorite count.
>- Image Predictions File, containing the predicted breeds of dogs given by Udacity.

## Data Wrangling

### Packages/Libraries
> These libraries were used in the project.
>- pandas
>- NumPy
>- requests
>- json
>- datetime
>- matplotlib
>- seaborn

> Using Pandas all the files were read into a DataFrame. The first two file were read directly with exception of the text-json.txt which had its individual lines read as JSON and then converted into a DataFrame.

## Assessing data
> The datasets were assessed programmatically and visually. Here are some quality and tidy 
issues associated with them. 

#### Quality issues
>- There are missing values in in_reply_to_status_id, in_reply_to_user_id, 
retweeted_status_id, retweeted_status_user_id columns
>- Wrong rating numerators and rating denominators
>- The timestamp column had a wrong datatype.

#### Tidy
>- doggo, floffer, pupper and puppo columns should collapsed into a single column since 
they are rather observations
>- The three dog prediction algorithms (p1, p2, p3) should be collapsed into a single 
column.


## Cleaning data
The quality and tidy issues were cleaned programmatically using the Define-Code-Test 
format.
>- Define: convert the assessments into defined cleaning tasks.
>- Code: convert those definitions to code and run that code.
>- Test: test your dataset, visually or with code, to make sure cleaning operations worked.


## Storing data
The datasets were merged into a one DataFrame and stored as twitter_archive_master.csv. 


## Analysis
> The  following questions were used in the analysis.

>- Which breed had the highest average rating, favorite count and retweet count?
>- Do dogs with higher ratings have higher retweets counts?
>- Do dogs with higher ratings have higher favorite counts?
>- What are the top 10 most tweeted breeds.
>- What is the relationship between retweet_count and favorite_count?
>- What was the highest rating attained by a dog and what was the impact of the 
number of images on the retweet and favorite counts on high rated dogs?


## Deliveries
#### Notebooks
>- The analysis is found in the wrangle_act.ipynb nootebook
>- [Wrangle Report](https://github.com/Bright136/Wrangling_a_datset_project-Udacity-Data-Analyst-Nanodegree-/blob/master/wrangle_act.ipynb )

#### Wrangle Report
>  A summary of the project was documented in wrangle_report.pdf file. 

>- [Wrangle Report](https://github.com/Bright136/Wrangling_a_datset_project-Udacity-Data-Analyst-Nanodegree-/blob/master/reports/wrangle_report.pdf)

#### Act Report
> The insights communicated were also docummented in the act_report.pdf file.
>- [Act Report](https://github.com/Bright136/Wrangling_a_datset_project-Udacity-Data-Analyst-Nanodegree-/blob/master/reports/act_report.pdf)


#### A Photo of Atticus, the most rated dog by WeRateDogs

<div align='center'> 
    <img src="https://github.com/Bright136/Wrangling_a_datset_project-Udacity-Data-Analyst-Nanodegree-/blob/master/images/Aticus.jpg"/>

</div>





