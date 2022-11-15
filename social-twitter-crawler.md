# Social Media Bailout Nov-14-2022

## Take a backup of data /  content on twitter and Linkedin and make this consistently stored.

### Pick up social graphs from twitter, linkedin and facebook and pull them up elsewhere.

Twitter:
This would be an attempt to make a paginated api calls to;
- fetch the list of all followed on twitter
- fetch the list of all following on twtiter
- fetch all the tweets made by me (Authenticated user)
- fetch a list of all the bookmarked tweets
- fetch just textual information from the links that are auto shortened /  use twitter URL shortener for twitter analytics
- Dump all of this into csv files, into S3, into anywhere. 
- Obtain a list of all of these related information
- Look for equivalent to google takeout or similar. (Mandatory since GDPR ruling / adherence)


From here, attempt to construct a timeline of the last set of independent tweets from those followed searching for the words: reach, contact, email or period ( full stop (.)) or mastodon or any form of social contact presence.
*Look throught patterns for what people say when they want to leave contact information through the obtained data*

Put together multiple feeds from fetched data (Similar to tweetdeck (might be down since *musk*) ref: [tweetdeck](https://www.wired.com/2012/03/hands-on-tweetdeck-wants-to-be-your-pro-twitter-client-again/)) 
Let this be an repetitive running loop that updates feed of tweets every 30 minutes.
```
~ 5000 api calls each 30 minutes for fetching immediate timelines
~ 50 * 2  polling api calls to fetch following and followed users list unless sorted by proximity time; Let it be append only to a deduplicated list.
~ 1000 API calls for initially seeding bookmarks table
```
### Questions: 
- What are immediate rate limiters for obtaining this information ?
- How long until we hit rate limiters ?
- What is the process for bypassing exponential backoff or whatever their ddos countering mechanism is ?
- How do visualize this data 
	- Roam js web
