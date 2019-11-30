### **Introduction**

This dataset is the tweet archive of Twitter user @dog\_rates, also known as WeRateDogs. WeRateDogs is a Twitter account that rates people&#39;s dogs with a humorous comment about the dog. These ratings almost always have a denominator of 10. The numerators, though? Almost always greater than 10. 11/10, 12/10, 13/10, etc. The objective of this project is to wrangle the messy Twitter data to create interesting and trustworthy analysis and visualizations.

#### The following steps were taken to wrangle the data

- Gathering data
- Assessing data
- Cleaning data

#### **Step 1 : Gathering Data**

1. The WeRateDogs Twitter archive. Downloaded the file manually from the following link: twitter\_ archive\_enhanced.csv
2. The tweet image predictions, i.e., what breed of dog is present in each tweet. This file(image\_predictions.tsv) is hosted on Udacity&#39;s servers and was downloaded programmatically using the [Requests](https://pypi.org/project/requests/) library and the following URL: [https://d17h27t6h515a5.cloudfront.net/topher/2017/August/599fd2ad\_image-predictions/image-predictions.tsv](https://d17h27t6h515a5.cloudfront.net/topher/2017/August/599fd2ad_image-predictions/image-predictions.tsv)
3. Using the tweet IDs from the Twitter archive, the Twitter API was queried  for each tweet&#39;s JSON data using Python&#39;s [Tweepy](http://www.tweepy.org/) library and stored the entire set of tweet data in a file called tweet\_json.txt  file.

#### **Step 2 : Assessing Data**

As a second step of the Data wrangling process, assessing helped to figure out several Quality issues (content related) and some tidiness issues (structural types).

#### **Step 3: Cleaning Data**

After Assessing the data the data it was time to clean the data, which means addressing all the quality and tidiness issues listed above. Copies of each of the dataset were made before the Cleaning step. Cleaning also involved removing duplicates and missing data. The dataset was then stored as twitter\_archive\_master.csv.
