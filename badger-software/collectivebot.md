# CollectiveBot

## Installation

* Navigate to [https://discordapp.com/developers/applications](https://discordapp.com/developers/applications) 

![](https://i.gyazo.com/0c17de9c4829923b00be6582d63149f8.png)

* Click on `New Application` then name the bot what you would like \(however `CollectiveBot` makes the most sense\)

![](https://i.gyazo.com/b318fc46b86f4d18d479c157b900e6a4.png)

* Click on `Bot` on the side bar

![](https://i.gyazo.com/5bc9274b7df8cb3e94f883c52a3839a3.png)

* Click on `Add Bot`

![](https://i.gyazo.com/f182331bac6513777b4c8781bd4e2764.png)

* Click on `Copy` to copy your token
* Navigate to [https://github.com/TheWolfBadger/CollectiveBot/releases](https://github.com/thewolfbadger/collectivebot/releases) and download the latest release
* Extract the .zip file you download
* Navigate to the config.yml within the now extracted directory
* You should see something like this:

```text
#######################
###  CollectiveBot  ###
###       by        ###
###     Badger      ###
#######################
BotToken: ''
Enables:
  SuggestionsAddon: true
  WelcomeMessage: true
SuggestionAcceptEmoji: ':YesEmoji:'
SuggestionDenyEmoji: ':NoEmoji:'
SuggestionApprovedEmoji: ':ApprovedEmoji:'
SuggestionDeniedEmoji: ':DeniedEmoji:'
SuggestionChannels:
  - '693985384907931719'
SuggestionDeniedChannel: '695294976908722229'
SuggestionApprovedChannel: '695294976908722229'
SuggestionRoles: # These are the roles that are allowed to approve and/or deny suggestions
  - '693833282240118794'

WelcomeMessage:
  Title: 'Welcome {USER-TAG} to Project Badger'
  TitleLink: ''
  Description: "**You're member #{MEMBER-COUNT} :tada:**"
  Footer: 'CollectiveBot by Badger'
  FooterIMG: 'https://i.gyazo.com/981a86c82860fc5ae5859bcd1bb0df09.gif'
  Thumbnail: '{USER-AVATAR}'
  Channel: '693836887651254283'
  Color: '0 254 0'
```

* You now will want to place that token you copied and place it into the `''` that comes after `BotToken:` 
* After doing this, save the config.yml file
* Go back to the applications page of the discord developers site
* Click on `OAuth2` 

![](https://i.gyazo.com/e52825f0f3a4f9bc471533eeeb235d7f.gif)

* Do exactly as is done in the GIF on the `OAuth2` 
* Paste this link you just copied into your browser, then invite the bot to your discord server you'd like the bot on
* You can invite this bot to as many servers as you'd like, however you will need to set up configurations for roles for each different server you add it to
* After doing all of this, you will have the bot properly set up to run and work on your server.
* All you need to do is click `start_CollectiveBot.bat` file to start up the bot

## Configuring Permissions via RoleIDs in config.yml

* You will now navigate to the `config.yml` file and open it
* We now need to understand how the configuration works

```text
#######################
###  CollectiveBot  ###
###       by        ###
###     Badger      ###
#######################
BotToken: ''
Enables:
  SuggestionsAddon: true
  WelcomeMessage: true
SuggestionAcceptEmoji: ':YesEmoji:'
SuggestionDenyEmoji: ':NoEmoji:'
SuggestionApprovedEmoji: ':ApprovedEmoji:'
SuggestionDeniedEmoji: ':DeniedEmoji:'
SuggestionChannels:
  - '693985384907931719'
SuggestionDeniedChannel: '695294976908722229'
SuggestionApprovedChannel: '695294976908722229'
SuggestionRoles: # These are the roles that are allowed to approve and/or deny suggestions
  - '693833282240118794'

WelcomeMessage:
  Title: 'Welcome {USER-TAG} to Project Badger'
  TitleLink: ''
  Description: "**You're member #{MEMBER-COUNT} :tada:**"
  Footer: 'CollectiveBot by Badger'
  FooterIMG: 'https://i.gyazo.com/981a86c82860fc5ae5859bcd1bb0df09.gif'
  Thumbnail: '{USER-AVATAR}'
  Channel: '693836887651254283'
  Color: '0 254 0'
```

* The keys for most of the configuration are pretty straight forward
* `SuggestionRoles` is a list in which you can add multiple roleIDs under and they will be able to move suggestions to the approved and denied channels by adding the approved or denied emoji to the suggestion
* `SuggestionChannels` is a list in which you can add multiple suggestion channel-IDs and they will then automatically be given an AcceptEmoji and DenyEmoji when a message is posted within that channel

{% hint style="info" %}
**Any further questions and/or concerns?**

You may gather more support personally and from other members of the Badger Developer Community over [here](https://discord.gg/Rmzgwpn).
{% endhint %}

