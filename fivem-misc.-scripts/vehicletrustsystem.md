# VehicleTrustSystem

**Version 1.0**

It is here everyone! The first of it's kind \(at least I think\)! A vehicle restriction script that is just for personal vehicles! You have commands such as /trust, /untrust to trust and untrust players to use the vehicle you own.

This all works via a file called whitelist.json and it keeps track of every player's vehicles they are allowed to drive! If you run a huge huge server, this may not be the resource for you unless you have a developer capable of moving it to a database storage system... Other than that, this resource runs well for the smaller servers. I may look into adding an SQL option in the future though.

### For all your hosting needs

![Iceline Hosting](https://i.gyazo.com/24c65c27acc53ce0656cda7e7ed29230.gif)

#### Use code `BADGER15` at [https://iceline-hosting.com/billing/aff.php?aff=284](https://iceline-hosting.com/billing/aff.php?aff=284) for `15% off` your first month of any service \(excluding dedicated servers\)

If they do not have access to your personal vehicle?: 

![](https://i.gyazo.com/224097368c55014475e89f25299d03ea.gif)

Some examples of messages gotten by running commands: 

![](https://i.gyazo.com/f982903a9c8deb6bee619340f4c8c9ce.png)

* **Commands**

`/trust [playerID] [spawncode] = Trust the specified player to your vehicle if you own it.`

`/untrust [playerID] [spawncode] = Opposite of /trust... Lol..`

`/vehicles = List the vehicles you have access to utilize`

![](https://i.gyazo.com/d89b1a0c98572b0bdcc2561d7d6a1dfd.png)

* **Admin Commands**

`/setOwner [playerID] [spawncode] = Set the owner of a personal vehicle`

`/clear [spawncode] = Gets rid of all the specified vehicle's data in case you messed up setOwner`

* **Permissions**

This gives permission to run Admin commands:

```text
add_ace group.admin VehwlCommands.Access allow
```

* **Download**

[VehicleTrustSystem](https://github.com/TheWolfBadger/VehicleTrustSystem)

