
## .:[ Price ]:. [(Free Private Rules)](https://github.com/oqyh/cs2-Private-Plugins/blob/11b92dc04067753a390d796dbba39d789f270aab/README.md?plain=1#L27)
```diff
+ PRICE FREE [Only Discord Members] 
```

# [CS2] Fake-Rcon-GoldKingZ (1.0.0)  

### Dynamic Fake Rcon Depend FakeRcon_Settings.json
### Setup Each Group's Limits With Logs

![notallowed](https://github.com/oqyh/cs2-Private-Plugins/assets/48490385/cccd5c4e-82f4-4353-a1ac-102a631269b3)

![ingame](https://github.com/oqyh/cs2-Private-Plugins/assets/48490385/04a6e5b0-c1a9-41fb-a8a6-d9c4ae1da2f2)

![text](https://github.com/oqyh/cs2-Private-Plugins/assets/48490385/fae1db69-1296-4c8e-8680-2bd00026e09d)

![mode5](https://github.com/oqyh/cs2-Private-Plugins/assets/48490385/ef06b10e-628a-41fb-a60e-7eba60b0ba37)


## .:[ Dependencies ]:.
[Metamod:Source (2.x)](https://www.sourcemm.net/downloads.php/?branch=master)

[CounterStrikeSharp](https://github.com/roflmuffin/CounterStrikeSharp/releases)

[Newtonsoft.Json](https://www.nuget.org/packages/Newtonsoft.Json)

[MySqlConnector](https://www.nuget.org/packages/MySqlConnector)

## .:[ Configuration ]:.

> [!CAUTION]
> Config Located In ..\addons\counterstrikesharp\plugins\Fake-Rcon-GoldKingZ\config\config.json                                         

```json

{
  //Key To Active Plugin
  KEY = "";

//-----------------------------------------------------------------------------------------

  //Enable Logging Fake Rcons Located In Fake-Rcon-GoldKingZ/logs/ ?
  TextLog_Enable = false;

  //Log Message Format
  //{TIME} == Time
  //{DATE} == Date
  //{CMD} == Command Send
  //{PLAYERNAME} == Player Name Who Type In Chat
  //{STEAMID} = STEAM_0:1:122910632
  //{STEAMID3} = U:1:245821265
  //{STEAMID32} = 245821265
  //{STEAMID64} = 76561198206086993
  //{IP} = 127.0.0.0
  TextLog_MessageFormat = "[{DATE} - {TIME}] Sending... [ {CMD} ] FROM {PLAYERNAME} {STEAMID}";

  //Date and Time Formate
  TextLog_DateFormat = "MM-dd-yyyy";
  TextLog_TimeFormat = "HH:mm:ss";

  //Auto Delete Logs If More Than X (Days) Old
  TextLog_AutoDeleteLogsMoreThanXdaysOld = 0;
  
//-----------------------------------------------------------------------------------------
  //Send Log To Discord Via WebHookURL
  // (0) = Disable
  // (1) = Text Only (Result Image : https://github.com/oqyh/cs2-Private-Plugins/blob/main/cs2-Fake-Rcon-GoldKingZ/Resources/mode1.png?raw=true)
  // (2) = Text With + Name + Hyperlink To Steam Profile (Result Image : https://github.com/oqyh/cs2-Private-Plugins/blob/main/cs2-Fake-Rcon-GoldKingZ/Resources/mode2.png?raw=true)
  // (3) = Text With + Name + Hyperlink To Steam Profile + Profile Picture (Result Image : https://github.com/oqyh/cs2-Private-Plugins/blob/main/cs2-Fake-Rcon-GoldKingZ/Resources/mode3.png?raw=true)
  // (4) = Text With + Name + Hyperlink To Steam Profile + Profile Picture + Saparate Date And Time From Message (Result Image : https://github.com/oqyh/cs2-Private-Plugins/blob/main/cs2-Fake-Rcon-GoldKingZ/Resources/mode4.png?raw=true)
  // (5) = Text With + Name + Hyperlink To Steam Profile + Profile Picture + Saparate Date And Time From Message + Server Ip In Footer (Result Image : https://github.com/oqyh/cs2-Private-Plugins/blob/main/cs2-Fake-Rcon-GoldKingZ/Resources/mode5.png?raw=true)
  DiscordLog_EnableMode = 0;

  //Log Message Format
  //{TIME} == Time
  //{DATE} == Date
  //{CMD} == Command Send
  //{PLAYERNAME} == Player Name Who Type In Chat
  //{STEAMID} = STEAM_0:1:122910632
  //{STEAMID3} = U:1:245821265
  //{STEAMID32} = 245821265
  //{STEAMID64} = 76561198206086993
  //{IP} = 127.0.0.0
  DiscordLog_MessageFormat = "[{DATE} - {TIME}] Sending... [ {CMD} ] FROM {PLAYERNAME} {STEAMID}";

  //Date and Time Formate
  DiscordLog_DateFormat = "MM-dd-yyyy";
  DiscordLog_TimeFormat = "HH:mm:ss";

  //If DiscordLog_EnableMode (2) or (3) or  (4) or (5) How Would You Side Color Message To Be Check (https://www.color-hex.com/) For Colors
  DiscordLog_SideColor = "00FFFF";

  //Discord WebHookURL
  DiscordLog_WebHookURL = "https://discord.com/api/webhooks/XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX";

  //If DiscordLog_EnableMode (3) or  (4) or (5) And Player Doesn't Have Profile Picture Which Picture Do You Like To Be Replaced
  Discord_UsersWithNoAvatarImage = "https://github.com/oqyh/cs2-Private-Plugins/blob/main/cs2-Fake-Rcon-GoldKingZ/Resources/noavatar.jpg?raw=true";

  //If DiscordLog_EnableMode (5) Image Url Footer
  Discord_FooterImage = "https://github.com/oqyh/cs2-Private-Plugins/blob/main/cs2-Fake-Rcon-GoldKingZ/Resources/serverip.png?raw=true";

}

```


## .:[ Configuration FakeRcon ]:.

> [!CAUTION]
> ReservedSlots Config Located In ..\addons\counterstrikesharp\plugins\Fake-Rcon-GoldKingZ\config\FakeRcon_Settings.json.json                                         
```json

{
  "Group_1": {
    "ALLOW_THESE_ONLY": "sv_alltalk,sv_allow_votes", // This Group Only Have These sv_alltalk,sv_allow_votes
    "FLAGS": "@css/vip,#css/vip"
  },
  "Group_2": {
    "ALLOW_ANY_EXCEPT_THESE": "sv_cheats,mp_respawn_on_death_t,mp_respawn_on_death_ct", // This Group Have ANY Execpt These sv_cheats,mp_respawn_on_death_t,mp_respawn_on_death_ct
    "FLAGS": "@css/mods,#css/mods"
  },
  "Group_3": { // ANY Convars
    "FLAGS": "@css/admin,#css/root"
  }
}

```

## .:[ Language ]:.
```json
{
	//==========================
	//        Colors
	//==========================
	//none
	//==========================
	//        Other
	//==========================
	//{0} = Convar
	//==========================
	"console.player.notallowed": "You are not allowed",
	"console.player.notallowed.command": "This Command [{0}] is not allowed for you",
	"console.send.fakeron": "Sending: {0}"
}
```

## .:[ Change Log ]:.
```
(1.0.0)
-Initial Release
```
