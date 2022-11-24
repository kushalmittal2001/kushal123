# DiscordMirroerPlus

DiscordMirrorerPlus is a an extensive application capable of mirroring Discord messages from channel A to channel B in the most verbose way capable in the Discord API. 

## Installation

All that is required is Node.js. A quick google search will allow you to download and install it. The application is written in such a way that no node_modules are required for it to function (saves headaches).

```bash
node dist/index.js
```

### .env file
TOKEN is your Discord access token
DEBUG should be left as it is
IGNORE_SETUP will if set to true automatically load the save.json
LOGIN_USERNAME will if set to your DiscordMirrorerPlus username login you automatically, if LOGIN_PASSWORD is set as well

### Common errors
Q: My cmd crashes on startup after I've registered!
Make sure that the full path containing the script folder does not include any spaces (example: C:\Users\Desktop\my script\DiscordMirrorerPlus-release => C:\Users\Desktop\my_script\DiscordMirrorerPlus-release)

Q: After using automatic mode and cloning all channels, not all channels are being mirrored!
If it's a large amount of channels, I recommend either choosing less channels or inputting them manually with the manual mode. This is because rate-limiting for the creation of webhooks is not yet implemented (will be soon) and/or the webhook limit per server is 50.

### Latest updates
14/9/2022 - Added proxy support
05/09/2022 - Added embed editor
31/8/2022 - Added native attachment support