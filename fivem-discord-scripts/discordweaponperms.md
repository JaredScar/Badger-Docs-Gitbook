# DiscordWeaponPerms

## **Version 1.0**

Another discord script of course! With this script, you can restrict weapons to certain roles on your discord server! This script also allows restricting certain attachments to different groups as well \(however, it'll remove the weapon if they have the attachment, I'll eventually update it to just remove the attachment from the weapon\).

### Badger's Discord Community

[![Developer Discord](https://discordapp.com/api/guilds/597445834153525298/widget.png?style=banner4)](https://discord.com/invite/WjB5VFz)

## **Requirements**

{% embed url="https://github.com/JaredScar/Badger\_Discord\_API" %}

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
restrictedWeapons = {
{}, -- Trusted Civ (1)
{}, -- Donator (2)
{
"WEAPON_RPG",
}, -- Personal (3)
}
```

The RPG weapon would then be restricted to only people with personal discord role within your discord server.

It's quite simple **:\)**

## **Download**

 [DiscordWeaponPerms](https://github.com/TheWolfBadger/DiscordWeaponPerms)

