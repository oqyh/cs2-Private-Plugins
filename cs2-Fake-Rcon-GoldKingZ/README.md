
## .:[ Price ]:. [(Free Private Rules)](https://github.com/oqyh/cs2-Private-Plugins/blob/11b92dc04067753a390d796dbba39d789f270aab/README.md?plain=1#L27)
```diff
+ PRICE FREE [Only Discord Members] 
```

# [CS2] Fake-Rcon-GoldKingZ (1.0.4)  

### Dynamic Fake Rcon Depend FakeRcon_Settings.json
### Setup Each Group's Limits With Logs
### `-fakercon <password>` StartUp If Not Found Plugin Will Use FakeRcon_Settings.json

![fake_rcon](https://github.com/user-attachments/assets/a89303b9-c9f1-4d1f-ba6b-05f58d971437)

![fake_rcon_text](https://github.com/user-attachments/assets/98ecbf87-fe0f-4584-8033-0d5472fa9125)

![fake_rcon_discord](https://github.com/user-attachments/assets/572f91e6-242a-4601-9113-ec4bf0c63f11)

## .:[ Dependencies ]:.
[Metamod:Source (2.x)](https://www.sourcemm.net/downloads.php/?branch=master)

[CounterStrikeSharp](https://github.com/roflmuffin/CounterStrikeSharp/releases)

[Newtonsoft.Json](https://www.nuget.org/packages/Newtonsoft.Json)


## .:[ Configuration ]:.

> [!CAUTION]
> Config Located In ..\addons\counterstrikesharp\plugins\Fake-Rcon-GoldKingZ\config\config.json                                         

```json

{
//----------------------------[ ↓ Fake Rcon Config ↓ ]----------------------------

  //Commands In Game For Fake Rcon
  "FakeRcon_CommandsInGame": "fake_rcon,f_r,fakercon,fr",

  //Commands In Game For Fake Rcon Password
  "FakeRconPassword_CommandsInGame": "fake_rcon_password,f_r_p,fakerconpassword,fakerconpass,frp",

  //(Time In Min) Caching After Enter Correct Password So You Dont Need To Write Password Again
  "FakeRcon_Caching_TimeInXMins_PerPlayer": 120,

  //Give How Many X Tries  If Enter Wrong Password
  "FakeRcon_WrongPasswords_Xtry": 3,

  //(Time In Min) If FakeRcon_WrongPasswords_Xtry Pass Give CoolDown
  "FakeRcon_GiveCoolDown_InXMins": 10,

//----------------------------[ ↓ Text Log Config ↓ ]----------------------------

  //Enable Logging Fake Rcons Located In Fake-Rcon-GoldKingZ/logs/ ?
  "TextLog_Enable": false,
  //Log Message Format
  //{TIME} == Time
  //{DATE} == Date
  //{CMD} == Command Send
  //{GROUP} == Group Name
  //{PLAYERNAME} == Player Name Who Type In Chat
  //{STEAMID} = STEAM_0:1:122910632
  //{STEAMID3} = U:1:245821265
  //{STEAMID32} = 245821265
  //{STEAMID64} = 76561198206086993
  //{IP} = 127.0.0.0
  "TextLog_MessageFormat": "[{DATE} - {TIME}] Sending... [ {CMD} ] FROM [ Group: {GROUP} ] {PLAYERNAME} {STEAMID}",
  
  //Date and Time Formate
  "TextLog_DateFormat": "MM-dd-yyyy",
  "TextLog_TimeFormat": "HH:mm:ss",

  //Auto Delete Logs If More Than X (Days) Old
  "TextLog_AutoDeleteLogsMoreThanXdaysOld": 0,

//----------------------------[ ↓ Discord Log Config ↓ ]----------------------------

  //Send Log To Discord Via WebHookURL
  // (0) = Disable
  // (1) = Text Only (Result Image : https://github.com/oqyh/cs2-Private-Plugins/blob/main/cs2-Fake-Rcon-GoldKingZ/Resources/mode1.png?raw=true)
  // (2) = Text With + Name + Hyperlink To Steam Profile (Result Image : https://github.com/oqyh/cs2-Private-Plugins/blob/main/cs2-Fake-Rcon-GoldKingZ/Resources/mode2.png?raw=true)
  // (3) = Text With + Name + Hyperlink To Steam Profile + Profile Picture (Result Image : https://github.com/oqyh/cs2-Private-Plugins/blob/main/cs2-Fake-Rcon-GoldKingZ/Resources/mode3.png?raw=true)
  // (4) = Text With + Name + Hyperlink To Steam Profile + Profile Picture + Saparate Date And Time From Message (Result Image : https://github.com/oqyh/cs2-Private-Plugins/blob/main/cs2-Fake-Rcon-GoldKingZ/Resources/mode4.png?raw=true)
  // (5) = Text With + Name + Hyperlink To Steam Profile + Profile Picture + Saparate Date And Time From Message + Server Ip In Footer (Result Image : https://github.com/oqyh/cs2-Private-Plugins/blob/main/cs2-Fake-Rcon-GoldKingZ/Resources/mode5.png?raw=true)
  "DiscordLog_EnableMode": 0,

  //Log Message Format
  //{TIME} == Time
  //{DATE} == Date
  //{CMD} == Command Send
  //{GROUP} == Group Name
  //{PLAYERNAME} == Player Name Who Type In Chat
  //{STEAMID} = STEAM_0:1:122910632
  //{STEAMID3} = U:1:245821265
  //{STEAMID32} = 245821265
  //{STEAMID64} = 76561198206086993
  //{IP} = 127.0.0.0
  "DiscordLog_MessageFormat": "[{DATE} - {TIME}] Sending... [ {CMD} ] FROM [ Group: {GROUP} ] {PLAYERNAME} {STEAMID}",
  
  //Date and Time Formate
  "DiscordLog_DateFormat": "MM-dd-yyyy",
  "DiscordLog_TimeFormat": "HH:mm:ss",
  
  //If DiscordLog_EnableMode (2) or (3) or  (4) or (5) How Would You Side Color Message To Be Check (https://www.color-hex.com/) For Colors
  "DiscordLog_SideColor": "00FFFF",
  
  //Discord WebHookURL
  "DiscordLog_WebHookURL": "https://discord.com/api/webhooks/XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX",
  
  //If DiscordLog_EnableMode (3) or  (4) or (5) And Player Doesn't Have Profile Picture Which Picture Do You Like To Be Replaced
  "Discord_UsersWithNoAvatarImage": "https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/refs/heads/main/Resources/noavatar.jpg",
  
  //If DiscordLog_EnableMode (5) Image Url Footer
  "Discord_FooterImage": "https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/refs/heads/main/Resources/serverip.png",

//----------------------------[ ↓ Debug ↓ ]----------------------------

  //Enable Debug Will Print Server Console If You Face Any Issue
  "EnableDebug": false,
}

```


## .:[ Configuration FakeRcon ]:.

> [!CAUTION]
> FakeRcon Config Located In ..\addons\counterstrikesharp\plugins\Fake-Rcon-GoldKingZ\config\FakeRcon_Settings.json                                         
```json

//==========================
//        Options
//==========================
// "Flags": "@css/root,@css/vip" //Only These Can Access Group
// "Password": "RootPassWORD123123" //Password To Enter The Group (Note: If Using Pass Priority From Top To Bottom)
// "Allow_Any_Except_These": "sv_cheats,mp_respawn_on_death_t,mp_respawn_on_death_ct" //Allow Any Convar Except These In The String 
// "Allow_These_Only": "sv_alltalk,sv_allow_votes" //Allow Only These In The String
//==========================

{
	"Root_Admin_Rcon":
	{
		"Flags": "@css/admin,#css/root",
		"Password": "RootPassWORD123123"
	},
	"Mods_Rcon":
	{
		"Flags": "@css/mods,#css/mods",
		"Allow_Any_Except_These": "sv_cheats,mp_respawn_on_death_t,mp_respawn_on_death_ct",
		"Password": "ModsPassword123123"
	},
	"Vip_Rcon":
	{
		"Allow_These_Only": "sv_alltalk,sv_allow_votes",
		"Password": "vip123123"
	}
}

```

## .:[ Language ]:.
```json
{
	//==========================
	//        Other
	//==========================
	//{nextline} = Print On Next Line
	//==========================

	"PrintConsoleToPlayer.Notallowed": "You Are Not Allowed To Use Fake Rcon",
	"PrintConsoleToPlayer.Notallowed.This.Command": "This Command [{0}] is not allowed for you",
	"PrintConsoleToPlayer.Banned": "You Reached Password Tries Limit You On CoolDown For {0}",
	"PrintConsoleToPlayer.Password.Wrong": "Password Is Wrong You Have {0} Tries Left",
	"PrintConsoleToPlayer.Access.Group": "You Have Accese To [{0}]",
	"PrintConsoleToPlayer.Send.Fakercon": "Sending: {0}"
}
```

## .:[ Change Log ]:.
```
(1.0.4)
-Fix GKZ Api

(1.0.3)
-Fix Bugs
-Fix GKZ Api
-Remove Port Restricted
-Remove Key No Needed
-Remove ChangeCheckIpAdressToWebSite

(1.0.2)
-Fix Server Will Crash on Capital letter Send Commands (fake_rcon MAP DE_DUST2)

(1.0.1)
-Reword Plugin
-Fix Some Bugs
-Fix Flags In FakeRcon_Settings.json
-Fix TextLog_AutoDeleteLogsMoreThanXdaysOld
-Added Command Line (-fakercon <password>)
-Added {GROUP} In MessageFormat
-Added ChangeCheckIpAdressToWebSite
-Added FakeRcon_CommandsInGame
-Added FakeRconPassword_CommandsInGame
-Added FakeRcon_Caching_TimeInXMins_PerPlayer
-Added FakeRcon_WrongPasswords_Xtry
-Added FakeRcon_GiveCoolDown_InXMins
-Added EnableDebug
-Added Password In FakeRcon_Settings.json  
-Added gkz_json Check FakeRcon_Settings.json Is Correct Or Not
-Added "PrintConsoleToPlayer.Banned" In Lang
-Added "PrintConsoleToPlayer.Password.Wrong" In Lang
-Added "PrintConsoleToPlayer.Access.Group" In Lang

(1.0.0)
-Initial Release
```
