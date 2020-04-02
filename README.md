# Game Deals

This is a Discord bot that scrapes the [r/GameDeals](https://www.reddit.com/r/GameDeals/) subreddit for free deals. It sends new deals to channels called "free-games" at 6am and 6pm every day.

## Built With

* [PRAW](https://github.com/praw-dev/praw) - Python Reddit API Wrapper
* [discord.py](https://github.com/Rapptz/discord.py) - Python Discord API Wrapper

## Configure bot

Create a `config.py` with the following properties:

```
DISCORD_TOKEN="" # Discord API token
DISCORD_CHANNEL_ID="" # name of the channel to post in
REDDIT_CLIENT_ID="" # Reddit client id from the API app
REDDIT_CLIENT_SECRET="" # Reddit secret from the API app
REDDIT_USERNAME="" # Account username to login
REDDIT_PASSWORD="" # Account password to auth
REDDIT_USER_AGENT="Game Deals" # Any name to define the Reddit user agent
```

## Register Discord Bot
Use the client API ID from the Discord app and enter this into the url
https://discordapp.com/oauth2/authorize?client_id=XXXX&scope=bot&permissions=8

Replace `XXXX` with your ID.


## Run Bot
```
python bot.py
```

This will connect the local running script with the Discord bot API and run the bot.