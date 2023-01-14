<h1>Stock Market and Twitter Correlation Analysis</h1>

 ### [YouTube Demonstration](https://youtu.be/7eJexJVCqJo)

<h2>Description</h2>
Project consists of a simple PowerShell script that walks the user through "zeroing out" (wiping) any drives that are connected to the system. The utility allows you to select the target disk and choose the number of passes that are performed. The PowerShell script will configure a diskpart script file based on the user's selections and then launch Diskpart to perform the disk sanitization.
<br />


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
