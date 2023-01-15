<h1>Stock Market and Twitter Correlation Analysis</h1>

 ### [Video Demonstration](https://youtu.be/7eJexJVCqJo)

<h2>Description</h2>
We began by using the Polygon API to collect stock information from various large companies such as Apple, Microsoft, and Amazon.
We pulled daily statistics from January 1st, 2022 up until November 30th and aggregated the information into a large list. We chose
to simplify the data into three vectors (date, performance, and range) and store it in a list of pandas dataframes, where each
company had its own dataframe. Date represented the day that the given piece of information pertained to, performance represented
how much the stock price increased or decreased over that day, and range represented the difference between the highest and lowest
stock prices of that day. From there, we normalized the performance and range indicators to values between 0 and 1.
<br/>

Since the stock information is our outcome, we needed to convert it into one metric, which we did by summing performance and range
and then normalizing it once again. This converted the information into one ‘Activity’ metric which served as a general
representation for how much a stock value changed over a day’s period.
<br/>

Our next step was to collect twitter information, which we did using Tweepy to access the Twitter API. We compiled a list of the
usernames of CEOs for the companies we pulled stock data from, and used Tweepy to create a dataframe of how many tweets, likes,
retweets, and quote tweets were associated with each of those usernames over a day’s period between January 1st, 2022 and November
30th. During this process we found that some values were null which meant that no tweets, likes, retweets, or quote tweets happened
on that day. So, we chose to fill those null values with 0 to quantitatively represent that.
<br/>

From there, we concatenated our twitter and stock dataframes into one dataframe that we used to create our model with. 
<br/>

<h2>Languages and Utilities Used</h2>

- <b>Python</b> 
- <b>Numpy/Pandas</b> 
- <b>SciKitLearn</b>
- <b>Twitter API Tweepy Client</b>
- <b>Polygon API RESTClient</b>

<h2>Environments Used </h2>

- <b>Jupyter Notebook</b>

<h2>Program walk-through:</h2>

<p align="center">
Import the necessary libraries: <br/>
<img src="https://imgur.com/Pxgi08u.png" height="80%" width="80%"/>
<br />
<br />
Set up the Polygon API Client:  <br/>
<img src="https://imgur.com/7ZJUEPw.png" height="80%" width="80%"/>
<br />
<br />
Collect data from Polygon: <br/>
<img src="https://imgur.com/3usO9r8.png" height="80%" width="80%"/>
<br />
<br />
Set up the Twitter API Tweepy Client:  <br/>
<img src="https://imgur.com/ymauZ62.png" height="80%" width="80%"/>
<br />
<br />
Collect data from Twitter:  <br/>
<img src="https://imgur.com/kmIwqQN.png" height="80%" width="80%"/>
<br />
<img src="https://imgur.com/MlfeJ0c.png" height="80%" width="80%"/>
<br />
<br />
Build a Random Forest Regressor model:  <br/>
<img src="https://imgur.com/SNejO7I.png" height="80%" width="80%"/>
<br />
<br />
Build a Support Vector Machine Regression model:  <br/>
<img src="https://imgur.com/U41qDis.png" height="80%" width="80%"/>
<br />
<br />
Build a Linear Regression model:  <br/>
<img src="https://imgur.com/CkaKasL.png" height="80%" width="80%"/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
