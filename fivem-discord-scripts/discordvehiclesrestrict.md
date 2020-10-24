# DiscordVehiclesRestrict

## DiscordVehiclesRestrict

This is a Discord Vehicle Restriction script that restricts vehicles to certain roles with discord. This idea came about because of FAXES DiscordVehicleWhitelist. I have gotten permission from FAXES to add onto his script and make it possible to restrict vehicle use to only certain roles within Discord.

The permissions update every respawn for a player :\)

### Download

[DiscordVehiclesRestrict](https://github.com/TheWolfBadger/DiscordVehicleWhitelist)

### How to Install

**Requirement**

{% embed url="https://github.com/JaredScar/Badger\_Discord\_API" %}

### Setup

1. The 1s must be replaced with IDs of the roles within your discord
2. The order of the roles need to match up with the restrictedVehicles list within the client.lua:
3.   ```text
   --- Config ---

   --[[
       REPLACE THE '1's WITH YOUR DISCORD ROLES' IDs
   ]]
   -- THESE NEED TO BE THE RESPECTIVE ROLE IDs OF YOUR DISCORD ROLES:
   roleList = {
   1, -- Civ
   1, -- Trusted Civ
   }
   ```

