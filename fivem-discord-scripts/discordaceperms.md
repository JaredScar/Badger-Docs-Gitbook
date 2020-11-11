# DiscordAcePerms

## **Version 1.0**

This is another one of my discord scripts! :\) If used properly along with my other scripts, you can fully make your server use only discord roles for permissions and chat roles ;\)

### For all your hosting needs:

![Iceline Hosting](https://i.gyazo.com/24c65c27acc53ce0656cda7e7ed29230.gif)

#### Use code `BADGER15` at [https://iceline-hosting.com/billing/aff.php?aff=284](https://iceline-hosting.com/billing/aff.php?aff=284) for `15% off` your first month of any service \(excluding dedicated servers\)

## **Requirement**

{% embed url="https://github.com/JaredScar/Badger\_Discord\_API" %}

## **Installation Tutorial**

{% embed url="https://youtu.be/UUzSdQtJE4s" %}

The permissions for a user update after every restart when they first login \(so long as they have the discord role ID associated with the group in the list\).

Example of how to set it up:

```text
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
5. Enjoy ![:slight\_smile:](https://forum.cfx.re/images/emoji/twitter/slight_smile.png?v=9)

## **Download**

 ****[DiscordAcePerms](https://github.com/TheWolfBadger/DiscordAcePerms)

