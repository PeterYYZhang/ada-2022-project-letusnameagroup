# Trends in the American Beer Market: How can we help the declining beer styles to revive?


## Date story website
To learn more about our work, please visit our webpage[Let us make the most popular beer🍺!](https://letusmakepopularbeer.streamlit.app/).

## Abstract
In this task, we aim to find out what is the trend in the **American beer market** as well as specified to specific regions. We will utilize statistical and time series modeling to analyze the trends and make some predictions, and employ sentiment analysis and natural language processing techniques to analyze consumer comments. Through this analysis, we aim to identify key trends in consumer preferences for different beer styles and understand how these preferences have evolved over time. Our findings will provide valuable insights for breweries and marketers in the industry seeking to better understand the changing preferences of beer drinkers.

## Introduction
Beer is one of the oldest beverages in the world. With the progress of brewing technology,
many new brands and styles have been created. Meanwhile, a proportion of breweries are still
trying to preserve their traditional brewing techniques.
As a significant beer consumer, the United States plays a crucial role in the world’s beer
industry. Therefore, with the curiosity about beer among Americans, let’s have an insight into
their beer industry. After some research, we found that the website “BeerAdvocate.” users
are mainly from the U.S., So we retrieved the user data, brewery data, and review data,
ranging from 1998 to 2017, from the BeerAdvocate datase

## Research questions
### 1. Identity the sentiments in users' reviews, and extract high-frequency words to obtain useful information.<br>
We will investigate the influence of consumer reviews on changes in beer style trends and identify the qualities that the best-selling beer should possess in the eyes of consumers. We will also provide suggestions for beer production based on our findings.

### 2. Data Visualization and Choose the popular beers<br>
We will explore the changing trends in the popularity of the most popular beer styles in the United States from 1998 to 2017, as reflected in the number of reviews on BeerAdvocate. We will also examine the changing trends of the top 3 beer styles and make predictions about their future. Additionally, we will identify common characteristics shared by the top 3 beers.

### 3. Suggestions in Brewing Beer<br>
To investigate the relationship between beer style preference and region, we will examine the trend of beer style preference in various regions over time and generate recommendations for breweries and sellers based on the results.



In this part, we conducting an analysis of consumer preferences for beer in different regions,then we have compiled all of the relevant data to provide suggestions for beer production based on our findings.


## Datasets
**BeerAdvocate**

## Method
### Data preprocessing
**Data slice**
Although the initial rating data was saved in text format, they were too big to parse and analyze. Before the analysis, we used Python bash to slice and prepare the data for CSV loading by pandas.

**Clean Data**
- We first find that nan values in ```overall``` coexists with ```['appearance', 'aroma', 'palate', 'taste', 'overall']```, We also checked the website manually and found that we should rate the appearance, aroma, palate, taste, and overall. So, these data are meaningless if all of these features are nan values. So we also deleted data like this.
- Some reviews' *overall* scores are significant incompatible to the other 4 scores. For example, if the each of the 4 scores is less than 3, while the overall score is greater than 4, then we considered them to be invalid.
- We will also delete the data without review text.


## Analytic methods<br>

- We initially conducted a statistical analysis on the pre-processed dataset to examine the relationship between the four scoring aspects and the overall score. Afterwards, we utilized a statistical model to further analyze the dataset in order to gain a better understanding of trends in consumer reviews of beer in the US beer market<br>
<img src="Image\2.png" />


- Consumer reviews often contain valuable insights and opinions on different beers. In order to better understand consumer preferences and opinions, it is necessary to analyze these reviews. In this study, we used sentiment analysis and natural language processing techniques to analyze the tone and content of consumer reviews. We employed the SentimentIntensityAnalyzer module from the nltk library to identify the sentiment of consumer comments and identified the most frequently mentioned keywords by consumers. These findings provide important insights into consumer preferences and opinions on different beer styles.<br>

  <img src="Image\4.png" width=350 height=280/> <img src="Image\6.png" width=350 height=280/>



- Analyze the distribution of popular beers with respect to different characteristics and summarize their features. Afterwards, use data visualization techniques to select the most popular beers.<br>

  <img src="Image\7.png" />



- we will perform a further analysis of the three most popular beers in the US market and use a time series model to forecast their future trends. To improve the accuracy of our predictions, we will utilize the time series prediction module in the sktime library.<br>

  <img src="Image\8.png" /> 

- To investigate the preferences of consumers in different regions for beer styles, we utilized the bar_chart_race library to dynamically visualize the changes in consumer preferences over time. This allowed us to gain a better understanding of the evolving preferences of beer drinkers in different regions.Combining all the above factors, we aprovide suggestions for beer production based on our findings.<br>

  ![Alt Text](https://github.com/Weijun-H/ada-2022-project-letusnameagroup/blob/main/gif/+United%20States,%20California.gif?raw=true)
  



## Proposed timeline

- 15.11.22 Slice and preprocess the dataset
- 18.11.22 Explore the factors associated with the beer ratings.
- 18.11.22 **Milestone 2** deadline
- 22.11.22 Pause project work.
- 02.12.22 **Homework 2** deadline
- 08.12.22 Begin developing a rough draft of the datastory.
- 09.12.22 Finish Statistical tests
- 11.12.22 Complete all code implementations and visualisations relevant to analysis.
- 14.12.22 Complete datastory.
- 21.12.22 Complete the website
- 23.12.22 **Milestone 3** deadline


## Organization within the team
- datastory: member 1 & 2
- website: member 3 & 4
- Code implementation: Work together
- Analysis: Group discussion
    

​    

