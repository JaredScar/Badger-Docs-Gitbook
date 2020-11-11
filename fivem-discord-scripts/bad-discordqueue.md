# Bad-DiscordQueue

### All I ask

All I ask is that if you enjoy this resource, please give it a like on the forum page, on GitHub \(if you have an account\), and pop me a follow over on GitHub.

### What is it?

This is basically a discord queue for logging into a server. When you connect to the server, you get added to a queue. Depending on your priority, you can be at the back of the queue or added to the top automatically. This all depends on what discord roles you have considering it works off of priority numbers. I'm not the best at writing descriptions. I'll be honest, I personally am probably not going to use this script, but I had a lot of people request this script from me, so here it is. Why not increase my rep within the Fivem community?

### For all your hosting needs

![Iceline Hosting](https://i.gyazo.com/24c65c27acc53ce0656cda7e7ed29230.gif)

#### Use code `BADGER15` at [https://iceline-hosting.com/billing/aff.php?aff=284](https://iceline-hosting.com/billing/aff.php?aff=284) for `15% off` your first month of any service \(excluding dedicated servers\)

### Badger's Discord Community

[![Developer Discord](https://discordapp.com/api/guilds/597445834153525298/widget.png?style=banner4)](https://discord.com/invite/WjB5VFz)

### Installation

{% embed url="https://youtu.be/UUzSdQtJE4s" %}

### Dependencies

{% embed url="https://github.com/JaredScar/Badger\_Discord\_API" %}

### Screenshots

![Queue Gif](https://i.gyazo.com/3606be50c8770850b86a83fd8efbec18.gif)

### Configuration

```text
Config = {
	Default_Prio = 500000, -- This is the default priority value if a discord isn't found
	AllowedPerTick = 1, -- How many players should we allow to connect at a time?
	HostDisplayQueue = true,
	onlyActiveWhenFull = true,
	Displays = {
		Prefix = '[BadgerDiscordQueue]',
		ConnectingLoop = { 
			'🦡🌿🦡🌿🦡🌿',
			'🌿🦡🌿🦡🌿🦡',
			'🦡🌿🦡🌿🦡🥦',
			'🌿🦡🌿🦡🥦🦡',
			'🦡🌿🦡🥦🦡🥦',
			'🌿🦡🥦🦡🥦🦡',
			'🦡🥦🦡🥦🦡🥦',
			'🥦🦡🥦🦡🥦🦡',
			'🦡🥦🦡🥦🦡🌿',
			'🥦🦡🥦🦡🌿🦡',
			'🦡🥦🦡🌿🦡🌿',
			'🥦🦡🌿🦡🌿🦡',
		},
		Messages = {
			MSG_CONNECTING = 'You are being connected [{QUEUE_NUM}/{QUEUE_MAX}]: ', -- Default message if they have no discord roles 
			MSG_CONNECTED = 'You are up! You are being connected now :)'
		}
	}
}

Config.Rankings = {
	-- LOWER NUMBER === HIGHER PRIORITY 
	-- ['roleID'] = {rolePriority, connectQueueMessage},
	['1'] = {500, "You are being connected (donate for a better priority) [{QUEUE_NUM}/{QUEUE_MAX}]:"}, -- Discord User 
	['1'] = {400, "You are being connected (Donator Queue) [{QUEUE_NUM}/{QUEUE_MAX}]:"}, -- Donator 
	['1'] = {300, "You are being connected (Trial-Mod Queue) [{QUEUE_NUM}/{QUEUE_MAX}]:"}, -- Trial Mod 
	['1'] = {200, "You are being connected (Mod Queue) [{QUEUE_NUM}/{QUEUE_MAX}]:"}, -- Mod 
	['1'] = {100, "You are being connected (Admin Queue) [{QUEUE_NUM}/{QUEUE_MAX}]:"}, -- Admin 
	['1'] = {1, "You are being connected (Management Queue) [{QUEUE_NUM}/{QUEUE_MAX}]:"}, -- Management
}
```

* Replace the `'1'`s in the configuration with the discord role ID you want to set up priority for 

### Download

{% embed url="https://github.com/JaredScar/Bad-DiscordQueue" %}

