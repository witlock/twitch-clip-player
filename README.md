# twitch-clip-player

Add as browser source and fill in the client key by creating an app at https://dev.twitch.tv/console

1. Download **clipplayer.html**
1. Sign up at https://dev.twitch.tv/console
2. Register a new application on the dev console by picking a name and using http://localhost for "OAuth Redirect URLs"
3. Copy the **Client Key**
4. Open **clipplayer.html** and paste the **Client Key** to **var apiKey = "HERE";**
5. Change **var twitchChannel = "witlock"**; to your own channel
6. Add a new browser source in OBS and browse to **clipplayer.html**

If the clips are getting cut off while playing change the **var playDelay = 2500;** to some higher value (milliseconds)
