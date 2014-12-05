Explaining Racism @racismexplained
=====

A twitter bot to reply to racists based on  NodeJS.

####Local Setup:

All that you need to do is create a new file named runtime.js inside the config folder, and update this:

    
    {
    "twitter" : {
        "consumer_key" : "<your consumer key>",
        "consumer_secret" : "<your consumer key>",
        "access_token_key" : "<your access token>",
        "access_token_secret" : "<your access token secret>"
      },
      "keywords" : "words to match in tweet",
      "match" : "a string or regex. (capture groups are allowed)",
      "replies" : [
        "some reply. Can reference parts of the tweet like [user.screen_name] or regex matches like $1"
      ],
      "max_replies_per_minute" : 6,
      "in_reply_to" : true
    }
    

This code is based on: Jesse Ditson's reply bot running on NodeJS