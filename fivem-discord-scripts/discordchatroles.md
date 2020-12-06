# DiscordChatRoles

**CURRENT VERSION: 7.0**

## Badger's Discord Community

[![Developer Discord](https://discordapp.com/api/guilds/597445834153525298/widget.png?style=banner4)](https://discord.com/invite/WjB5VFz)

## Requirement

{% embed url="https://github.com/JaredScar/Badger\_Discord\_API" %}

## Installation Tutorial

{% embed url="https://youtu.be/UUzSdQtJE4s" %}

## **Version 1.0**

Picture example taken from my RP server:

![](https://i.gyazo.com/c845547a9cbcd99e7716726d53abb216.png)

**Example of how the chat roles are set up and what you should change:**

```text
--[[
    List in order of least priority to highest with 
    highest priority overtaking role before it if 
    they have that discord role.
]]--
roleList = {
{0, "^4Civilian | "}, -- 1
{1, "^3Trusted Civ | "}, -- 2
{1, "^2Donator | "}, -- 3
{1, "^1T-Mod | "}, -- 4
{1, "^1Mod | "}, -- 5
{1, "^1Admin | "}, -- 6
{1, "^6Management | "}, -- 7
{1, "^5Owner | "}, -- 8
}

-- For allowing colored chat
allowedColors = {3, 4, 5, 6, 7, 8}
allowedRed = {4, 5, 6, 7, 8}
```

The 1s should be replaced with IDs of the respective roles in your discord server. \(0 should stay for Civilian as it is the default role for all users\)

**Download** [DiscordChatRoles](https://github.com/TheWolfBadger/DiscordChatRoles)

## **Version 2.0** 

Chat colors can now be restricted to certain groups. The color red can also be restricted to only staff ranks!

## **Version 3.0** 

There is now a StaffChat for your staff members to use: 

![](https://i.gyazo.com/b82ef0e256ba67aa89db7d7307f77eef.gif)

Permission to use /sc and /staffchat:

```text
StaffChat.Toggle
```

## **Version 4.0**

Toggle off getting StaffChat messages \(good for staff members if they are streaming their own RP\)

Commands:

`/sc toggle`

`/staffchat toggle`

## **Version 5.0**

You can now change your chat-tags with the in-game command using /chattag and /chattag \[id\]

![](https://i.gyazo.com/d41d1a27f326461d07b01f669ea07a8d.png)

## Version 6.0

You can now change your chat-color when you talk in-game using /cc or /chatcolor

Commands: /cc - List out the chat colors you have access to /chatcolor - List out the chat colors you have access to /chatcolor  - Change chatcolor to the ID specified /cc  - Change chatcolor to the ID specified

![](https://i.gyazo.com/394fa27e4c675cd63832e83d43d5b4a6.gif)

**How it works?** 

You basically set this up using a config in which the keys are the permission ACE value that gives them access to see and use those chat colors.

Config \(you'll have to find this in server.lua, in a future version I'll move it to the top though\):

```text
local availColors = 
{
    ['DiscordChatRoles.Access.Donator'] = {
        ['White'] = {'^0'},
        ['Green'] = {'^2'},
        ['Yellow'] = {'^3'},
        ['Blue'] = {'^4'},
        ['Light Blue'] = {'^5'},
        ['Purple'] = {'^6'},
        ['White'] = {'^7'},
        ['Pink'] = {'^9'},
        ['Police'] = {'^1', '^4'},
        ['Police2'] = {'^4', '^1'},
        ['Christmas'] = {'^2', '^1'},
        ['Christmas2'] = {'^1', '^2'},
    },
    ['DiscordChatRoles.Access.Elite'] = {
        ['RainbowYGB'] = {'^3', '^2', '^4'},
        ['RainbowFull'] = {'^3', '^4', '^1', '^5', '^6', '^7', '^9'},
    },
    ['DiscordChatRoles.Access.Staff'] = {
        ['Red'] = {'^1'},
    }
}
```

Following the format of the config, you can add multiple different permission for chat colors and set up a vast variety of different pattern combinations!

I hope you all enjoy! 

## Version 7.0

You now have the option of enabling block messages within the chat rather than the default chat messages you are used to. An example of this can be shown below.

![](https://i.gyazo.com/dba204b15bd15aadd387f0e7a0509293.gif)

To enable the block messages, just enable it within the configuration section in `server.lua` 

```text
-- CONFIG --
roleList = {
{0, "👦🏻 ^4Civillian | "}, -- 1
{1, "🏘️ ^3Resident | "}, -- 2
{1, "💳 ^2Donator | "}, -- 3
{1, '🤑 ^4ELITE | '}, -- Elite donator 4
{1, '🧯 ^8Fire/EMS | ^0'}, -- Fire/EMS 5
{1, '👮 ^2LSPD | '}, -- LSPD 6
{1, '👮 ^2SASP | '}, -- 7
{1, "✈️ ^9FAA | "}, -- 8
{1, '🛦️ ^3National Guard | '}, -- National Guard 9
{1, "🔻 ^1T-Mod | "}, -- 10
{1, "🔻 ️^1Mod | "}, -- 11
{1, "🐦 ^8Admin | "}, -- 12
{1, "☂️ ^6Management | "}, -- 13
{1, "🐉 ^5Owner | "}, -- 14
{1, "🦡 ^9Systems Administrator | "},
}
sendBlockMessages = true; -- This will enable sending block messages
```

## Download

{% embed url="https://github.com/TheWolfBadger/DiscordChatRoles" %}

