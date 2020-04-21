# FivemDiscordPerms

## About

This project was started by Badger in March of 2020 in response to Discord disabling Fivem's API requests utilizing the RPC method they used without Discord's permission. Many FiveM servers used the discord features in script and it made life so much easier... FivemDiscordPerms aims to bring back that ease again, however has a workaround to getting users' discords.

## Images

![](https://i.gyazo.com/3d841cab3bc468e696a239e252cda78e.gif)

![](https://i.gyazo.com/28a0eca6d1edbbb6555f8fbf28b4446c.jpg)

![](https://i.gyazo.com/e75b91aa6849743658a10682444a34f9.jpg)

## How it works?

Essentially, FivemDiscordPerms has a database in which holds the information of players who join your server. You run this website along with the database and fivem script. When a player joins and does not have a database account, they will be instructed to create one as soon as they spawn in the server. We also have the option of running this website publicly for all to use, but this may cause rate-limiting, so it may be a better idea for you to run it individually for your servers only. However, in case you want the publicly available version \(no setup required besides the Fivem script\), you can find that further below including more information.

## How do I as a developer use the BadgerDiscordAPI?

 So clearly, I couldn't take over Fivem's identifiers function. I, however made the function exported named `GetDiscordIdentifier(src)` in which you pass `src` as the player source within the server-side of your script. To fully utilize this \(within a lua script, not sure about C\#, so please make a pull request on GitHub if you do\): `exports.BadgerDiscordAPI:GetDiscordIdentifier(src)`

## Installation

* There are 2 options you can choose when installing FivemDiscordPerms. You can either use my personal database and website badger.store which I made publicly available for use or you can connect this to your own database and website.

**Installing using the provided database and website:**

* If you want to just use my database and website, just put BadgerDiscordAPI's `FIVEM-SCRIPTS-FOLDER`  scripts into your FiveM server. Then all you need to do is start all of the scripts just like you would any other resource. discord\_perms as well as the other discord scripts will need to be configured to fit your own needs though.
* You will now need to fix up your server.lua of FivemDiscordPerms config section
  * You will see the following at the top of the FivemDiscordPerms server.lua

```text
port = 30120;
sitePath = 'https://badger.store/discordapi';
```

* You need to set `port` to the port that your FiveM server is running on
* Keep `sitePath` to what it is. That does NOT need to be changed

**Installing using your own assets:**

* You need to find the `config_example.php` file and rename it to `config.php` 
* You will then see a file like this shown below:

```text
<?php
global $host;
global $port;
global $database;
global $username;
global $password;
$host = '';
$port = 3306;
$database = '';
$username = '';
$password = '';
global $clientID;
global $clientSecret;
global $urlRedirect;
global $redirect_URI;
$redirect_URI = '';
$urlRedirect = '';
$clientID = '';
$clientSecret = '';
?>
```

* Now, it is time to explain the values of the `config.php` configuration file.
  * `$host` is the variable that is for your database host name
  * `$port` is the port of your SQL database
  * `$database` is the database name you have your tables located at \(more on that later\)
  * `$username` is the username you use to login to your database
  * `$password` is the password you use to login to your database
  * `$redirect_URI` is the redirecting URI you will get via making a discord application
  * `$urlRedirect` is the URL to the discord application in which they will utilize to verify they own the discord account
  * `$clientID` is the client ID of your made discord application 
  * `$clientSecret` is the client secret of your made discord application
* You now need to make a discord application to fill in the discord steps of the configuration file
  * You will first navigate to [https://discordapp.com/developers/applications](https://discordapp.com/developers/applications)
  * You will then want to make a new application
  * We suggest naming it "DiscordAPI" or something that is descriptive
  * You will then go to `OAuth2` and will want to set up redirects here
    * This is your `$redirect_URI`
  * You will then go down to `OAuth2 URL Generator` and want to select your `Redirect URL` and then click the scopes `identify` and `email` 
  * Then you will copy the link at the bottom of the page within the `Scopes` box
    * This is your `$urlRedirect` 
  * Now click `General Information` 
  * Click `Copy` under where the Client ID is shown
    * This is your `$clientID` 
  * Now `Copy` under where the Client Secret section is
    * This is your `$clientSecret` 
* After setting up the whole configuration file, you have now completed the web configuration part
* Place the whole web part of FivemDiscordPerms into your web server
* You will now need to fix up your server.lua of FivemDiscordPerms config section
  * You will see the following at the top of the FivemDiscordPerms server.lua

```text
port = 30120;
sitePath = 'https://badger.store/discordapi';
```

* You need to set `port` to the port that your FiveM server is running on
* You need to set `sitePath` to where the website that contains the index.php of FivemDiscordPerms is located
* Once you set this part up, you have now completely installed FivemDiscordPerms successfully for your personal use

