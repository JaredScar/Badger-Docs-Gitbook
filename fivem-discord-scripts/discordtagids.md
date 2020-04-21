# DiscordTagIDs

**Version 1.0**

Yes yes I know... I only make discord-based scripts. Well, you're damn welcome!

This is a script that added prefixes to ID tags above players :\) by using fully discord roles thanks to IllusiveTea!

I also wanna give thanks to MrDaGree for originally creating the script this was adapted onto! You can find that here, [https://forum.cfx.re/t/release-changed-player-name-tags-distance-names/19204](https://forum.cfx.re/t/release-changed-player-name-tags-distance-names/19204)

You must have this installed and properly working for this script to work --&gt; [https://forum.cfx.re/t/discord-roles-for-permissions-im-creative-i-know/233805](https://forum.cfx.re/t/discord-roles-for-permissions-im-creative-i-know/233805)

**Installation Tutorial** 

{% embed url="https://www.youtube.com/watch?v=sjbFzkII2T0" %}

{% embed url="https://www.youtube.com/watch?v=xDfyGcqX5sA" %}

**Commands:** `/tag-toggle - Turns off the prefix from being shown for the player (if they have a prefix in their tag)` 

`/tags-toggle - Turns off all tags from being shown above other players for ONLY yourself (good for streamers and/or pictures)` 

`/headtag - Check what Head-Tags you have access to and change them with /headtag [id]`

Running /headtag: ![](https://i.gyazo.com/66e55c315a0ad4830109ff0475804010.png)

On /tag-toggle not being active: ![](https://i.gyazo.com/07766951b02108c7ea49f8cbe2f372cd.png)

On /tag-toggle being active: ![](https://i.gyazo.com/b0249df9842dd7011c231d4deaf54fc7.png)

On /tags-toggle for tags not being active: ![](https://i.gyazo.com/6ba28b6e653f3c7bf82e90c3690a2dc5.png)

On /tags-toggle for tags being active: ![](https://i.gyazo.com/e3e9656dc5cc0faf42fb3c857106ee72.png)

How does the tags look on players? Let's have a look :\)

![](https://i.gyazo.com/253bc5c2bb10731cb870f1eb6f8893b4.jpg) ![](https://cdn.discordapp.com/attachments/577615878607077380/588710494483775508/unknown.png)

The 1s in this part of the server.lua file must be replaced with the IDs of your discord roles that are equal to the prefix you have associated with it:

```text
roleList = {
{0, "~w~"}, -- Regular Civilian / Non-Staff
{1, "~r~STAFF ~w~"}, --[[ T-Mod ]]-- 
{1, "~r~STAFF ~w~"}, --[[ Moderator ]]--
{1, "~r~STAFF ~w~"}, --[[ Admin ]]--
{1, "~p~MANAGEMENT ~w~"}, --[[ Management ]]--
{1, "~o~OWNER ~w~"}, --[[ Owner ]]--
}
```

**Download** [DiscordTagIDs](https://github.com/TheWolfBadger/DiscordTagIDs)

