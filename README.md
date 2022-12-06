# Twitter Sentiment Analysis for "JPMorgan" 

## Purpose: 
Extract live tweets using twitter API to do sentiment analysis that will determine
public sentiments about JPMorgan.


## Area of Interest:
This program will pull in 500 tweets but it has the ability to paginate for additiona data. 
The data is not limited to certian geo location. I am pulling 500 tweets that have geo 
location with them.  


## How to run this program
First, you will have to sign up for the twitter developer account. 
Once, your account is set up, please save your API key somewhere secure. You API keys shouldn't be share with any any as someone can access your twitter account through it. 
For this program, i have created a seperate config.ini file where you can store your api key, the program is then refering to the keys in that file. Make sure your config.ini and your program file are in the same location. 

Once you are authenticated, you can run the next block of jupyter program where i have stored all the funtions which are refered to in the next programs blocks. 
Right below the all my funtion, you will find code that search the 500 tweets with search string of "jpmorgan @jpmorgan". It will pull the following data: Tweet, Tweet's Author, Tweet's location, sentiments and tweet time. 

The follwoing code block will visualize the results in pie chart format using the 500 tweets we just extracted. It will show what the majority of tweets setiments are. 
The next code will show a visual of all the key words and their frequencies. The visuals can show what is most talk about words in the tweets. 
The next code will display word cloud of the first 500 words. This can help in analysis to know what are some topic that are being discussed in the tweets. 
The next few block of code are develop to create an interactive analysis on the data. The user is asked to input a location from the list of location that are pulled from twitter. When the user type in the intrest of location, they will get a output that will display the tweets of that location and there sentiment. The results are aggregated into a pie chart visuals to show for that particular location what are the highest sentiments. The same is done for the date as well where the user can select a date and analysis the tweets sentiments by date.  
Finally, in the last code block, i have tired to visualize the result over time. 

## References: 
https://developer.twitter.com/en
https://www.nltk.org/api/nltk.sentiment.vader.html
https://textblob.readthedocs.io/en/dev/
https://developer.twitter.com/en/docs/tutorials/filtering-tweets-by-location
https://developer.twitter.com/en/docs/twitter-api/v1/geo/place-information/api-reference/get-geo-id-place_id
https://www.youtube.com/watch?v=txPNMDDWsB8
https://docs.tweepy.org/en/stable/
https://gist.github.com/ssskip/5a94bfcd2835bf1dea52
