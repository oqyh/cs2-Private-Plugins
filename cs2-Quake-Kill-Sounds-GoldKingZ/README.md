
## .:[ Price ]:. [(Free Private Rules)](https://github.com/oqyh/cs2-Private-Plugins/blob/11b92dc04067753a390d796dbba39d789f270aab/README.md?plain=1#L27)
```diff
+ PRICE FREE [Only Discord Members (Limited Time Only)] 
```

# [CS2] Quake-Kill-Sounds-GoldKingZ (1.0.0)  

## Video ShowCase Of Plugin

[![Quake-Kill-Sounds-GoldKingZ](https://img.youtube.com/vi/Gm0OE0n7JD4/0.jpg)](https://youtu.be/iGlvhu2U1vI)


* Custom Quake Trackable (KillStreak, ComboKill, HeadShotKill, KnifeKill, GrenadeKill, MollyKill, TaserKill, NoScopeKill, OnAirKill, TeamKill) Sound
* Custom Quake Events (Suicide, Revenge, FirstBlood, RoundStart, RoundPrepare, LastManStanding, RageQuit) Sound
* Custom Dink / Hit / Kill Sounds
* Multiple Packs Male,Female,... 
* Volume Kill Sound Client Side
* Toggle Kill Chat / Center / Center Bottom Client Side
* Save Client Preferences MySql/Local Cookies Cross Servers


## .:[ Dependencies ]:.

[Metamod:Source (2.x)](https://www.sourcemm.net/downloads.php/?branch=master)

[MultiAddonManager](https://github.com/Source2ZE/MultiAddonManager)

[CounterStrikeSharp](https://github.com/roflmuffin/CounterStrikeSharp/releases)

[Newtonsoft.Json](https://www.nuget.org/packages/Newtonsoft.Json)

[MySqlConnector](https://www.nuget.org/packages/MySqlConnector)

## .:[ Configuration ]:.

> [!CAUTION]
> Config Located In ..\addons\counterstrikesharp\plugins\Quake-Kill-Sounds-GoldKingZ\config\config.json                                         

```json

{
  //Key To Active Plugin
  "KEY": "",

  //Change Check IpAdress To WebSite
  "ChangeCheckIpAdressToWebSite": "XXXXXXXXX.YYY",

//----------------------------[ ↓ Main Configs ↓ ]-------------------------------

  //Open Menu Mode:
  //0 = Disable Menu
  //1 = Custom Chat Menu By GoldKingZ
  //2 = Custom Chat Menu By GoldKingZ
  //3 = WASD Menu By GoldKingZ
  "OpenMenu_Mode": 3,

  //Allow These Groups Only To Open Kill/Quake (Make It Empty "" To Let AnyOne)  [Example:@css/root,@css/admin,@css/vip,#css/admin,#css/vip]
  "OpenMenu_Flags": "",

  //Commands In Game To Open Kill/Quake Menu
  "OpenMenu_CommandsInGame": "!kill,!killsounds,!killsound,!quake,!quakesounds,!quakesound,!qs",

  //Allow These Groups Only To Reload Json
  "Reload_Json_Flags": "@css/root,@css/admin,#css/root,#css/admin",

  //Commands In Game To Reload Json
  "Reload_Json_CommandsInGame": "!reloadquack,!reloadkill",

//----------------------------[ ↓ Quake Configs ↓ ]-------------------------------

  //Enable Quake OnWarmUp?
  "Quake_DisableOnWarmUp": true,

  //Reset KillStreaks On Every Round Start?
  "Quake_ResetKillStreakOnEveryRoundStart": true,

  //Pick Random Quake Sounds The One Selected?
  //true = Yes
  //false = No, Pick From Top To Bottom
  "Quake_Pick_Random_Sounds": true,

  //Available Quake Volumes To Clients 
  "Quake_AvailableVolumes": "0,20,40,60,80,100",

  //Default Quake Volume To Clients
  "Quake_Menu_DefaultVolume": "40",

  //Default Sound Pack It Will Get male Unique_Name
  "Quake_Menu_DefaultSoundPack": "male",

  //Default Quake ShowChat To Clients
  "Quake_Menu_DefaultShowChat": true,

  //Default Quake ShowCenter To Clients
  "Quake_Menu_DefaultShowCenter": true,

  //Default Quake ShowCenterBottom To Clients
  "Quake_Menu_DefaultShowCenterBottom": true,

//----------------------------[ ↓ Kill Configs ↓ ]-------------------------------

  //Enable Kill OnWarmUp?
  "Kill_DisableOnWarmUp": false,

  //Pick Random Kill Sounds The One Selected?
  //true = Yes
  //false = No, Pick From Top To Bottom
  "Kill_Pick_Random_Sounds": true,

  //Available Kill Volumes To Clients 
  "Kill_AvailableVolumes": "0,20,40,60,80,100",

  //Default Kill Volume To Clients
  "Kill_Menu_DefaultVolume": "40",

  //Default HeadShot Kill To Clients
  "Kill_Menu_DefaultHeadShotKill": "None",

  //Default HeadShot Hit To Clients
  "Kill_Menu_DefaultHeadShotHit": "None",

  //Default BodyShot Kill To Clients
  "Kill_Menu_DefaultBodyKill": "None",

  //Default BodyShot Hit To Clients
  "Kill_Menu_DefaultBodyHit": "None",

//----------------------[ ↓ Save Players Data By Cookies Locally ↓ ]----------------------

  //Enable Cookies?
  //true = Yes, (Will Be Located In ../Quake-Kill-Sounds-GoldKingZ/Cookies/Cookies.json)
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

//----------------------------[ ↓ Debug ↓ ]----------------------------------------------

  //Enable Debug Will Print Server Console If You Face Any Issue
  "EnableDebug": false,
}

```


## .:[ Configuration Kill_Settings ]:.

> [!CAUTION]
> Config Located In ..\addons\counterstrikesharp\plugins\Quake-Kill-Sounds-GoldKingZ\config\Kill_Settings.json                                                        

```json
//==========================
//        Options
//==========================
// "Hide_It_And_Show_Only_ForFlags": "@css/root,@css/vip" //Hide Menu/SubMenu And Only These Flags Can See It
// "Only_These_Flags_Can_Access_It": "@css/root,@css/vip" //Only These Can Access Menu/SubMenuz
// "Only_These_Flags_Can_Vol.0": "@css/vip,#css/vip" //Only These Can Access To Toggle Volume 0 As Example To (SubMenu.STATUS.QUAKEVOL. OR SubMenu.STATUS.KILLVOL.)
// "SubMenu.STATUS.QUAKESELECTED.xxxxxxxxxxx:":{} //Show Client His Current Selected Quake
// "SubMenu.STATUS.QUAKEVOL.xxxxxxxxxxx:":{} //Show Client His Current Quake Volume
// "SubMenu.STATUS.QUAKECHAT.xxxxxxxxxxx:":{} //Show Client His Current Quake Show Chat
// "SubMenu.STATUS.QUAKECENTER.xxxxxxxxxxx:":{} //Show Client His Current Quake Center
// "SubMenu.STATUS.QUAKECENTERBOTTOM.xxxxxxxxxxx:":{} //Show Client His Current Quake Center Bottom
// "SubMenu.STATUS.KILLHKSELECTED.xxxxxxxxxxx:":{} //Show Client His Current Selected HeadShot Kill
// "SubMenu.STATUS.KILLHHSELECTED.xxxxxxxxxxx:":{} //Show Client His Current Selected HeadShot Hit
// "SubMenu.STATUS.KILLBKSELECTED.xxxxxxxxxxx:":{} //Show Client His Current Selected BodyShot Kill
// "SubMenu.STATUS.KILLBHSELECTED.xxxxxxxxxxx:":{} //Show Client His Current Selected BodyShot Hit
// "SubMenu.STATUS.KILLHKNONSELECTED.xxxxxxxxxxx:":{} //Ability To Disable Custom HeadShot Kill
// "SubMenu.STATUS.KILLHHNONSELECTED.xxxxxxxxxxx:":{} //Ability To Disable Custom HeadShot Hit
// "SubMenu.STATUS.KILLBKNONSELECTED.xxxxxxxxxxx:":{} //Ability To Disable Custom BodyShot Kill
// "SubMenu.STATUS.KILLBHNONSELECTED.xxxxxxxxxxx:":{} //Ability To Disable Custom BodyShot Hit
// "SubMenu.STATUS.KILLVOL.xxxxxxxxxxx:":{} //Show Client His Current Kill Volume
// "Unique_Name": "Bamboo", //Unique Name To Let Plugin Search For It
// "Make_It_Previewable": true, //true = Make Sound Previewable Before Select It //false OR Not Used = Wil Be Disabled
// "Priority_Controller": "KillStreak_26,KillStreak_24", //Left Is High Priority To Right Lower Priority (Will Override Any Sound)
// "ComboTimeInSecs": 2, //Time In Secs After Each Kill To Count Combo Kills
// "RageQuitInSecs": 10, //Time In Secs After Player Death If Player Left With 10 Secs Example Will Play Sound
// "PlaySound_Mode": "2,3", // 1- Play sound to everyone // 2- Play sound to attacker // 3- Play sound to victim
// "ShowChat_Mode": "2,3", // 1- Show Chat to everyone // 2- Show Chat to attacker // 3- Show Chat to victim
// "ShowCenter_Mode": "2,3:10", // 1- Show Center to everyone // 2- Show Center to attacker // 3- Show Center to victim  (After : Is How Much In Secs Duration Show Center Not Using It Will Be Default 5 Secs)
// "ShowCenter_Bottom_Mode": "2,3:10", // 1- Show Center Bottom to everyone // 2- Show Center Bottom to attacker // 3- Show Center Bottom to victim  (After : Is How Much In Secs Duration Show Center Bottom Not Using It Will Be Default 5 Secs) 
// "Sound_Paths": // Sound Path Of Music Added As Many Music As You Like
//============================================
//        Quake Can Be Trackable Add _1 _2 _3
//============================================
// "KillStreak": // Kill Streaks Will Reset On Death
// "ComboKill": // Kills Per ComboTimeInSecs Will Reset If Time Pass With No Kills
// "HeadShotKill": // HeadShot Kills Will Reset On Death 
// "KnifeKill": // Knife Kills Will Reset On Death 
// "GrenadeKill": // Grenade Kills Will Reset On Death
// "MollyKill": // Molly Kills Will Reset On Death
// "TaserKill": // Taser Kills Will Reset On Death
// "NoScopeKill": // No Scope Kills Will Reset On Death
// "OnAirKill": // On Air Kills Will Reset On Death
// "TeamKill": // Team Kill Will Reset On Death
// "TeamKill": // Team Kill Will Reset On Death
//============================================
//        Quake Events
//============================================
// "Suicide": // When Player Kill Him Self
// "Revenge": // When Player Kill His Last Player Killed Him
// "FirstBlood": // First Kill When On Every New Round Start
// "RoundStart": // Round Start 
// "RoundPrepare": // When There Is (mp_freezetime)
// "LastManStanding": // Last Player Alive In CT OR T
// "RageQuit": // After Player Got Killed Will Track RageQuitInSecs If He Left Fast RageQuit Will Play
//==========================

{
	"Menu.xxxxxxxx": //After Menu. Is Menu Name
	{
		"SubMenu.xxxxxxxx": //After SubMenu. Is The Name Of Submenu
		{
      "Unique_Name": "male",

      "Priority_Controller": "KillStreak_26,KillStreak_24,KillStreak_22,KillStreak_20,KillStreak_18,KillStreak_16,KillStreak_14,KillStreak_10,KillStreak_8,HeadShotKill_5",
      "ComboTimeInSecs": 2,
      "RageQuitInSecs": 10,
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

	"PrintChatToPlayer.Menu.Disabled": "{green}Gold KingZ {grey}| {darkred}Quake Menu Is {darkred}Disabled By The Server",
	"PrintChatToPlayer.Menu.Not.Allowed": "{green}Gold KingZ {grey}| {darkred}Quake Menu Is For {lime}VIPS {darkred}Only",
	"PrintChatToPlayer.ReloadJson.Not.Allowed": "{green}Gold KingZ {grey}| {darkred}You Dont Have Permission To Access This",
	"PrintChatToPlayer.Menu.Selected.Not.Allowed": "{green}Gold KingZ {grey}| {darkred}You Dont Have Permission To Access This",

	"PrintChatToPlayer.Selected.QUAKE": "{green}Gold KingZ {grey}| Your Selected Now: {lime}{0}",
	"PrintChatToPlayer.Selected.QUAKEVOL": "{green}Gold KingZ {grey}| {grey}Quake Volume Set To: {lime}{0}",
	"PrintChatToPlayer.Selected.QUAKEVOL.0": "{green}Gold KingZ {grey}| {grey}Quake Volume Set To: {darkred}Muted",
	"PrintChatToPlayer.Selected.QUAKECHAT.Enabled": "{green}Gold KingZ {grey}| Quake Chat Set To: {lime}Enabled",
	"PrintChatToPlayer.Selected.QUAKECHAT.Disabled": "{green}Gold KingZ {grey}| Quake Chat Set To: {darkred}Disabled",
	"PrintChatToPlayer.Selected.QUAKECENTER.Enabled": "{green}Gold KingZ {grey}| Quake Center Set To: {lime}Enabled",
	"PrintChatToPlayer.Selected.QUAKECENTER.Disabled": "{green}Gold KingZ {grey}| Quake Center Set To: {darkred}Disabled",
	"PrintChatToPlayer.Selected.QUAKECENTERBOTTOM.Enabled": "{green}Gold KingZ {grey}| Quake Center Bottom Set To: {lime}Enabled",
	"PrintChatToPlayer.Selected.QUAKECENTERBOTTOM.Disabled": "{green}Gold KingZ {grey}| Quake Center Bottom Set To: {darkred}Disabled",

	"PrintChatToPlayer.Selected.KILLHK": "{green}Gold KingZ {grey}| HeadShot Kill Now: {lime}{0}",
	"PrintChatToPlayer.Selected.KILLHH": "{green}Gold KingZ {grey}| HeadShot Hit Now: {lime}{0}",
	"PrintChatToPlayer.Selected.KILLBK": "{green}Gold KingZ {grey}| BodyShot Kill Now: {lime}{0}",
	"PrintChatToPlayer.Selected.KILLBH": "{green}Gold KingZ {grey}| BodyShot Hit Now: {lime}{0}",
	"PrintChatToPlayer.Selected.KILLVOL": "{green}Gold KingZ {grey}| {grey}Kill Volume Set To: {lime}{0}",
	"PrintChatToPlayer.Selected.KILLVOL.0": "{green}Gold KingZ {grey}| {grey}Kill Volume Set To: {darkred}Muted",

	//==========================
	//    Quake Kill Sounds
	//==========================
	//{0} = Attacker Player Name
	//{1} = Victim Player Name
	//{2} = How Much Kills 
	//==========================
	
	"ShowChat.FirstBlood": "{green}Gold KingZ {grey}| FirstBlood !!!  {purple}{0} {red}Killed  {purple}{1}",
	"ShowCenter.RoundPrepare": "<font color='#cc66ff'>Prepare For Battle",
	"ShowCenter.RoundStart": "<font color='#99ff66'>Play !",
	"ShowChat.LastManStanding": "{green}Gold KingZ {grey}| You The Last Man Standing",
	"ShowChat.RageQuit": "{green}Gold KingZ {grey}| {purple}{1} {grey}Rage Quit",
	"ShowChat.Revenge": "{green}Gold KingZ {grey}| {purple}{0} {grey}Got His Revenge From {purple}{1}",
	"ShowChat.KnifeKill": "{green}Gold KingZ {grey}| {purple}{0} {red}✄Knife Kill✄ {purple}{1}",
	"ShowChat.TeamKill": "{green}Gold KingZ {grey}| {purple}{0} {red}Team Kill {purple}{1}",
	"ShowChat.ComboKill_2": "{green}Gold KingZ {grey}| {purple}{0} {grey}Did {lime}{2} Combo Kills!",
	"ShowChat.ComboKill_3": "{green}Gold KingZ {grey}| {purple}{0} {grey}Did {lime}HaaaatTrick Combo Kills!",
	"ShowChat.ComboKill_4": "{green}Gold KingZ {grey}| {purple}{0} {grey}Did {green}Multikill Combo Kills!",
	"ShowChat.ComboKill_5": "{green}Gold KingZ {grey}| {purple}{0} {grey}Did {darkred}{2} Combo Kills!!!",
	"ShowCenter.ComboKill_5": "<font color='purple'>{0} <font color='green'>Is On Fire !!!! Did {2} Combo Kills!!!!!!! <br> <img src='https://raw.githubusercontent.com/oqyh/cs2-Quake-Kill-Sounds-GoldKingZ/main/Resources/ComboKill_5.gif' class=''> <br>",
	"ShowChat.HeadShotKill_3": "{green}Gold KingZ {grey}| {purple}{0} {grey}Did {lime}{2} HeadShot Kills!",
	"ShowChat.HeadShotKill_5": "{green}Gold KingZ {grey}| {purple}{0} {grey}Did {darkred}{2} HeadShot Kills!!!",
	"ShowChat.KillStreak": "{green}Gold KingZ {grey}| {purple}{0} {grey}Is On {lime}{2} KillStreak",
	"ShowChat.KillStreak_16": "{green}Gold KingZ {grey}| {purple}{0} {grey}Is On {lime}{2} KillStreak !!!!",
	"ShowChat.KillStreak_18": "{green}Gold KingZ {grey}| {purple}{0} {darkred}GodLike !!  {darkred}{2} KillStreak !!",
	"ShowCenter.KillStreak_18": "<font color='purple'>{0} <font color='green'>GodLike !! {2} KillStreak!! <br> <img src='https://raw.githubusercontent.com/oqyh/cs2-Quake-Kill-Sounds-GoldKingZ/main/Resources/KillStreak_18.gif' class=''> <br>",
	"ShowChat.KillStreak_20": "{green}Gold KingZ {grey}| {purple}{0} {darkred}Whicked Sick !!  {darkred}{2} KillStreak !!",
	"ShowCenter.KillStreak_20": "<font color='purple'>{0} <font color='green'>Whicked Sick !! {2} KillStreak!! <br> <img src='https://raw.githubusercontent.com/oqyh/cs2-Quake-Kill-Sounds-GoldKingZ/main/Resources/KillStreak_20.gif' class=''> <br>",
	"ShowChat.KillStreak_22": "{green}Gold KingZ {grey}| {purple}{0} {darkred}Mega Kill !!  {darkred}{2} KillStreak !!",
	"ShowCenter.KillStreak_22": "<font color='purple'>{0} <font color='green'>Mega Kill !! {2} KillStreak!! <br> <img src='https://raw.githubusercontent.com/oqyh/cs2-Quake-Kill-Sounds-GoldKingZ/main/Resources/KillStreak_22.gif' class=''> <br>",
	"ShowChat.KillStreak_24": "{green}Gold KingZ {grey}| {purple}{0} {darkred}Ludicrous Kill !!  {darkred}{2} KillStreak !!",
	"ShowCenter.KillStreak_24": "<font color='purple'>{0} <font color='green'>Ludicrous Kill !! {2} KillStreak!! <br> <img src='https://raw.githubusercontent.com/oqyh/cs2-Quake-Kill-Sounds-GoldKingZ/main/Resources/KillStreak_24.gif' class=''> <br>",
	"ShowChat.KillStreak_26": "{green}Gold KingZ {grey}| {purple}{0} {darkred}Holyyyyyyy Shhiiiiiiit !!!! {darkred}{2} KillStreak !!",
	"ShowCenter.KillStreak_26": "<font color='purple'>{0} <font color='green'>Holyyyyyyy Shhiiiiiiit !!!!  {2} KillStreak!! <br> <img src='https://raw.githubusercontent.com/oqyh/cs2-Quake-Kill-Sounds-GoldKingZ/main/Resources/KillStreak_26.gif' class=''> <br>",


	"Mode_1.MainMenu.Title": "{Magenta} Quake/Kill Menu",
	"Mode_1.SubMenu.Title": "{Purple} .:[ {0} ]:.",

	"Mode_1.Previewable.Title": "{White}Set {Blue}{0} {White}?",
	"Mode_1.Previewable.Yes": "{Lime}Yes",
	"Mode_1.Previewable.No": "{LightRed}No",
	"Mode_1.Previewable.Preview": "{Olive}Play The Sound",

	"Mode_1.STATUS.QUAKESELECTED": "{Gold} {0}",
	"Mode_1.STATUS.QUAKEVOL": "{Lime} {0} %",
	"Mode_1.STATUS.QUAKEVOL.0": "{Darkred} Muted",
	"Mode_1.STATUS.QUAKECHAT.Enabled": "{Lime} ✔",
	"Mode_1.STATUS.QUAKECHAT.Disabled": "{Darkred} ✖",
	"Mode_1.STATUS.QUAKECENTER.Enabled": "{Lime} ✔",
	"Mode_1.STATUS.QUAKECENTER.Disabled": "{Darkred} ✖",
	"Mode_1.STATUS.QUAKECENTERBOTTOM.Enabled": "{Lime} ✔",
	"Mode_1.STATUS.QUAKECENTERBOTTOM.Disabled": "{Darkred} ✖",

	"Mode_1.STATUS.KILLVOL": "{Lime} {0} %",
	"Mode_1.STATUS.KILLVOL.0": "{Darkred} Muted",
	"Mode_1.STATUS.KILLHKSELECTED": "{Gold} {0}",
	"Mode_1.STATUS.KILLHKSELECTED.None": "{Darkred} {0}",
	"Mode_1.STATUS.KILLHHSELECTED": "{Gold} {0}",
	"Mode_1.STATUS.KILLHHSELECTED.None": "{Darkred} {0}",
	"Mode_1.STATUS.KILLBKSELECTED": "{Gold} {0}",
	"Mode_1.STATUS.KILLBKSELECTED.None": "{Darkred} {0}",
	"Mode_1.STATUS.KILLBHSELECTED": "{Gold} {0}",
	"Mode_1.STATUS.KILLBHSELECTED.None": "{Darkred} {0}",



	"Mode_2.MainMenu.Title": "<font class='fontSize-M' color='#b74eae'> Quake/Kill Menu</font>",
	"Mode_2.SubMenu.Title": "<font class='fontSize-M' color='#f809e6'> .:[ {0} ]:. </font>",

	"Mode_2.Previewable.Title": "<font color='white'>Set <font color='#00f0ff'>{0} <font color='white'>?",
	"Mode_2.Previewable.Yes": "<font color='#0cff00'>Yes",
	"Mode_2.Previewable.No": "<font color='#ff2d00'>No",
	"Mode_2.Previewable.Preview": "<font color='#91dd02'>Play The Sound",

	"Mode_2.STATUS.QUAKESELECTED": "<font color='gold'> {0}",
	"Mode_2.STATUS.QUAKEVOL": "<font color='#0cff00'> {0} %",
	"Mode_2.STATUS.QUAKEVOL.0": "<font color='#ff2d00'> Muted",
	"Mode_2.STATUS.QUAKECHAT.Enabled": "<font color='#0cff00'> ✔",
	"Mode_2.STATUS.QUAKECHAT.Disabled": "<font color='#ff2d00'> ✖",
	"Mode_2.STATUS.QUAKECENTER.Enabled": "<font color='#0cff00'> ✔",
	"Mode_2.STATUS.QUAKECENTER.Disabled": "<font color='#ff2d00'> ✖",
	"Mode_2.STATUS.QUAKECENTERBOTTOM.Enabled": "<font color='#0cff00'> ✔",
	"Mode_2.STATUS.QUAKECENTERBOTTOM.Disabled": "<font color='#ff2d00'> ✖",

	"Mode_2.STATUS.KILLVOL": "<font color='#0cff00'> {0} %",
	"Mode_2.STATUS.KILLVOL.0": "<font color='#ff2d00'> Muted",
	"Mode_2.STATUS.KILLHKSELECTED": "<font color='#ffd700'> {0}",
	"Mode_2.STATUS.KILLHKSELECTED.None": "<font color='#ff0c00'> {0}",
	"Mode_2.STATUS.KILLHHSELECTED": "<font color='#ffd701'> {0}",
	"Mode_2.STATUS.KILLHHSELECTED.None": "<font color='#ff0900'> {0}",
	"Mode_2.STATUS.KILLBKSELECTED": "<font color='#ffd702'> {0}",
	"Mode_2.STATUS.KILLBKSELECTED.None": "<font color='#ff0600'> {0}",
	"Mode_2.STATUS.KILLBHSELECTED": "<font color='#ffd703'> {0}",
	"Mode_2.STATUS.KILLBHSELECTED.None": "<font color='#ff0300'> {0}",



	"Mode_3.MainMenu.Title": "<font class='fontSize-M' color='#b74eae'> Quake/Kill Menu</font>",
	"Mode_3.SubMenu.Title": "<font class='fontSize-M' color='#f809e6'> .:[ {0} ]:. </font>",

	"Mode_3.Previewable.Title": "<font color='white'>Set <font color='#00f0ff'>{0} <font color='white'>?",
	"Mode_3.Previewable.Yes": "<font color='#0cff00'>Yes",
	"Mode_3.Previewable.No": "<font color='#ff2d00'>No",
	"Mode_3.Previewable.Preview": "<font color='#91dd02'>Play The Sound",

	"Mode_3.STATUS.QUAKESELECTED": "<font color='gold'> {0}",
	"Mode_3.STATUS.QUAKEVOL": "<font color='#0cff00'> {0} %",
	"Mode_3.STATUS.QUAKEVOL.0": "<font color='#ff2d00'> Muted",
	"Mode_3.STATUS.QUAKECHAT.Enabled": "<font color='#0cff00'> ✔",
	"Mode_3.STATUS.QUAKECHAT.Disabled": "<font color='#ff2d00'> ✖",
	"Mode_3.STATUS.QUAKECENTER.Enabled": "<font color='#0cff00'> ✔",
	"Mode_3.STATUS.QUAKECENTER.Disabled": "<font color='#ff2d00'> ✖",
	"Mode_3.STATUS.QUAKECENTERBOTTOM.Enabled": "<font color='#0cff00'> ✔",
	"Mode_3.STATUS.QUAKECENTERBOTTOM.Disabled": "<font color='#ff2d00'> ✖",

	"Mode_3.STATUS.KILLVOL": "<font color='#0cff00'> {0} %",
	"Mode_3.STATUS.KILLVOL.0": "<font color='#ff2d00'> Muted",
	"Mode_3.STATUS.KILLHKSELECTED": "<font color='#ffd700'> {0}",
	"Mode_3.STATUS.KILLHKSELECTED.None": "<font color='#ff0c00'> {0}",
	"Mode_3.STATUS.KILLHHSELECTED": "<font color='#ffd701'> {0}",
	"Mode_3.STATUS.KILLHHSELECTED.None": "<font color='#ff0900'> {0}",
	"Mode_3.STATUS.KILLBKSELECTED": "<font color='#ffd702'> {0}",
	"Mode_3.STATUS.KILLBKSELECTED.None": "<font color='#ff0600'> {0}",
	"Mode_3.STATUS.KILLBHSELECTED": "<font color='#ffd703'> {0}",
	"Mode_3.STATUS.KILLBHSELECTED.None": "<font color='#ff0300'> {0}"
}

```

## .:[ Change Log ]:.
```
(1.0.0)
-Initial Release
```
