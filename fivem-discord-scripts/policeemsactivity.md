# PoliceEMSActivity

**CURRENT VERSION: 1.0**

## **Version 1.0** 

So you want a script in which other emergency services can see their colleagues on the mini map with their locations, but you don't want regular players to see these blips unless they are on duty as well? You want this script to support multiple roles? You want it to be customizable? You want it to use discord for the permission basis of it? Oh well, I have the script for you.

_Essentially, PoliceEMSActivity is a script in which is like a /onduty command, but on steroids. You can use /duty to toggle between being on duty and off duty. With this comes some awesome things too though. There are Blip-Tags people can toggle between if they are in multiple departments. Also, there are webhooks you can set up for each different department and send their clock-ins and clock-outs to when they toggle /duty or log off whilst on duty. There is also a /cops command so you can check to make sure all the people who are using /duty are actually on duty and in RTO \(on your discord server voice channels I assume\), then punish them accordingly if they use it for metagaming._

### Badger's Discord Community

[![Developer Discord](https://discordapp.com/api/guilds/597445834153525298/widget.png?style=banner4)](https://discord.com/invite/WjB5VFz)

## **Download**

 [PoliceEMSActivity](https://github.com/TheWolfBadger/PoliceEMSActivity)

## **Installation Tutorial** 

{% embed url="https://www.youtube.com/watch?v=xDfyGcqX5sA" %}

**Dependency:** 

{% embed url="https://github.com/JaredScar/Badger\_Discord\_API" %}

**Features** 

Blips on the map with Blip-Tags

![](https://i.gyazo.com/47fd9b1214ab90f3fe0e5ffab28fb892.png)

Blip-Tags \(using /bliptag to list them out - /bliptag \[id\] to change\): 

![](https://i.gyazo.com/5039d464bab28edb0457528be8b388e5.png)

Using /cops to list the online players on duty: 

![](https://i.gyazo.com/fc94e5f06e2f18a08aa28d0aacebc063.png)



**Config**

```lua
--[[
    1 = Red
    2 = Green
    3 = Blue
    5 = Yellow
    17 = Orange
]]--
-- CONFIG --
RoleList = { 
    ["ROLE-NAME-OR-ID-HERE"] = {
        {'👮 Sheriff | ', 17, nil},
        {'👮 LSPD | ', 2 , nil},
        {'👮 SAHP | ', 3, nil},
    },
},

Inheritances = { --MUST HAVE EnableInheritances SET TO TRUE TO WORK!
    ["ROLE-1-NAME-OR-ID-HERE"] = {"ROLE-TO-INHERITE-ID-OR-NAME-HERE", "ANOTHER-ROLE-TO-INHERITE-ID-OR-NAME-HERE",},
},
```

Change the "key" to the corresponding discord role ID or BDAPI Name you want it to represent. You can also add more roles too. Below is an example of adding another role to the list and giving it the color yellow. In terms to the nil values, you can replace those with webhook links and they will log clock-ins and clock-outs to that channel for the player.

As for the Inheritances simply add the role name or ID in the "key" and the role name(s)/ID(s) you want the first role to inherit.

```lua
RoleList = { 
    ["ROLE-NAME-OR-ID-HERE"] = {
        {'👮 Sheriff | ', 17, nil},
        {'👮 LSPD | ', 2 , nil},
        {'👮 SAHP | ', 3, nil},
    },
    ["EXAMPLE-ROLE-NAME-OR-ID"] = {
        {'ExampleRole | ', 5, nil},
    },
},

Inheritances = { --MUST HAVE EnableInheritances SET TO TRUE TO WORK!
    ["ROLE-1-NAME-OR-ID-HERE"] = {"ROLE-TO-INHERITE-ID-OR-NAME-HERE", "ANOTHER-ROLE-TO-INHERITE-ID-OR-NAME-HERE",},
},
```

**Version 2.0** 

NEW FEATURE

Duration of minutes on tour is now included in the webhook messages! Example shown below. Also, weapons and armor are now removed when someone goes off duty :\)

![](https://i.gyazo.com/70c849fce1be1d54c9ccd822744a1ae3.png)

**VERSION 3.0**

NEW FEATURE

Added Inheritances and Exports. (Thanks to [@NickReagan](https://github.com/NickReagan))

**Exports;**
```lua
exports.PoliceEMSActivity:IsPlayerOnDuty(player) -- Returns bool(true/false) SERVER SIDE ONLY
exports.PoliceEMSActivity:GetPlayerDutyBlip(player) -- Returns a player's active duty blip as a string. SERVER SIDE ONLY
```

**Thanks** 

I wanna credit @minipunch for the original code I based this off of and used for the blips code. He made my life a whole hell of a lot easier :\) You can find his API this uses over [here](https://forum.cfx.re/t/release-emergencyblips/493022)

