# Installation

## Badger\_Discord\_API Installation

### Notes

Some methods of the API not may fully work or be broken. I was able to test most and 75% of it works. If something does not work, please just submit an issue or pull request for it on the GitHub page. Thanks!

### What is it?

This is essentially a Discord API for FiveM. It utilizes the REST API of Discord for all your essential needs :\) Things that are heavy in Discord rate limiting \(such as retreiving all server roles and player avatars\) will be automatically stored to a cache for developers automatically. I will be moving all my scripts over to use this API for better ease of use. Some features include not having to gather role IDs at all, since the script gets the server's roles automatically, so you can just specify the role's name instead of role IDs at all \(however, be aware that this will break then if someone changes the roles' names on Discord\)... I hope you can all find some use for this, I know I will :P

### Installation

1. Set up a Discord bot via the developer portal on Discord. \([https://discord.com/developers/applications](https://discord.com/developers/applications)\)
2. Invite the Discord bot you created to your Discord.
3. Get the Discord bot token from the newly created bot.
4. Place the Discord bot token in `Bot_Token = '{BOT_TOKEN}',` in the `config.lua` file in place of `{BOT_TOKEN}` 
5. Get your Guild ID by copying the ID of your Discord server's logo in the sidebar of Discord.
6. Place the Guild ID in `Guild_ID = '{GUILD_ID}',` in the `config.lua` file in place of `{GUILD_ID}` 
7. You can now choose to set up the `RoleList` or not. Utilizing the `RoleList` makes you able to use keys in the other Discord scripts that will correspond to the config's value when checking a user for matching roles.

### Example Configuration

```text
Config = {
	Guild_ID = '597445834153525298', -- Badger's Development Discord
	Bot_Token = 'NzE4OTM2MjQxNjI5OTU0MTcw.XtwHjQ.pJa80TEeRG0wyN2KNi9zyr4pBK8', 
	RoleList = {
		['Founder'] = 597446100206616596,
		['Admin'] = 597446815054430219,
		['Staff'] = 597450498060058624,
	},
}

Config.Splash = {
	Header_IMG = 'https://forum.cfx.re/uploads/default/original/3X/a/6/a6ad03c9fb60fa7888424e7c9389402846107c7e.png',
	Enabled = true,
	Wait = 10, -- How many seconds should splash page be shown for? (Max is 12)
	Heading1 = "Welcome to [ServerName]",
	Heading2 = "Make sure to join our Discord and check out our website!",
	Discord_Link = 'https://discord.gg',
	Website_Link = 'https://badger.store',
}
```

### Download

{% embed url="https://github.com/JaredScar/Badger\_Discord\_API" %}

