
## .:[ Price ]:. [(Payment Rules)](https://github.com/oqyh/cs2-Private-Plugins/blob/8040379022008134dde7d34cf08f7a611c750862/README.md?plain=1#L7)
```diff
+ PRICE 5$ + FREE Multiple Servers [Lifetime ( One Time Payment )] 
```

# [CS2] Advanced-ReservedSlots-GoldKingZ (1.0.1)  

### Dynamic Kick Reserved Slots Depend Group Priority 
### when server is full - 1  it random kick start with normal people when group_1 or 2 or 3 joined then if no normal people in game it random kick Group_1 and so on...

![image](https://github.com/oqyh/cs2-Private-Plugins/assets/48490385/c7eea100-f571-40e9-880c-ef2414e055d6)

![serverfull](https://github.com/oqyh/cs2-Private-Plugins/assets/48490385/789259bd-a31c-40b5-a140-5ddf26c04bbf)


## .:[ Dependencies ]:.

[Metamod:Source (2.x)](https://www.sourcemm.net/downloads.php/?branch=master)

[CounterStrikeSharp](https://github.com/roflmuffin/CounterStrikeSharp/releases)

[Newtonsoft.Json](https://www.nuget.org/packages/Newtonsoft.Json)


## .:[ Configuration ]:.

> [!CAUTION]
> Config Located In ..\addons\counterstrikesharp\plugins\Advanced-ReservedSlots-GoldKingZ\config\config.json                                         

```json

{
//----------------------------[ ↓ Main Config ↓ ]----------------------------
  
  //Allow These Groups Only To Reload Json
  "Reload_Json_Flags": "@css/root,@css/admin,#css/root,#css/admin",

  //Commands In Game To Reload Json
  "Reload_Json_CommandsInGame": "!reloadreserved,!reloadreservedslot,!reloadreserv",

//----------------------------[ ↓ ReservedSlots Config ↓ ]----------------------------

  //Kick Mode?
  //(0) = Kick Random Players
  //(1) = Kick Highest Ping
  //(2) = Kick Highest Score
  //(3) = Kick Lowest Score
  //(4) = Kick Player Who In The Server Longest Time
  //(5) = Kick Player Who In The Server Shortest Time
  "KickMode": 0,

  //Do KickMode On Players In Spectators First?
  //(true) = Yes
  //(false) = No (Any)
  "PriorityKickOnSpecPlayers": true,

  //Kick With Proper Reason?
  "KickWithReason": false,

  //Do Delay Kick?
  "Delaykick": true,

  //If Delaykick true Do Delay Kick Time (InSecs)
  "DelayTimeXInSecs": 10,

//----------------------------[ ↓ Utilities ↓ ]----------------------------

  //Enable Debug Will Print Server Console If You Face Any Issue
  "EnableDebug": false
}

```


## .:[ Configuration ReservedSlots ]:.

> [!CAUTION]
> ReservedSlots Config Located In ..\addons\counterstrikesharp\plugins\Advanced-ReservedSlots-GoldKingZ\config\ReservedSlots_Settings.json                                         
```json

{
  "VIPS": { //Group Name 
    "Flags": "@css/vip,#css/vip" //Flags
  },
  "VVIPS": { //Group Name 
    "Flags": "@css/vvip,#css/vvip" //Flags
  },
  "ADMINS": { //Group Name 
    "Flags": "@css/admin,#css/admin" //Flags
  }
}

```

## .:[ Language ]:.
```json
{
	//==========================
	//        Colors
	//==========================
	//{Yellow} {Gold} {Silver} {Blue} {DarkBlue} {BlueGrey} {Magenta} {LightRed}
	//{LightBlue} {Olive} {Lime} {Red} {Purple} {Grey}
	//{Default} {White} {Darkred} {Green} {LightYellow}
	//==========================
	//        Other
	//==========================
	//{nextline} = Print On Next Line
	//==========================

	"PrintChatToPlayer.ReloadJson.Not.Allowed": "{green}Gold KingZ {grey}| {darkred}You Dont Have Permission To Access This",

	"PrintChatToPlayer.Kicked.Full.Delay": "{red}------------------------------------------ {nextline} {green}[AdvancedReservedSlots] {red}Server is full {grey}This Slot Reserved For {lime}Vips Only {nextline} {red}------------------------------------------",
    "PrintChatToPlayer.Kicked.Full.Replaced": "{red}------------------------------------------ {nextline} {green}[AdvancedReservedSlots] {grey}You Will Be Kicked {nextline} {green}[AdvancedReservedSlots] {grey}Reason: {lime}[ {purple}{0} {grey}/ {gold}{1} {lime}] {grey}Took Your Spot {nextline} {red}------------------------------------------",
    "PrintChatToAll.Kick": "{green}[AdvancedReservedSlots] {lime}[ {purple}{0} {grey}/ {gold}{1} {lime}] {grey}Joinned {nextline} {green}[AdvancedReservedSlots] {grey}Player: {red}{2} {grey}Will Get Kicked"
}
```

## .:[ Change Log ]:.
```
(1.0.1)
-Fix Bugs
-Fix GKZ Api
-Remove Port Restricted
-Remove Key No Needed
-Added KickMode (Kick Random Players,Kick Highest Ping,Kick Highest Score,Kick Lowest Score,Kick Player Who In The Server Longest Time,Kick Player Who In The Server Shortest Time)
-Added PriorityKickOnSpecPlayers 
-Added KickWithReason 
-Added Reload_Json_Flags 
-Added Reload_Json_CommandsInGame 

(1.0.0)
-Initial Release
```
