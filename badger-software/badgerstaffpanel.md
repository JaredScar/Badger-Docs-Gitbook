# BadgerStaffPanel

## Setting up BadgerStaffPanel

### Discord Application Configuration

```text
<?php
$clientID = '{CLIENT-ID}';
$clientSecret = '{CLIENT-SECRET}';
$redirect_URI = '{REDIRECT-URI}';
$guildID = '{GUILD-ID}';
$discordRedirectAuth = '{DISCORD-REDIRECT-AUTH}';
$botToken = '{BOT-TOKEN}';
```

* Navigate to [https://discordapp.com/developers/applications](https://discordapp.com/developers/applications) 

![](../.gitbook/assets/image%20%281%29.png)

* Click on `New Application` then name the bot what you would like

![](../.gitbook/assets/image%20%282%29.png)

* Click `Copy` under the `Client ID` on the page. Then replace `{CLIENT-ID}` within the `config.php` file
* Click `Copy` under the `Client Secret` on the page. Then replace the `{CLIENT-SECRET}` within the `config.php` file
* Click on `OAuth2` within the side navigation bar
* Add your website's URL as a redirect, for example we will use `http://localhost` for a locally hosted website
* You will then want to generate a discord authorization link
* To do this, navigate down to the `OAuth2 URL Generator` section, then select our `http://localhost` redirect URL
* Now we choose the options we need for the authorization URL, select `identify`, `email`, and `guilds` 

![](../.gitbook/assets/image%20%283%29.png)

* Now you will want to click the `Copy` button and copy the huge link that has been generated
* Now we go back into our `config.php` file again

```text
$redirect_URI = '{REDIRECT-URI}';
$guildID = '{GUILD-ID}';
$discordRedirectAuth = '{DISCORD-REDIRECT-AUTH}';
$botToken = '{BOT-TOKEN}';
```

* You now want to submit `http://localhost` where `{REDIRECT-URI}` is located
* You then want to submit the huge link you copied in the previous step and replace `{DISCORD-REDIRECT-AUTH}` with it
* You now need to get the guild ID of your discord server
* You will first turn on the developer mode in Discord to be able to do this \(check below GIF\)

![](https://i.gyazo.com/c6306c90a976361e2e1e3d4fc09f4d21.gif)

* Now you will need to copy your server's guild ID \(check below GIF\)

![](https://i.gyazo.com/0da39238b6975994e1c7272755a7ca0c.gif)

* Now replace `{GUILD-ID}` with the guild ID you just got through your discord application
* We now need to create a discord bot, navigate to `Bot` on the side navigation
* Create the discord bot, confirm creating it
* Now, click `Copy` and get the discord bot token
* Replace`{BOT-TOKEN}` within the `config.php` file with the token you had just copied
* Invite the discord bot to your server now by going to the `OAuth2` on the side navigation

![](../.gitbook/assets/image%20%284%29.png)

* Click `Copy` and then enter the URL in a browser, then invite this bot to your discord server
* You have now completed the discord application configuration section of BadgerStaffPanel 

### Server API Configuration

```text
$serverIP = '{SERVER-IP}';
$port = 80; // Website port
$steamAPIkey = '{STEAM-API-KEY}';
$server_port = 30120;
$rconPassword = '{RCON-PASSWORD}';
$serverName = '{SERVER-NAME}';
```

* Replace `{SERVER-IP}` with the server IP of your server
* Replace `80` with the port your website runs on \(for most websites, the default port is port 80\)
* Replace `{STEAM-API-KEY}` with the steam API key you get from a key you get from [https://steamcommunity.com/dev/apikey](https://steamcommunity.com/dev/apikey)
* Replace `30120` with the port of your FiveM server \(for most servers, the default port is 30120\)
* Replace `{RCON-PASSWORD}` with the RCON password within your `server.cfg` file 
* Replace `{SERVER-NAME}` with your server's name
* You have now completed the server API configuration section of BadgerStaffPanel

### SQL Configuration

```text
// SQL INFO
$host = '';
$username = '';
$password = '';
$db = '';
$port = 3306;
```

### Website Permissions Configuration

```text
$permissionsSetup = [
    '{T-MOD-RANK}' => [// Start T-Mod
        'Permission.Note',
        'Permission.Warn',
        'Permission.Kick',
        'Permission.RemoveNote',
        'Permission.RemoveWarn',
    ], // End T-Mod
    '{MOD-RANK}' => [// Start Mod
        'Permission.Note',
        'Permission.Warn',
        'Permission.Kick',
        'Permission.Tempban',
        'Permission.Ban',
        'Permission.RemoveNote',
        'Permission.RemoveWarn',
        'Permission.RemoveKick',
        'Permission.RemoveTempban',
    ], // End Mod
    '{ADMIN-RANK}' => [ // Start Admin
        'Permission.Note',
        'Permission.Warn',
        'Permission.Kick',
        'Permission.Tempban',
        'Permission.Ban',
        'Permission.RemoveNote',
        'Permission.RemoveWarn',
        'Permission.RemoveKick',
        'Permission.RemoveTempban',
        'Permission.RemoveBan',
    ], // End Admin
    '{MANAGEMENT-RANK}' => [ // Start Management
        'Permission.Note',
        'Permission.Warn',
        'Permission.Kick',
        'Permission.Tempban',
        'Permission.Ban',
        'Permission.RemoveNote',
        'Permission.RemoveWarn',
        'Permission.RemoveKick',
        'Permission.RemoveTempban',
        'Permission.RemoveBan',
    ], // End Management
];
```

* Replace `{T-MOD-RANK}` with the role ID of the T-Mod rank in your discord server
* Replace `{MOD-RANK}` with the role ID of the Mod rank in your discord server
* Replace `{ADMIN-RANK}` with the role ID of the Admin rank in your discord server
* Replace `{MANAGEMENT-RANK}` with the role ID of the Management rank in your discord server

