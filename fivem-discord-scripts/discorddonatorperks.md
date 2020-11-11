# DiscordDonatorPerks

## Version 1.0

### What is it?

DiscordDonatorRanks is a script I made for my server to give some perks to players who were part of the Tebex/Patreon subscription helping to keep us paying for the server. I wanted to give something to those players every month, but didn't want extra work for my staff to have to do. So, with DiscordDonatorRanks, it essentially automates the process of giving money and/or jobs in-game to players depending on their discord roles. It'll then save them to the database and they will not be able to access the perks for another 30 days \(essentially a whole month, maybe down the line I'll make it an official month no matter what month it is\). It's a quite simple script and I'm honestly surprised I haven't found one like it.

### For all your hosting needs

![Iceline Hosting](https://i.gyazo.com/24c65c27acc53ce0656cda7e7ed29230.gif)

#### Use code `BADGER15` at [https://iceline-hosting.com/billing/aff.php?aff=284](https://iceline-hosting.com/billing/aff.php?aff=284) for `15% off` your first month of any service \(excluding dedicated servers\)

### Badger's Discord Community

[![Developer Discord](https://discordapp.com/api/guilds/597445834153525298/widget.png?style=banner4)](https://discord.com/invite/WjB5VFz)

### Images

![](https://i.gyazo.com/3c32592dc1dc38fce373f45f549e0547.gif)

### Requirements

{% embed url="https://github.com/sadboilogan/discord\_perms" %}

{% embed url="https://github.com/brouznouf/fivem-mysql-async" %}

### Installation

* Find the `insert.sql` file and insert its code into your essentialmode database. \(The same database you are using for ESX\)

**Insert.sql:**

```text
CREATE TABLE IF NOT EXISTS Donator_Data 
(
	id INTEGER(11) AUTO_INCREMENT PRIMARY KEY,
	identifier VARCHAR(50),
	playerName VARCHAR(50),
	dateReceiveNext INTEGER(64),
	acceptedPerkID INTEGER(11),
	rankPackage VARCHAR(50),
);
```

* After setting up the `Donator_Data` table within your database, you will then want to move onto configuring `discord_perms` and `DiscordDonatorPerks` configs

{% embed url="https://www.youtube.com/watch?v=sjbFzkII2T0" %}

### Configuration

```text
roleList = {
	{"Bronze-Tier", 1, {"$1,000,000 voucher", {'Money', 1000000}} 
	}, -- Bronze Tier 
	{"Silver-Tier", 1, {"$5,000,000 voucher",{'Money', 5000000}} 
	}, -- Silver Tier 
	{"Gold-Tier", 1, 
		{"$15,000,000 voucher",{'Money', 15000000}}, 
		{"Invitation to Mafia [Gang]", {'Job', 'mafia', 0}},
		{"Invitation to LS Kings [Gang]", {'Job', 'woodyguns', 0}},
		{"Invitation to Sons of Anarchy [Gang]", {'Job', 'lazy', 0}},
		{"Invitation to Black Diamond Cartel [Gang]", {'Job', 'stevestacos', 0}}
	}, -- Gold Tier 
}
```

* It's now time to understand how the configuration works
* `{"$1,000,000 voucher", {'Money', 1000000}}` is what I like to call a `Offer` 
* `Offers` are basically what the player will be offered in-game on their character to accept or deny
* The `Offers` can be seen above in `Images` in which it asks the player whether they want to accept or reject
* **How do we set up a job for `Silver Tier` ?**
  * We first need to set it up correctly, so we need to add another `Offer` to it
  * You'll notice below that we added a job to `Silver Tier` simply by adding the `,` and correct format of jobs being `{"Invitation to Job", {'Job', 'jobname', 0}}` 
  * `"Invitation to Job"` is known as the `Label` and will be displayed on the player's screen asking if they want to accept or reject it 
  * `{'Job', 'jobname', 0}` is known as the `Job-Details` in which the script will use to give them the job if they accept it
  * `'Job'` is the identifier of what type of `Offer` it is
  * `'jobname'` is the name of the job \(the one you use to set players to work for it\)
  * `0` is known as the `Job-Grade` in which is the level of the job they will obtain when accepting the `Offer` 

```text
{"Silver-Tier", 1, 
    {"$5,000,000 voucher",{'Money', 5000000}},
    {"Invitation to Job", {'Job', 'jobname', 0}}
	}, -- Silver Tier 
```

* **How do we set up another money voucher for `Silver Tier` ?**

  * We once again need to add another `Offer` to it
  * You'll notice below we have the `Label` as `"$100,000 voucher"`
  * We have the `Money-Details` as `{'Money', 100000}`

  ```text
  {"Silver-Tier", 1, 
      {"$5,000,000 voucher",{'Money', 5000000}},
      {"Invitation to Job", {'Job', 'jobname', 0}},
      {"$100,000 voucher", {'Money', 100000}}
  	}, -- Silver Tier 
  ```

* We want to replace the `1`s within the `server.lua` with the roleIDs of the corresponding rank you want in that spot
* If you're familiar with my work, the roleList should come as no surprise to you lol...
* **Note:** Currently \(as of version 1.0\), accepting and denying jobs will put the job in the database because we don't want it asking them for joining the jobs every other time they login. In the future I'll hopefully make a command such as /select for selecting a job from where they got invitations to, so they can switch.
* **Another Note:** What this means is, when the player first logins, they need to select the character they want the job on first \(if they have a job perk\), then accept it and deny the others on it. If they want the money on another account, they can just deny it and accept it the next time they login with the other character.

### Download

{% embed url="https://github.com/TheWolfBadger/DiscordDonatorPerks" %}

