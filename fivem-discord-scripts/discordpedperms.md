# DiscordPedPerms

**Version 1.0** 

### Badger's Discord Community

[![Developer Discord](https://discordapp.com/api/guilds/597445834153525298/widget.png?style=banner4)](https://discord.com/invite/WjB5VFz)

## **What is it?**

Another discord script, yes, you're all welcome!

This one restricts peds to certain discord groups much like my other scripts

![](https://i.gyazo.com/871c59810a40bff4bedacee0759bdd9f.gif)

Forgive my typing mistakes in the gif please... Thanks

You must set up IllusiveTea's discord\_perms script for this to work properly. --&gt; [https://forum.cfx.re/t/discord-roles-for-permissions-im-creative-i-know/233805](https://forum.cfx.re/t/discord-roles-for-permissions-im-creative-i-know/233805)

{% embed url="https://youtu.be/sjbFzkII2T0" %}

## **How it works**

Find the following within your server.lua and replace the 1s in here with discord role IDs:

```text
roleList = {
1, -- Trusted Civ (1)
1, -- Donator (2)
1, -- Personal (3)
}
```

responds to it's respective number within the other list \(which will be located in the client.lua\):

```text
restrictedPeds = {
{}, -- Trusted Civ (1)
{}, -- Donator (2)
{
"mickeymouse",
"deadpool",
"kermit",
"blackpanther",
}, -- Personal (3)
}
```

Therefore blackpanther, deadpool, and kermit would be restricted to be used by the roleList group 'Personal'

It's quite simple :\)

## **Download**

 [DiscordPedPerms](https://github.com/TheWolfBadger/DiscordPedPerms)

