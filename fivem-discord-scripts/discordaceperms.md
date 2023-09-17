# DiscordAcePerms

## **Version 1.0**

This is another one of my discord scripts! :) If used properly along with my other scripts, you can fully make your server use only discord roles for permissions and chat roles ;)

### Badger's Discord Community

[![Developer Discord](https://discordapp.com/api/guilds/597445834153525298/widget.png?style=banner4)](https://discord.com/invite/WjB5VFz)

## **Requirement**

{% embed url="https://github.com/JaredScar/Badger_Discord_API" %}

## **Installation Tutorial**

{% embed url="https://www.youtube.com/watch?v=blOnyLfevw8" %}

Example of how to set it up:

```
roleList = {
{1, "group.tc"}, --[[ Trusted-Civ --- ]] 
{1, "group.faa"}, --[[ FAA --- ]]
{1, "group.donator"}, --[[ Donator --- ]]
{1, "group.trialModerator"}, --[[ T-Mod --- ]] 
{1, "group.moderator"}, --[[ Moderator --- ]]
{1, "group.admin"}, --[[ Admin --- ]]
{1, "group.admin"}, --[[ Management --- ]]
{1, "group.owner"}, --[[ Owner --- ]]
}
```

The 1s should be replaced with IDs of the respective roles in your discord server. The quotes with groups should represent the groups in your permissions.cfg or server.cfg.

1. Download DiscordAcePerms
2. Extract the .zip and place the folder in your /resources/ of your Fivem server
3. Put `add_ace resource.DiscordAcePerms command.add_principal allow` and `add_ace resource.DiscordAcePerms command.remove_principal allow` in server.cfg
4. Make sure you add \`start DiscordAcePerms\` in your server.cfg
5. Enjoy ![:slight\_smile:](https://forum.cfx.re/images/emoji/twitter/slight\_smile.png?v=9)

Common Errors:

1.
{% embed url="https://imgur.com/a/F6GzgOg" %}

This usually means you have not added a comma at the end of the line

2. Server not granting roles when you join
   (No screenshot for this one due to no errors pop up in console)
   This usally means you have not put quotation marks on the role names

There are other errors that I have not covered but majority of the time this is caused to to LUA syntax errors (ie missing a comma missing a quotation mark ext)
You can check if your configuration file has any syntax errors if you go to a website such as https://fptje.github.io/glualint-web/ or https://rextester.com/l/lua_online_compiler and inputting your config file.




## **Download**

&#x20;**** [DiscordAcePerms](https://github.com/TheWolfBadger/DiscordAcePerms)
