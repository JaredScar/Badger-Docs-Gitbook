# SimpleRoleBot

## Installation

* Navigate to [https://discordapp.com/developers/applications](https://discordapp.com/developers/applications) 

![](https://i.gyazo.com/0c17de9c4829923b00be6582d63149f8.png)

* Click on `New Application` then name the bot what you would like \(however `SimpleRoleBot` makes the most sense\)

![](https://i.gyazo.com/b318fc46b86f4d18d479c157b900e6a4.png)

* Click on `Bot` on the side bar

![](https://i.gyazo.com/5bc9274b7df8cb3e94f883c52a3839a3.png)

* Click on `Add Bot`

![](https://i.gyazo.com/f182331bac6513777b4c8781bd4e2764.png)

* Click on `Copy` to copy your token
* Navigate to [https://github.com/TheWolfBadger/SimpleRoleBot/releases](https://github.com/TheWolfBadger/SimpleRoleBot/releases) and download the latest release
* Extract the .zip file you download
* Navigate to the config.yml within the now extracted directory
* You should see something like this:

```text
#############################
###     SimpleRoleBot     ###
###      created by       ###
###        Badger         ###
#############################
BotToken: ''
RoleConfiguration:
  693833984173408328: # Staff Role
    - '*' # All Permission for every role below their highest role
  693901091678716006: # National Guard OIC
    - '694065977398132738' # National Guard HC
    - '694065982565515265' # National Guard FTO
    - '694065982565515265' # National Guard Recruiter
    - '694065988206985244' # Military Police
    - '694065994850762794' # Civilian Contractor NG
    - '693900886535307346' # National Guardsmen
  694065977398132738: # National Guard HC
    - '694065982565515265' # National Guard FTO
    - '694065982565515265' # National Guard Recruiter
    - '694065988206985244' # Military Police
    - '694065994850762794' # Civilian Contractor NG
    - '693900886535307346' # National Guardsmen
  693856860750479371: # CHP Commissioner
    - '694648106117103728' # CHP High Command
    - '694648102300287187' # CHP Deputy Commissioner
    - '694648103193804902' # CHP FTO Evaluation Specialist
    - '694648104409890897' # CHP Patrol Administration
    - '694648107018879008' # CHP Assistant Commissioner
    - '694648108671434902' # CHP Chief
    - '694648110437236766' # CHP Colonel
    - '694648111418835076' # CHP Lieutenant Colonel
    - '694648113520181297' # CHP Major
    - '694648114438602804' # CHP Captain
    - '694649104801988618' # CHP Lieutenant
    - '694649105552638043' # CHP Staff Sergeant
    - '694649106391629914' # CHP Supervisor
    - '694649106894815252' # CHP Sergeant
    - '694649107943260170' # CHP Corporal
    - '694649108765343786' # CHP Patrol FTO
    - '694649108778188871' # Trooper First Class
    - '694649109922971669' # Trooper
    - '694649111995220560' # Probationary Trooper
    - '694649112544673850' # CHP Application Handler
    - '694649758584930404' # CHP Recruitment Team
    - '694678105503039519' # CHP Supervisor
    - '693856967445446656' # CHP
  694648106117103728: # CHP High Command
    - '694648102300287187' # CHP Deputy Commissioner
    - '694648103193804902' # CHP FTO Evaluation Specialist
    - '694648104409890897' # CHP Patrol Administration
    - '694648107018879008' # CHP Assistant Commissioner
    - '694648108671434902' # CHP Chief
    - '694648110437236766' # CHP Colonel
    - '694648111418835076' # CHP Lieutenant Colonel
    - '694648113520181297' # CHP Major
    - '694648114438602804' # CHP Captain
    - '694649104801988618' # CHP Lieutenant
    - '694649105552638043' # CHP Staff Sergeant
    - '694649106391629914' # CHP Supervisor
    - '694649106894815252' # CHP Sergeant
    - '694649107943260170' # CHP Corporal
    - '694649108765343786' # CHP Patrol FTO
    - '694649108778188871' # Trooper First Class
    - '694649109922971669' # Trooper
    - '694649111995220560' # Probationary Trooper
    - '694649112544673850' # CHP Application Handler
    - '694649758584930404' # CHP Recruitment Team
    - '694678105503039519' # CHP Supervisor
    - '693856967445446656' # CHP
  693857216725516299: # Sheriff
    - '694654347962876035' # SO High Command
    - '694653003184996423' # Chief Deputy
    - '694653005194199041' # Colonel
    - '694653007698198630' # Major
    - '694653017378521098' # Captain
    - '694653009552211988' # Lieutenant
    - '694653011569541140' # Sergeant
    - '694653013259845723' # Corporal
    - '694653015176773693' # Master Deputy
    - '694653019253506078' # Senior Deputy
    - '694653022525194372' # Deputy
    - '694653021019439174' # Probationary Deputy
    - '694735836456943666' # SO Awaiting Training
    - '694654349309378620' # SO FTO
    - '694654352052322384' # SO Application Handler
    - '694654353763598336' # SO Supervisor
    - '693857339672887367' # Sheriff Department
  694654347962876035: # SO High Command
    - '694653003184996423' # Chief Deputy
    - '694653005194199041' # Colonel
    - '694653007698198630' # Major
    - '694653017378521098' # Captain
    - '694653009552211988' # Lieutenant
    - '694653011569541140' # Sergeant
    - '694653013259845723' # Corporal
    - '694653015176773693' # Master Deputy
    - '694653019253506078' # Senior Deputy
    - '694653022525194372' # Deputy
    - '694653021019439174' # Probationary Deputy
    - '694735836456943666' # SO Awaiting Training
    - '694654349309378620' # SO FTO
    - '694654352052322384' # SO Application Handler
    - '694654353763598336' # SO Supervisor
    - '693857339672887367' # Sheriff Department
  693857132902088736: # LAPD Chief of Police
    - '694650836550287471' # LAPD High Command
    - '694649763156459550' # LAPD Assistant Chief of Police
    - '694650813997383711' # LAPD Deputy Chief of Police
    - '694650815893340271' # LAPD Commander
    - '694650818472837149' # LAPD Captain
    - '694650820532371528' # LAPD Lieutenant
    - '694650822751027200' # LAPD Police Sergeant II
    - '694650824931934248' # LAPD Police Sergeant
    - '694650827435933727' # LAPD Corporal
    - '694650829822623784' # LAPD Police Officer
    - '694650832452321301' # LAPD Trainee
    - '694650834285363200' # LAPD Supervisor
    - '694650838852829268' # LAPD Training Officer
    - '694650841230999553' # LAPD Application Handler
    - '693857015663034429' # LAPD
  694650836550287471: # LAPD High Command
    - '694649763156459550' # LAPD Assistant Chief of Police
    - '694650813997383711' # LAPD Deputy Chief of Police
    - '694650815893340271' # LAPD Commander
    - '694650818472837149' # LAPD Captain
    - '694650820532371528' # LAPD Lieutenant
    - '694650822751027200' # LAPD Police Sergeant II
    - '694650824931934248' # LAPD Police Sergeant
    - '694650827435933727' # LAPD Corporal
    - '694650829822623784' # LAPD Police Officer
    - '694650832452321301' # LAPD Trainee
    - '694650834285363200' # LAPD Supervisor
    - '694650838852829268' # LAPD Training Officer
    - '694650841230999553' # LAPD Application Handler
    - '693857015663034429' # LAPD
  693899388858138685: # Head of Fire/EMS
    - '694655531133960304' # Deputy Head of Fire/EMS
    - '694655532740378644' # High Command Fire/EMS
    - '694655533298483201' # MedEvac Team Leader
    - '694655535018147941' # Fire Commissioner
    - '694655536527966258' # Deputy Fire Commissioner
    - '694655538188779601' # District Chief
    - '694655539111657523' # Assistant District Chief
    - '694655540802093097' # Captain
    - '694655541703606283' # Lieutenant
    - '694655543192715466' # Firefighter
    - '694655544555864179' # Probationary Firefighter
    - '694655545851904011' # Senior Paramedic
    - '694657765888491601' # Paramedic
    - '694657770879975545' # EMT
    - '694657775552430193' # Probationary EMT
    - '694658269062365187' # Fire/EMS FTO
    - '694658273407795257' # Sr.Paramedic
    - '694658277421613056' # Senior Firefighter
    - '694658280454226161' # MedEvac
    - '693899961800327309' # Fire/EMS Department
  694655532740378644: # High Command Fire/EMS
    - '694655531133960304' # Deputy Head of Fire/EMS
    - '694655533298483201' # MedEvac Team Leader
    - '694655535018147941' # Fire Commissioner
    - '694655536527966258' # Deputy Fire Commissioner
    - '694655538188779601' # District Chief
    - '694655539111657523' # Assistant District Chief
    - '694655540802093097' # Captain
    - '694655541703606283' # Lieutenant
    - '694655543192715466' # Firefighter
    - '694655544555864179' # Probationary Firefighter
    - '694655545851904011' # Senior Paramedic
    - '694657765888491601' # Paramedic
    - '694657770879975545' # EMT
    - '694657775552430193' # Probationary EMT
    - '694658269062365187' # Fire/EMS FTO
    - '694658273407795257' # Sr.Paramedic
    - '694658277421613056' # Senior Firefighter
    - '694658280454226161' # MedEvac
    - '693899961800327309' # Fire/EMS Department
  693857605159747646: # FAA Director
    - '693901064847622146' # FAA Deputy Director
    - '693900243238125620' # FAA FTO
    - '693900419432448040' # FAA Flight Instructor
    - '694291765452079166' # FAA Mil-Grade
    - '693900058659127357' # FAA Commercial
    - '693899544513216563' # FAA Aircraft
    - '693899765561294939' # FAA Rotorcraft
    - '693857675888295976' # FAA Certified
    - '693899292716302486' # FAA Recruit
    - '693900790779215912' # FAA
    - '693900832718061638' # ATC FTO
    - '693900658473959496' # ATC
  693900243238125620: # FAA FTO
    - '693900419432448040' # FAA Flight Instructor
    - '694291765452079166' # FAA Mil-Grade
    - '693900058659127357' # FAA Commercial
    - '693899544513216563' # FAA Aircraft
    - '693899765561294939' # FAA Rotorcraft
    - '693857675888295976' # FAA Certified
    - '693899292716302486' # FAA Recruit
    - '693900790779215912' # FAA
    - '693900832718061638' # ATC FTO
    - '693900658473959496' # ATC
    - '693901064847622146' # FAA Deputy Director
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
* All you need to do is click `start_SimpleRoleBot.bat` file to start up the bot

## Configuring Permissions via RoleIDs in config.yml

* You will now navigate to the `config.yml` file and open it
* We now need to understand how the configuration works

```text
#############################
###     SimpleRoleBot     ###
###      created by       ###
###        Badger         ###
#############################
BotToken: ''
RoleConfiguration:
  693833984173408328: # Staff Role
    - '*' # All Permission for every role below their highest role
  693901091678716006: # National Guard OIC
    - '694065977398132738' # National Guard HC
```

* The roles under `RoleConfiguration:` are known as the `RoleID` keys
* The `RoleID` keys `693901091678716006` and `693901091678716006` are the ID of roles that you will set up permissions for for adding and removing roles from other users
* All the `RoleID` values which can be displayed as `'*'` and `'694065977398132738'` are also IDs of roles within discord, however these are the IDs of roles that the `RoleID` key role will be able to add and remove from users
* **Note:** `693901091678716006` is the ID of the role `National Guard OIC` within my discord server
* **Note:** `693833984173408328` ****is the ID of the role `Staff` within my discord server
* If you would like to give a role permissions to add/remove roles to users \(so long as the role is below their highest role\), you will want to give them the `'*'` permission under their `RoleID` key

{% hint style="info" %}
**Any further questions and/or concerns?**

You may gather more support personally and from other members of the Badger Developer Community over [here](https://discord.gg/Rmzgwpn).
{% endhint %}

