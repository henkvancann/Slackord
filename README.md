# ![Slackord Logo](https://i.imgur.com/PyVjqzL.png)Slackord
![Discord Shield](https://discordapp.com/api/guilds/1095636526873972766/widget.png?style=shield)    
[Join the Slackord Discord!](https://discord.gg/yccMweYPN8)

Slackord is a cross-platform application that parses JSON chat history file exports from Slack and posts them into Discord instantly with a single command.

# Demo
https://github.com/thomasloupe/Slackord/assets/6563450/adee8003-b51b-4859-b8d4-3a3e8dcc33c2

# Features
1. `Cross platform` - Works on Windows(x64) and Mac(x64).
1. `Imports channels` - Slackord will automatically recreate all your Slack channels on Discord along with their descriptions.
1. `Batch parsing/posting` - Instead of importing JSON files individually, Slackord will read your entire Slack export directory for JSON files, and parse/post them to Discord.
1. `Output window` - Slackord has a log window that will warn you if anything went wrong.
1. `Progress bar` - Slackord has a progress bar for parsing and posting messages to Discord.
1. `Slack-to-Discord markdown` - Slackord will convert messages with markdown to Discord markdown.
1. `Auto rate-limit detection` - Slackord limits the messages it sends over time so it doesn't spam or get itself squelched for posting too often.
1. `Ease-of-use` - Slackord only needs to be set up once, and it'll remember your bot's token, making future imports easy.
1. `Multiple Discord Servers` - Slackord can discern which Discord server it's in and can post to the server(s) you choose.
1. `Privacy first` - Slackord checks if user messages have a display name and will attempt to keep real names private unless there isn't one.
1. `Data safety` - Your data is yours. Slackord works completely off your local connection and machine.
1. `Update checks` - Slackord can check for the latest version with a single click. Get the latest version with new features and fixes easily!

# Getting Started
If you are on the free plan of Slack or need a reliable tool for exporting both private/public Slack JSON files *mostly* compatible with Slackord, check out [Slackdump](https://github.com/rusq/slackdump)! Please note, this tool is not developed by myself, and could potentially stop working for Slackord at any time.
1. Download the [latest](https://github.com/thomasloupe/Slackord/releases) Slackord release for your OS and extract the contents. If you're on Mac, make sure to `cd` into the Slackord directory you extracted, and grant execute permissions to the directory with `chmod +x *` from Terminal.
1. Create a Discord bot [here](https://discord.com/developers/applications) by selecting "New Application" at the top-right.
1. Name your bot "Slackord", or any preferred custom name.
1. Select "Bot" from the left panel, and click "Add Bot" at the top-right.
1. Under OAuth2>URL Generator, set the bot's "SCOPES" to "bot". This opens a new menu called "BOT PERMISSIONS" below.
1. In "BOT PERMISSIONS", set the bot's permissions to "Administrator". This allows Slackord to post to private channels, too.
1. Copy the "GENERATED URL" link below the "BOT PERMISSIONS", and paste into a browser.
1. Join the bot into your desired server using the link generated.
1. In the "Bot" page underneath "OAuth2", Upload an image for your bot if desired.
1. Click "Reset Token", select "Yes, do it!", then click the "Copy" button to the left of "Regenerate". "Keep it secret, keep it safe."
1. Ensure that both "PUBLIC BOT" and "REQUIRES OAUTH2 CODE GRANT" sliders are turned off.
1. In "Privileged Gateway Intents", tick the slider to enable "MESSAGE CONTENT INTENT".

# Running Slackord
1. Run Slackord.
1. Click `Set Bot Token` and paste the copied token into the popup text field. Slackord will remember your token if you close it.
1. Click `Connect` to connect the bot to your server.
1. Click `Import JSON` and select the Slack JSON chat history root folder.
1. Once parsing has completed, visit any Discord channel you wish and type `/slackord` (case insensitive). Messages will begin posting and the progress bar will update as messages are sent.

# Important: Please Read!
1. If you need help, please feel free to join the Discord community listed at the top of this page, or open a new issue if it doesn't already exist.
1. If you have a very large Slack server to import, it's much better to parse a couple channels at a time rather than of all of them at once. "Large servers" would be Slack imports that have more than 400+ JSON files to parse in total across all channels.
1. Slackord is free, and it will always be free. However, if you found Slackord worth donating something, you can donate from within Slackord by clicking Donate inside Slackord, or you can sponsor Slackord at the top of this repository by clicking the heart (sponsor) button. You can also [click here](https://paypal.me/thomasloupe) (PayPal) to donate directly to me.
