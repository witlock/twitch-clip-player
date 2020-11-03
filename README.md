# twitch-clip-player

Add as browser source and fill in the client key by creating an app at https://dev.twitch.tv/console

1. Download **clipplayer.html**
1. Sign up at https://dev.twitch.tv/console
2. Register a new application on the dev console by picking a name and using http://localhost for "OAuth Redirect URLs"
3. Copy the **Client Key**
4. Open **clipplayer.html** and paste the **Client Key** to **var apiKey = "HERE";**
5. Change **var twitchChannel = "witlock"**; to your own channel
~~6. Add a new browser source in OBS and browse to **clipplayer.html**~~
6. Host this file on a local server (ex. WampServer) or on your website and add a browser source pointing to it.

If the clips are getting cut off while playing change the **var playDelay = 2500;** to some higher value (milliseconds)

You can avoid certain clips by adding the **slugs** (twitch.tv/witlock/clip/**ToughAdorableNewtFutureMan**?filter=clips&range=7d&sort=time) to the skipClips array.

```
skipClips = [
    'ToughAdorableNewtFutureMan',
    'ShySullenMallardDancingBaby',
    'your clip slug',
    'your second clip slug']
```
