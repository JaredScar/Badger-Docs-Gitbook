# Fivem Keybase Anticheat

## Version 1.0

### How it works

Essentially this script protects your server events from being triggered by others from the client side of scripts \(people with Lua executors\). You will give the server events passwords, then to trigger the event, you must run it through the Keybase-Anticheat so it will verify it as a valid event triggered by you on the server-side. This is very useful considering nobody can exploit it from the client-side as they will not know the key you set for the event.

### Configuration

```text
ProtectedServerEvents = {
	{'KB-AC:UnprotectedExample:OOC', 'KEY-FOR-EVENT'},
	{'EVENT', 'KEY-FOR-EVENT'},
	{'EVENT', 'KEY-FOR-EVENT'},
	{'EVENT', 'KEY-FOR-EVENT'},
	{'EVENT', 'KEY-FOR-EVENT'},
}
BlacklistedServerEvents = {
  "antilynxr4:detect",
  "ynx8:anticheat",
  "antilynx8r4a:anticheat",
  "lynx8:anticheat",
}
```

* You'll see this configuration section above within the `server.lua` of Keybase-Anticheat
* You'll want to put the event name within `'Event'` and then the password/key you want for the event where `KEY-FOR-EVENT` is
* `BlacklistedServerEvents` is a list of popular server events hackers trigger with their common Lua executors when joining servers and/or on servers
  * You'll want to add more events to this list
  * Only add events here that don't actually exist, but are known to be events hackers will commonly trigger
    * You can find more of these possible events here: [https://gist.github.com/d0p3t/1ad255374d68fcc3f252e13015b028cb](https://gist.github.com/d0p3t/1ad255374d68fcc3f252e13015b028cb)
* Once you set all of these up, you'll then need to know how to trigger your events within your script

### How to trigger my events?

* Now you have set up a protection for triggering your server events, but how do you make your server events valid? You do this by going through the Keybase-Anticheat API
* We will show an example using the event in the first line of our configuration above
* We will use `{'KB-AC:UnprotectedExample:OOC', 'KEY-FOR-EVENT'},` 
* We want to trigger this event
* We would do the following to successfully trigger the server event without setting off our Anticheat

```text
TriggerEvent('KB-AC:TriggerServerEvent', 'KEY-FOR-EVENT', 'KB-AC:UnprotectedExample:OOC', table.concat(args, ' '))
```

* By doing it this way, we passed the key for the event, then this lets the Anticheat know it is a valid event being used

### Download

{% embed url="https://github.com/TheWolfBadger/Fivem-Keybase-Anticheat" %}



