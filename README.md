# Twitter Sentiment Analysis for "JPMorgan" 

## Purpose: 
Extract live tweets using twitter API to do sentiment analysis that will determine public sentiments about JPMorgan.
## Area of Interest:
This program will pull in 200 tweets, but it has the ability to paginate for additional data. 
The data is not limited to certain geo location. I am pulling 200 tweets and some of the tweets might not have geo information. 
## How to run this program
First, you will have to sign up for the twitter developer account. 
Once, your account is set up, please save your API key somewhere secure. Your API keys shouldn't be share with any one as someone can access your twitter account through it. 
For this program, i have created a separate config.ini file where you can store your api key, the program is then referring to the keys in that file. Make sure your config.ini and your program file are in the same location. 

Once you are authenticated, you can run the next block of Jupiter program where i have stored all the functions which are referred to in the next programs blocks. 
Right below all my function, you will find code that search the 200 tweets with search string of "jpmorgan @jpmorgan". You can change the number of tweets. You can pull more than 200 tweets if you like. If you apply for elevated access on twitter, you can pull up to 2 million tweets!
It will pull the following data: Tweet, Tweet's Author, Tweet's location, sentiments, and tweet time. 

The following code block will visualize the results in pie chart format using the 200 tweets we just extracted. It will show what the majority of tweets sentiments are. 
The next code will show a visual of all the key words and their frequencies. The visuals can show what is most talk about topic in the tweets. 
The next code will display word cloud of the first 500 words. This can help in analysis to know what are some topics that are being discussed in the tweets. 
The next few blocks of code are developed to create an interactive analysis on the data. The user is asked to input a location from the list of location that are pulled from twitter. When the user type in the interested location, they will get an output that will display the tweets of that location and there sentiment along with aggregated sentiments result as a pie chart which can help us know which sentiment is highest in that location. it will also display a word cloud of that location as well. The same is done for the date as well where the user can select a date and analyze the tweets sentiments by date.  
Finally, in the last code block, I have tried to visualize the sentiment over time. 

## References: 
https://developer.twitter.com/en
https://www.nltk.org/api/nltk.sentiment.vader.html
https://textblob.readthedocs.io/en/dev/
https://developer.twitter.com/en/docs/tutorials/filtering-tweets-by-location
https://developer.twitter.com/en/docs/twitter-api/v1/geo/place-information/api-reference/get-geo-id-place_id
https://www.youtube.com/watch?v=txPNMDDWsB8
https://docs.tweepy.org/en/stable/
https://gist.github.com/ssskip/5a94bfcd2835bf1dea52
