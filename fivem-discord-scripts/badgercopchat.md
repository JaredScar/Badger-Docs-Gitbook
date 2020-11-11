# BadgerCopChat

## Version 1.0

This is a pretty simple script, but cool one also. It utilizes a player's discord roles to determine if they are a LEO or not. If they are within the roleList, then they are considered to be a LEO and will have access to use the /leoChat commands.

### For all your hosting needs:

![Iceline Hosting](https://i.gyazo.com/24c65c27acc53ce0656cda7e7ed29230.gif)

#### Use code `BADGER15` at [https://iceline-hosting.com/billing/aff.php?aff=284](https://iceline-hosting.com/billing/aff.php?aff=284) for `15% off` your first month of any service \(excluding dedicated servers\)

### Requirements

{% embed url="https://github.com/JaredScar/Badger\_Discord\_API" %}

### Configuration

```text
roleList = {
1, -- National Guardsmen
1, -- SASP 
1, -- LSPD 
1, -- Fire/EMS Department
}
prefix = '^0[^3LEO Chat^0] ^r';
```

* You will want to replace the 1s with the roleIDs of your respective discord LEO roles. I placed a few common LEO roles as comments next to the 1s for terms of a structure. Keep in mind, you can change all of this, you can also add more roles to this by just adding the roleIDs with commas after them within the `{}` of the roleList
* You can change `prefix` to anything you want, as this will just be the prefix the script displays in front of every message it sends

### Commands

`/leoChat` - Toggles on and off LEO Chat

`/leoChat on` - Turns LEO Chat on

`/leoChat off` - Turns LEO Chat off

`/leoChat vis` - Toggles on and off the visibility of seeing LEO Chat messages from others

### Pictures

![](https://i.gyazo.com/6d5170b5a2e774ff49bea36274d03592.png)

### Download

{% embed url="https://github.com/TheWolfBadger/BadgerCopChat" %}

