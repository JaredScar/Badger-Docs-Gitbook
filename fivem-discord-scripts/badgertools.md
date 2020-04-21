# BadgerTools

The administration tool for server owners that you've all been looking for! One of the most useful features being /spectate in which you can cycle spectating through players on the server and also hear everything said whilst spectating and being able to speak the user you are spectating! I hope you all enjoy! :\)

**Installation Tutorial**

{% embed url="https://www.youtube.com/watch?v=sjbFzkII2T0" %}

{% embed url="https://www.youtube.com/watch?v=xDfyGcqX5sA" %}

**IMPORTANT**

You must set up IllusiveTea’s discord\_perms script for this to work properly. --&gt; [Discord roles for permissions \(im creative, i know\)](https://forum.cfx.re/t/discord-roles-for-permissions-im-creative-i-know/233805)

You also must have my DiscordTagIDs script properly installed --&gt; [https://forum.cfx.re/t/discordtagids-i-know-i-know-i-only-make-discord-based-scripts/582513](https://forum.cfx.re/t/discordtagids-i-know-i-know-i-only-make-discord-based-scripts/582513)

**MAKE SURE YOU DISABLE vMenu VOICE CHAT OTHERWISE YOU WILL RUN INTO PROBLEMS**

```text
####################################
#     VOICE CHAT OPTIONS MENU      #
####################################
# To disable vMenu's voice chat options, simply remove this section completely and vMenu won't touch voice chat at all.
#add_ace builtin.everyone "vMenu.VoiceChat.Menu" allow
#add_ace builtin.everyone "vMenu.VoiceChat.All" allow
#add_ace builtin.everyone "vMenu.VoiceChat.Enable" allow
#add_ace builtin.everyone "vMenu.VoiceChat.ShowSpeaker" allow
#add_ace builtin.everyone "vMenu.VoiceChat.ShowSpeaker" allow

# Staff voice channel is restricted to moderators/admins by default.
#add_ace group.moderator "vMenu.VoiceChat.StaffChannel" allow
#add_ace group.trialModerator "vMenu.VoiceChat.StaffChannel" allow
#add_ace group.admin "vMenu.VoiceChat.StaffChannel" allow
#add_ace group.owner "vMenu.VoiceChat.StaffChannel" allow
```

**What is BadgerTools?**

_BadgerTools is a nifty script that took me a long while to perfect... It's still not perfect and I will continue to optimize it, but it's a very stable state for now. So, basically what BadgerTools is is staff administration tools. Currently it only features a /spectate and /spectate \[id\] as well as it's own custom voice chat \(15 meters voice chat by default for everyone, but can be changed with /proximity\) that replaces vMenu's voice chat. You can cycle through players on the server once in /spectate mode as well by using the left and right arrow keys on your keyboard as well. Simply type /spectate to get out of spectate mode. Whilst you are spectating a player, you can hear all the players they can hear within your /proximity specified radius from them too. You can also speak to the user you are spectating and users around them. What is special about BadgerTools voice chat? Well, you can add tags to currently speaking voice chat. BadgerTools also gets rid of voice chat color tags from a user unless they have a certain rank. It also gets rid of users who are not staff's red colors in their name._

**Screenshots** _**Spectating**_ 

![](https://i.gyazo.com/012f16d990daaefc33b1c4024eb98690.gif)

_**Voice Chat**_ As seen in the clip below, rusty-sir has colors in his username, however BadgerTools does not allow his colors to go through to the voice chat since he is not a donator. 

![](https://i.gyazo.com/83dc4b3f6ea2e2ec42139c7c51d43847.gif)

_**Freezing Players**_ 

![](https://i.gyazo.com/12cc12c435870276f3ceb7f8f13c91c2.gif)

**Permission to use BadgerTools Spectate:**

```text
BadgerTools.Commands.Spectate
```

**Configuration for tags** 

All you have to worry about for configuration purposes is this section: The first role should always be the default role, so the role ID in the first item doesn't actually matter therefore I put a 0 there to indicate it is default.

```text
roleList = {
{0, ""}, -- 1
{577661583497363456, "~g~Donator | "}, -- 3
{577631197987995678, "~r~T-Mod | "}, -- 4
{506211787214159872, "~r~Mod | "}, -- 5
{506212543749029900, "~r~Admin | "}, -- 6
{577966729981067305, "~p~Management | "}, -- 7
{506212786481922058, "~o~Owner | "}, -- 8
}
```

**Configuration for allowing colors in voice chat** 

For allowing colors in voice chat name, you use the permission:

```text
BadgerTools.Colors
```

**How to cycle spectate?** 

Use the left and right arrow keys on your keyboard to cycle between spectating all the players on your server! :\)

**Commands** 

`/proximity [distance] - Changes the proximity range of which you can speak and hear others within`

`/voicetag - Lists the voice tags you have access to (linked through the discord roles)`

`/voicetag [index] - Changes your voice tag to the one you select (where id is the index next to the voice tag in /voicetag)`

`/spectate - Start spectate cycling players`

`/spectate [id] - Spectate the player with the specified ID (this will also put you in a spectate cycle too though)`

`/tp [id] - Teleport the specified ID`

`/summon [id] - Summon the specified ID to you`

`/freeze [id] - Freeze the player so they cannot run from staff sits`

**Download** [BadgerTools](https://github.com/TheWolfBadger/BadgerTools-Revamped)

