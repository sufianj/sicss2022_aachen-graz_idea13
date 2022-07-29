# sicss2022_aachen-graz_idea13

## Description: 
The American National Election Studies (ANES) are national representative surveys of American eligible voters that have been conducted before and after every presidential election since 1948. The focus of the survey includes voter perceptions of the major political parties, the candidates, national and international issues. 

Here we asked whether opinions expressed by Twitter users match, in an aggregated manner, those gathered in the ANES (after controlling for demographics) or if it is true that extreme opinions are overrepresented and more salient in social networks.

## Research questions and hypotheses:
As seen in ANES data, negative feelings towards the opposite party are increasing (Iyengar et al., 2019). Could we observe this trend using Twitter data?

Just before every American election there is an important and controversial event that captures media attention (aka “October Surprise”). How do these events impact Twitter? Are there more tweets related to the election? Are there more negative tweets? Do the negative tweets affect both candidates or only the one involved in the scandal?

## the notebooks

download_sampled_tweets.ipynb pulls tweets and saves it to a local MongoDB, then clean emojis @user and URL in the text contents, and export the tweets to .CSV

tweet_processing.ipynb uses pretrained classifiers to annotate the collected tweets, and calcultes the daily average sentiment of the october surprises. We highly recommend to run it with GPU.

MergedDataByYear.ipynb combines the results from classified tweets and ANES data

## the data
According to Twitter's policy, we are not allowed to publish tweets. 

Thus we share the classified results for those who want to run MergedDataByYear.ipynb with ANES data.

The ANES could be downloaded from https://electionstudies.org/data-center/ 