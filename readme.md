# AO-Killboard

A discord bot for Albion Online's killboard

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

![Screenshot](https://i.imgur.com/gLnvJpX.png)

### Usage
* !ping - replies with @user pong
* !kbclear - delets all messages in the config.botChannel
* !kbinfo <eventId> - displays the killboard post for a specific kill to the current channel

### Prerequisites

* [NodeJS](https://nodejs.org/)

### Installing
* Install Node JS on the machine that will run the bot
* Create a new [Discord Application](https://discordapp.com/developers/applications/me)
* Copy config.json.example --> config.json
* Add the 'APP BOT USER' token as 'token' in 'config.json'
* Enable developer mode in Discord (Settings -> Appearance)
* Right click the channel you wish to use as the kill board, and Copy ID
* Set ID as 'botChannel'
* OPTIONAL: Set User IDs for admin accounts

* **To add the bot to your server**: Visit https://discordapp.com/oauth2/authorize?client_id={YOUR CLIENT ID}
Example: https://discordapp.com/oauth2/authorize?client_id=975390562344173493

###### * to only display Guild kills and not alliance, set allianceName to something that cannot exist i.e <NONE>

Example: config.json
--
```json
{
	"cmdPrefix": "!",
	"allianceName": "<NONE>",
	"guildName": "IX Legion",
	"username": "AO-KillBot",
	"admins": [
		"353675594527145994"
	],
	"botChannel": "353675594527145994",
	"token": "MzUzNjkyMzk0MDk0NTkyMDEw.DIzpnA.ZDJM_MHu9GnbwSS5XC3SeVBTX7o"
}
```

### Built With

* [Discord.js](https://github.com/hydrabolt/discord.js/) - Discordapp library for Node.js and browsers.
* [Request](https://github.com/request/request) - Simplified HTTP client

## Authors

* **Dogukan AKTEKE** *Hex#9851*
