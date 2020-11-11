# DiscordReports

## Version 1.0

### What is it?

DiscordReports is a script I made way back in August of 2019, but I never actually got around to releasing it. I know there is another discord report script on the forums made by my old good friend @ApolloCore which you can find below. However, my script is a little different in the way it works and has some quite unique features I thought would be useful. So therefore in my quest to become the \#1 open source developer on GitHub, I am releasing it today for your use cases. Jokes aside, it's a really cool and nifty script that can really help you staffing your server.

{% embed url="https://forum.cfx.re/t/release-discord-integration-simple-player-report-system-w-discord-webhook/630392" %}

### For all your hosting needs

![Iceline Hosting](https://i.gyazo.com/24c65c27acc53ce0656cda7e7ed29230.gif)

#### Use code `BADGER15` at [https://iceline-hosting.com/billing/aff.php?aff=284](https://iceline-hosting.com/billing/aff.php?aff=284) for `15% off` your first month of any service \(excluding dedicated servers\)

### Badger's Discord Community

[![Developer Discord](https://discordapp.com/api/guilds/597445834153525298/widget.png?style=banner4)](https://discord.com/invite/WjB5VFz)

### Images

![Report Sent Confirmation](https://i.gyazo.com/de1029ba48dc4b05d40993bf64a16add.png)

![Discord Webhook Report \[displayIdentifiers = true\]](https://i.gyazo.com/54a7edea9d7fb280c9b0c982e6403ae2.png)

![Discord Webhook Report \[displayIdentifiers = false\]](https://i.gyazo.com/a39666deca623de7df24bc0db99fc9b8.png)

![What a staff member will see --- \(Reporter Name\) \[ID Reported\]](https://i.gyazo.com/54dac4c18706dbdeda6830656c0508fa.png)

### Installation

* You will need to find the configuration section within the `server.lua`
* You will see the below block of code
* You can choose to put `displayIdentifiers` as `true` or `false`
  * Refer to above `Images` of what this will do 
* You also need to set up the `webhookURL` for where the script will post the reports within Discord
  * Refer to [https://docs.badger.store/fivem-general-help/setting-up-a-discord-webhook](https://docs.badger.store/fivem-general-help/setting-up-a-discord-webhook)
* You will need to give your staff group's the permission `BadgerReports.See` in order to see the action reports within the server
  * Refer to [https://docs.badger.store/fivem-general-help/ace-permissions](https://docs.badger.store/fivem-general-help/ace-permissions)

```text
-- Config --
webhookURL = ''
displayIdentifiers = true;
```

### Download

{% embed url="https://github.com/TheWolfBadger/DiscordReports" %}

