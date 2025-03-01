
## .:[ Price ]:. [(Payment Rules)](https://github.com/oqyh/cs2-Private-Plugins/blob/8040379022008134dde7d34cf08f7a611c750862/README.md?plain=1#L7)
```diff
+ PRICE 10$ + FREE Multiple Servers [Lifetime ( One Time Payment )] 
```

# [CS2] Say-Sound-GoldKingZ (1.0.5)  

### Let Players Convert Chat/Radio To Say Sound With Radius

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/GWZRZuL20QA/0.jpg)](https://www.youtube.com/watch?v=GWZRZuL20QA)

![mode1](https://github.com/user-attachments/assets/9a1a1524-a752-4808-8f61-ccfeab800afd)
![mode2](https://github.com/user-attachments/assets/2b63a3ef-0d50-489c-b7f1-0c21603a2b79)
![mode3](https://github.com/user-attachments/assets/0a5f692e-3854-4c3d-a08c-3762046e9b2a)




## .:[ Dependencies ]:.

[Metamod:Source (2.x)](https://www.sourcemm.net/downloads.php/?branch=master)

[MultiAddonManager](https://github.com/Source2ZE/MultiAddonManager)

[CounterStrikeSharp](https://github.com/roflmuffin/CounterStrikeSharp/releases)

[Newtonsoft.Json](https://www.nuget.org/packages/Newtonsoft.Json)

[MySqlConnector](https://www.nuget.org/packages/MySqlConnector)


## .:[ Configuration ]:.

> [!CAUTION]
> Config Located In ..\addons\counterstrikesharp\plugins\Say-Sound-GoldKingZ\config\config.json                                         

```json

{

//----------------------------[ ↓ Main Configs ↓ ]----------------------------

  //Override Plugins Controls Chat Hook
  "Override_These_Plugins": "CS2-Tags,Plugin2,Plugin3",

  //Open Menu Mode:
  // 0 = Disable Menu
  // 1 = Custom Chat Menu By GoldKingZ
  // 2 = Custom Chat Menu By GoldKingZ
  // 3 = WASD Menu By GoldKingZ
  "OpenMenu_Mode": 3,

  //Allow These Groups Only To OpenMenu_Mode (Make It Empty "" To Let AnyOne)  [Example:@css/root,@css/admin,@css/vip,#css/admin,#css/vip]
  "OpenMenu_Flags": "",

  //Commands In Game To Open Menu
  "OpenMenu_CommandsInGame": "!ssmenu,!saysoundmenu,!saysoundsmenu",

  //Allow These Groups Only To Reload Json
  "Reload_Json_Flags": "@css/root,@css/admin,#css/root,#css/admin",

  //Commands In Game To Reload Json
  "Reload_Json_CommandsInGame": "!reloadsaysound,!reloadss",


//----------------------------[ ↓ Say Sound Config ↓ ]----------------------------


  //Default Value Toggle Sound
  //true = Enabled
  //false = Disabled
  "Default_Toggle_Sound": true,

  //Default Value Toggle Message
  //true = Enabled
  //false = Disabled
  "Default_Toggle_Message": true,

  //Disable Say Sound On WarmUp?
  "DisableOnWarmUp": false,

  //Pick Random Say Sound Paths?
  //true = Yes
  //false = No, Pick From Top To Bottom
  "Pick_Random_SaySound": true,

  //Allow Dead Players To Toggle Say Sound?
  "AllowDeadPlayersToSaySound": false,

  //Hide Default Radio Message If Toggle Say Sound By Radio?
  "HideDefaultRadioMessageAfterSaySound": true,

  //Hide Default Chat Message If Toggle Say Sound By Chat?
  "HideDefaultChatMessageAfterToggleShortCutSaySound": true,

  //Skip Cooldown For These Flags  (Make It Empty "" To Let AnyOne)
  "ImmunityFromCooldownFlags": "@css/root,@css/admin,#css/root,#css/admin",

//----------------------[ ↓ Save Players Data By Cookies Locally ↓ ]----------------------

  //Enable Cookies?
  //true = Yes, (Will Be Located In ../Say-Sound-GoldKingZ/Cookies/Cookies.json)
  //false = No, Disable
  "Enable_Cookies": true,

  //Auto Delete Inactive Players Older Than X Days In Cookies
  "Cookies_AutoRemovePlayerCookieOlderThanXDays": 7,

//---------------------------[ ↓ Save Players Data By MySql ↓ ]----------------------------

  //Enable MySql?
  "Enable_MySql": false,

  //MySql
  "MySql_Host": "MySql_Host",
  "MySql_Database": "MySql_Database",
  "MySql_Username": "MySql_Username",
  "MySql_Password": "MySql_Password",
  "MySql_Port": 3306,

  //Auto Delete Inactive Players Older Than X Days In MySql
  "MySql_AutoRemovePlayersOlderThanXDays": 7,

//----------------------------[ ↓ Utilities ↓ ]----------------------------------------------

  //Auto Update Signatures
  "AutoUpdateSignatures": true,

  //Enable Debug Will Print Server Console If You Face Any Issue
  "EnableDebug": false,
}

```


## .:[ Configuration Say Sound ]:.

> [!CAUTION]
> SaySound Config Located In ..\addons\counterstrikesharp\plugins\Say-Sound-GoldKingZ\config\SaySound_Settings.json               
                          
```json
{
	//==========================
	//        Options
	//==========================
	// "Hide_It_And_Show_Only_ForFlags": "@css/root,@css/vip" //Hide Menu/SubMenu And Only These Flags Can See It
	// "Only_These_Flags_Can_Access_It": "@css/root,@css/vip" //Only These Can Access Menu/SubMenuz
	// "SubMenu.STATUS.TOGGLE_SOUND.xxxxxxxxxxx:":{} //Show Client His Current Toggle SaySound Sound Enabled Or Disabled
	// "SubMenu.STATUS.TOGGLE_MESSAGE.xxxxxxxxxxx:":{} //Show Client His Current Toggle SaySound Message Enabled Or Disabled
	// "Hook_Radio": "cheer", //Hook This Sound Into Player Radio [Example: coverme,takepoint,holdpos,regroup,followme,takingfire,go,fallback,sticktog,getinpos,stormfront,report,roger,enemyspot,needbackup,sectorclear,inposition,reportingin,getout,negative,enemydown,sorry,cheer,compliment,thanks,go_a,go_b,needrop,deathcry]
	// "Toggle_Sound_In_Chat": "hi,hello", //Toggle In Chat ShortCut By hi Or hello You Can Add As Many As You Like
	// "PrintChatToAll": true, // Show Message To All || True = Yes || false OR Not Used = No
	// "PrintChatToPlayer": true, // Show Message To Player Who SaySound || True = Yes || false OR Not Used = No
	// "OnlyForTeam": 1, // Only Team Can Access This || 1 = CT || 2 = T || 0 OR Not Used = Any Team
	// "Give_Cooldown_After_This_InXSecs": 5, //Give Cooldown After This 5 Secs
	// "Sound_Paths": "hi" // Using sounds/saysound/hi.vsnd Will Be Not 3d Radius || Using hi Only Will Be 3d Radius
	//==========================

	"Menu.Say Sound Settings":
	{
		"SubMenu.STATUS.TOGGLE_SOUND. Sound:": //Display Current Toggle SaySound Sound
		{
			"Only_These_Flags_Can_Access_It": "@css/root,@css/vip" //Only These Can Toggle On Off
		},
		
		"SubMenu.STATUS.TOGGLE_MESSAGE. Message:":{} //Display Current Toggle SaySound Message + Any Can Toggle On Off
	},
	"Menu.(Free) SaySounds":// ((Free) SaySounds) Is Then Display Menu Name
	{
		"SubMenu.Hi":
		{
			"Hook_Radio": "cheer",
			"Toggle_Sound_In_Chat": "hi,hello",
			"PrintChatToAll": true,
			"Give_Cooldown_After_This_InXSecs": 5,
			"Sound_Paths":
			[
				"hi"
			]
		}
		//..Add Many As You Like For More Submenus
	}
	//..Add Many As You Like For More Menus
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

	"PrintChatToPlayer.ReloadJson.Not.Allowed": "{green}[Say Sound] {darkred}You Dont Have Permission",
	"PrintChatToPlayer.Menu.Disabled": "{green}[Say Sound] {darkred}Say Sound Menu Is {darkred}Disabled By The Server",
	"PrintChatToPlayer.Menu.Not.Allowed": "{green}[Say Sound] {darkred}You Dont Have Permission",

	"PrintChatToPlayer.SaySound.Not.Allowed": "{green}[Say Sound] {darkred}You Dont Have Permission",
	"PrintChatToPlayer.SaySound.Disabled.On.WarmUp": "{green}[Say Sound] {grey}Say Sound Disabled On Warmup",
	"PrintChatToPlayer.SaySound.CT.Team.Only": "{green}[Say Sound] {grey}This Say Sound Only For CT Side",
	"PrintChatToPlayer.SaySound.T.Team.Only": "{green}[Say Sound] {grey}This Say Sound Only For T Side",
	"PrintChatToPlayer.SaySound.While.He.Is.Dead": "{green}[Say Sound] {grey}You Cant Say Sound When You Are Dead",
	"PrintChatToPlayer.SaySound.While.He.Is.OnCooldown": "{green}[Say Sound] {grey}You Are On Cooldown. Please Wait {yellow}{0} Seconds.",


	"PrintChatToPlayer.Toggle_Sound.SaySound.Not.Allowed": "{green}[Say Sound] {darkred}You Dont Have Permission",
	"PrintChatToPlayer.Toggle_Sound.SaySound.Enabled": "{green}[Say Sound] {grey}Sound Now {lime}Enabled",
	"PrintChatToPlayer.Toggle_Sound.SaySound.Disabled": "{green}[Say Sound] {grey}Sound Now {darkred}Disabled",

	"PrintChatToPlayer.Toggle_Message.SaySound.Not.Allowed": "{green}[Say Sound] {darkred}You Dont Have Permission",
	"PrintChatToPlayer.Toggle_Message.SaySound.Enabled": "{green}[Say Sound] {grey}Messages Now {lime}Enabled",
	"PrintChatToPlayer.Toggle_Message.SaySound.Disabled": "{green}[Say Sound] {grey}Messages Now {darkred}Disabled",



	"PrintChatToPlayer.SaySound": "{green}[Say Sound] {purple}{0} {grey}Saying.... {yellow}{1}",
	"PrintToChatToAll.SaySound": "{green}[Say Sound] {purple}{0} {grey}Saying.... {yellow}{1}",
	"PrintToChatToAll.SaySound.Hi": "{green}[Say Sound] {purple}{0} {grey}: Hi :))))",
	"PrintToChatToAll.SaySound.Wake Up (Not 3d Sound)": "{green}[Say Sound] {darkred}[ADMIN] {purple}{0} Everyone Wake Up!",




	"Mode_1.MainMenu.Title": "{Magenta} Say Sound Menu",
	"Mode_1.SubMenu.Title": "{Purple} .:[ {0} ]:.",
	"Mode_1.STATUS.TOGGLE_SOUND.Enabled": "{Lime} ✔",
	"Mode_1.STATUS.TOGGLE_SOUND.Disabled": "{Darkred} ✖",
	"Mode_1.STATUS.TOGGLE_MESSAGE.Enabled": "{Lime} ✔",
	"Mode_1.STATUS.TOGGLE_MESSAGE.Disabled": "{Darkred} ✖",

	"Mode_2.MainMenu.Title": "<font class='fontSize-M' color='#b74eae'> Say Sound Menu</font>",
	"Mode_2.SubMenu.Title": "<font class='fontSize-M' color='#f809e6'> .:[ {0} ]:. </font>",
	"Mode_2.STATUS.TOGGLE_SOUND.Enabled": "<font color='#0cff00'> ✔",
	"Mode_2.STATUS.TOGGLE_SOUND.Disabled": "<font color='#ff2d00'> ✖",
	"Mode_2.STATUS.TOGGLE_MESSAGE.Enabled": "<font color='#0cff01'> ✔",
	"Mode_2.STATUS.TOGGLE_MESSAGE.Disabled": "<font color='#ff2d01'> ✖",


	"Mode_3.MainMenu.Title": "<font class='fontSize-M' color='#b74eae'> Say Sound Menu</font>",
	"Mode_3.SubMenu.Title": "<font class='fontSize-M' color='#f809e6'> .:[ {0} ]:. </font>",
	"Mode_3.STATUS.TOGGLE_SOUND.Enabled": "<font color='#0cff00'> ✔",
	"Mode_3.STATUS.TOGGLE_SOUND.Disabled": "<font color='#ff2d00'> ✖",
	"Mode_3.STATUS.TOGGLE_MESSAGE.Enabled": "<font color='#0cff01'> ✔",
	"Mode_3.STATUS.TOGGLE_MESSAGE.Disabled": "<font color='#ff2d01'> ✖"
}
```

## .:[ Change Log ]:.
```
(1.0.5)
-Fix Some Bugs
-Fix Mysql
-Rework On Plugin
-Rework On Sound_Paths
-Added OnlyForTeam
-Added PrintChatToAll
-Added PrintChatToPlayer
-Added Reload_Json_Flags
-Added Reload_Json_CommandsInGame
-Added Default_Toggle_Sound
-Added Default_Toggle_Message
-Added DisableOnWarmUp
-Added Pick_Random_SaySound
-Added AutoUpdateSignatures
-Added GKZ MenuApi
-Added TOGGLE_SOUND
-Added TOGGLE_MESSAGE
-Removed Print_To_Chat


(1.0.4)
-Fix Some Bugs
-Added Hide_It_And_ShowThisOnlyForFlags In SaySound_Settings
-Added ImmunityFromCooldownFlags In Configs

(1.0.3)
-Added ChangeCheckIpAdressToWebSite
-Added OpenMenu_Mode 3 Custom Menu Chat Center WASD Works With Menu And SubMenus
-Added OpenMenu_Flags 
-Added OpenMenu_CommandsInGame 
-Added OpenMenu_CloseMenuAfterSelectItem 
-Added Toggle_DisableSaySoundsFlags 
-Added Toggle_DisableSaySoundsCommandsInGame
-Added Toggle_AutoRemovePlayerCookieOlderThanXDays
-Added MenuWASD_FreezePlayerOnMenuOpen
-Added MenuWASD_ExitMenuOnPressing 
-Added Enable_UseMySql 
-Added MySqlHost 
-Added MySqlDatabase
-Added MySqlUsername 
-Added MySqlPassword
-Added MySqlPort

(1.0.2)
-Added AllowDeadPlayersToSaySound

(1.0.1)
-Fix Some Bugs
-Added gkz_plugins To check status of gkz plugins
-Added MAKE_SOUND_3D
-Added Override_These_Plugins

(1.0.0)
-Initial Release
```
