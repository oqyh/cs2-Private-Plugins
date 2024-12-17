
## .:[ Price ]:. [(Free Private Rules)](https://github.com/oqyh/cs2-Private-Plugins/blob/11b92dc04067753a390d796dbba39d789f270aab/README.md?plain=1#L27)
```diff
+ PRICE FREE [Only Discord Members (Limited Time Only)] 
```

# [CS2] MVP-N-RoundEnd-Music-GoldKingZ (1.0.0)  

## Video ShowCase Of Plugin

[![MVP-N-RoundEnd-Music-GoldKingZ](https://img.youtube.com/vi/Gm0OE0n7JD4/0.jpg)](https://youtu.be/Gm0OE0n7JD4)


* Custom Mvp Music
* Custom Round End Music
* Volume Mvp Music Client Side
* Volume Round End Music Client Side
* Toggle Mvp + Round End Chat / Center / Center Bottom Client Side
* Save Client Preferences MySql/Local Cookies Cross Servers




## .:[ Dependencies ]:.

[Metamod:Source (2.x)](https://www.sourcemm.net/downloads.php/?branch=master)

[MultiAddonManager](https://github.com/Source2ZE/MultiAddonManager)

[CounterStrikeSharp](https://github.com/roflmuffin/CounterStrikeSharp/releases)

[Newtonsoft.Json](https://www.nuget.org/packages/Newtonsoft.Json)

[MySqlConnector](https://www.nuget.org/packages/MySqlConnector)

## .:[ Configuration ]:.

> [!CAUTION]
> Config Located In ..\addons\counterstrikesharp\plugins\MVP-N-RoundEnd-Music-GoldKingZ\config\config.json                                         

```json

{
  //Key To Active Plugin
  "KEY": "",

  //Change Check IpAdress To WebSite
  "ChangeCheckIpAdressToWebSite": "XXXXXXXXX.YYY",

//----------------------------[ ↓ Main Configs ↓ ]-------------------------------

  //Disable Default MVP Music?
  //true = Yes Completely
  //false = Only If Custom MVP/Round End Music Is Playing
  "Disable_Default_MVP_Music_Completely": false,

  //Custom Music length So It Will Apply When Round Finish
  "Custom_Music_length_InSecs": 10,

  //Open Menu Mode:
  //0 = Disable Menu
  //1 = Custom Chat Menu By GoldKingZ
  //2 = Custom Chat Menu By GoldKingZ
  //3 = WASD Menu By GoldKingZ
  "OpenMenu_Mode": 3,

  //Allow These Groups Only To Open MVP/RES (Make It Empty "" To Let AnyOne)  [Example:@css/root,@css/admin,@css/vip,#css/admin,#css/vip]
  "OpenMenu_Flags": "",

  //Commands In Game To Open MVP/RES Menu
  "OpenMenu_CommandsInGame": "!mvp,!mvps,!res",

  //Allow These Groups Only To Reload Json
  "Reload_Json_Flags": "@css/root,@css/admin,#css/root,#css/admin",

  //Commands In Game To Reload Json
  "Reload_Json_CommandsInGame": "!reloadmvp,!reloadres",

//----------------------------[ ↓ MVP Configs ↓ ]-------------------------------

  //Enable Custom MVP?
  //true = Yes, (Keep In Mind This Will Override Custom RES If There Is Custom MVP, If There Is Not Custom MVP Then This Will Get Skipped)
  //false = Disable Custom MVP
  "Enable_Custom_MVP": true,

  //Pick Random MVP Music The One Selected?
  //true = Yes
  //false = No, Pick From Top To Bottom
  "MVP_Pick_Random_Music": true,

  //Available MVP Volumes To Clients 
  "MVP_AvailableVolumes": "0,20,40,60,80,100",

  //Default MVP Volume To Clients
  "MVP_Menu_DefaultVolume": "40",

  //Default MVP ShowChat To Clients
  "MVP_Menu_DefaultShowChat": true,

  //Default MVP ShowCenter To Clients
  "MVP_Menu_DefaultShowCenter": true,

  //Default MVP ShowCenterBottom To Clients
  "MVP_Menu_DefaultShowCenterBottom": true,

//----------------------------[ ↓ Round End Configs ↓ ]-------------------------------

  //Enable Custom Round End?
  //true = Yes, (Keep In Mind This Will Get Override By MVP If There Is Custom MVP, If There Is Not Custom MVP Then This Will Get Played)
  //false = Disable Custom Round End
  "Enable_Custom_RES": true,

  //Pick Random Round End Music The One Selected?
  //true = Yes
  //false = No, Pick From Top To Bottom
  "RES_Pick_Random_Music": true,

  //Available Round End Volumes To Clients 
  "RES_AvailableVolumes": "0,20,40,60,80,100",

  //Default Round End Volume To Clients
  "RES_Menu_DefaultVolume": "40",

  //Default Round End ShowChat To Clients
  "RES_Menu_DefaultShowChat": true,

  //Default Round End ShowCenter To Clients
  "RES_Menu_DefaultShowCenter": true,

  //Default Round End ShowCenterBottom To Clients
  "RES_Menu_DefaultShowCenterBottom": true,

//----------------------[ ↓ Save Players Data By Cookies Locally ↓ ]----------------------

  //Enable Cookies?
  //true = Yes, (Will Be Located In ../MVP-N-RoundEnd-Music-GoldKingZ/Cookies/Cookies.json)
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


## .:[ Configuration MVP_N_RES_Settings ]:.

> [!CAUTION]
> ReservedSlots Config Located In ..\addons\counterstrikesharp\plugins\MVP-N-RoundEnd-Music-GoldKingZ\config\MVP_N_RES_Settings.json                                                        

```json
//==========================
//        Options
//==========================
// "Hide_It_And_Show_Only_ForFlags": "@css/root,@css/vip" //Hide Menu/SubMenu And Only These Flags Can See It
// "Only_These_Flags_Can_Access_It": "@css/root,@css/vip" //Only These Can Access Menu/SubMenuz
// "Only_These_Flags_Can_Vol.0": "@css/vip,#css/vip" //Only These Can Access To Toggle Volume 0 As Example To (SubMenu.STATUS.MVPVOL. OR SubMenu.STATUS.RESCHAT.)
// "SubMenu.STATUS.MVPSELECTED.xxxxxxxxxxx:":{} //Show Client His Current Selected MVP
// "SubMenu.STATUS.MVPNONSELECTED.xxxxxxxxxxx:":{} //Ability To Disable Custom MVP
// "SubMenu.STATUS.MVPVOL.xxxxxxxxxxx:":{} //Show Client His Current MVP Volume
// "SubMenu.STATUS.MVPCHAT.xxxxxxxxxxx:":{} //Show Client His Current MVP Show Chat
// "SubMenu.STATUS.MVPCENTER.xxxxxxxxxxx:":{} //Show Client His Current MVP Center
// "SubMenu.STATUS.MVPCENTERBOTTOM.xxxxxxxxxxx:":{} //Show Client His Current MVP Center Bottom
// "SubMenu.STATUS.RESVOL.xxxxxxxxxxx:":{} //Show Client His Current Round End Volume
// "SubMenu.STATUS.RESCHAT.xxxxxxxxxxx:":{} //Show Client His Current Round End Show Chat
// "SubMenu.STATUS.RESCENTER.xxxxxxxxxxx:":{} //Show Client His Current Round End Center
// "SubMenu.STATUS.RESCENTERBOTTOM.xxxxxxxxxxx:":{} //Show Client His Current Round End Center Bottom
// "Unique_Name": "9mm", //Unique Name To Let Plugin Search For It
// "Make_It_Previewable": true, //true = Make Music Previewable Before Select It //false OR Not Used = Wil Be Disabled
// "Sound_Paths": // Sound Path Of Music Added As Many Music As You Like
//==========================

{
	"RES.Lithe - Hold Out": //Start With RES. Will Be Hidden Its For Round End Configuration
	{
		"ShowChat": true,
		"ShowCenter": 10,
		"Sound_Paths":
		[
			"sounds/goldkingz/res/100_volume/holdout1.vsnd",
			"sounds/goldkingz/res/100_volume/holdout2.vsnd"
		]
	}

	"Menu.Free MVPs": //After Menu. Is Menu Name
	{
		"SubMenu.9MM - Memphis Cult": //After SubMenu. Is The Name Of Submenu
		{
			"Unique_Name": "9mm",
			
			"Make_It_Previewable": true,
			"ShowChat": true,
			"ShowCenter": 10,
			"Sound_Paths":
			[
				"sounds/goldkingz/mvp/100_volume/9mm.vsnd"
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
	
	"PrintChatToPlayer.Menu.Disabled": "{green}Gold KingZ {grey}| {darkred}MVP/RES Menu Is {darkred}Disabled By The Server",
	"PrintChatToPlayer.Menu.Not.Allowed": "{green}Gold KingZ {grey}| {darkred}MVP/RES Menu Is For {lime}VIPS {darkred}Only",
	"PrintChatToPlayer.ReloadJson.Not.Allowed": "{green}Gold KingZ {grey}| {darkred}You Dont Have Permission To Access This",
	"PrintChatToPlayer.Menu.Selected.Not.Allowed": "{green}Gold KingZ {grey}| {darkred}You Dont Have Permission To Access This",
	
	"PrintChatToPlayer.Selected.MVP": "{green}Gold KingZ {grey}| Your Mvp Now: {lime}{0}",
	"PrintChatToPlayer.Selected.MVPVOL": "{green}Gold KingZ {grey}| MVP Volume Set To: {lime}{0}",
	"PrintChatToPlayer.Selected.MVPVOL.0": "{green}Gold KingZ {grey}| MVP Volume Set To: {darkred}Muted",
	"PrintChatToPlayer.Selected.MVPCHAT.Enabled": "{green}Gold KingZ {grey}| MVP Chat Set To: {lime}Enabled",
	"PrintChatToPlayer.Selected.MVPCHAT.Disabled": "{green}Gold KingZ {grey}| MVP Chat Set To: {darkred}Disabled",
	"PrintChatToPlayer.Selected.MVPCENTER.Enabled": "{green}Gold KingZ {grey}| MVP Center Set To: {lime}Enabled",
	"PrintChatToPlayer.Selected.MVPCENTER.Disabled": "{green}Gold KingZ {grey}| MVP Center Set To: {darkred}Disabled",
	"PrintChatToPlayer.Selected.MVPCENTERBOTTOM.Enabled": "{green}Gold KingZ {grey}| MVP Center Bottom Set To: {lime}Enabled",
	"PrintChatToPlayer.Selected.MVPCENTERBOTTOM.Disabled": "{green}Gold KingZ {grey}| MVP Center Bottom Set To: {darkred}Disabled",
	
	"PrintChatToPlayer.Selected.RESVOL": "{green}Gold KingZ {grey}| RES Volume Set To: {lime}{0}",
	"PrintChatToPlayer.Selected.RESVOL.0": "{green}Gold KingZ {grey}| RES Volume Set To: {darkred}Muted",
	"PrintChatToPlayer.Selected.RESCHAT.Enabled": "{green}Gold KingZ {grey}| RES Chat Set To: {lime}Enabled",
	"PrintChatToPlayer.Selected.RESCHAT.Disabled": "{green}Gold KingZ {grey}| RES Chat Set To: {darkred}Disabled",
	"PrintChatToPlayer.Selected.RESCENTER.Enabled": "{green}Gold KingZ {grey}| RES Center Set To: {lime}Enabled",
	"PrintChatToPlayer.Selected.RESCENTER.Disabled": "{green}Gold KingZ {grey}| RES Center Set To: {darkred}Disabled",
	"PrintChatToPlayer.Selected.RESCENTERBOTTOM.Enabled": "{green}Gold KingZ {grey}| RES Center Bottom Set To: {lime}Enabled",
	"PrintChatToPlayer.Selected.RESCENTERBOTTOM.Disabled": "{green}Gold KingZ {grey}| RES Center Bottom Set To: {darkred}Disabled",
	
	//==========================
	//        MVP Music
	//==========================
	//{0} = Player Name Of Who MVP Of The Match
	//{1} = Selected Name Of MVP
	//==========================
	
	"MVP.ShowChat": "{green}Gold KingZ {grey}| {lightblue}{0} {grey}Is MVP Of The Match! {nextline}{green}Gold KingZ {grey}| Now Playing {purple}{1}",
	"MVP.ShowCenter": "<font color='purple'>{0} <font color='white'>Is MVP Of The Match! <br> <br> <font color='white'>Playing <font color='green'>{1}",
	"MVP.ShowCenter.9MM - Memphis Cult": "<font color='purple'>{0} <font color='white'>Is MVP Of The Match! <br> <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/main/cs2-MVP-N-RoundEnd-Music-GoldKingZ/Resources/9mm.gif' class=''> <br> <br> <font color='white'>Playing <font color='green'>{1}",
	"MVP.ShowCenter.дурной вкус - пластинки": "<font color='purple'>{0} <font color='white'>Is MVP Of The Match! <br> <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/main/cs2-MVP-N-RoundEnd-Music-GoldKingZ/Resources/badtaste.gif' class=''> <br> <br> <font color='white'>Playing <font color='green'>{1}",
	"MVP.ShowCenter.Playboi Carti - Beef": "<font color='purple'>{0} <font color='white'>Is MVP Of The Match! <br> <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/main/cs2-MVP-N-RoundEnd-Music-GoldKingZ/Resources/beef.gif' class=''> <br> <br> <font color='white'>Playing <font color='green'>{1}",
	"MVP.ShowCenter.BigXthaPlug - Change Me": "<font color='purple'>{0} <font color='white'>Is MVP Of The Match! <br> <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/main/cs2-MVP-N-RoundEnd-Music-GoldKingZ/Resources/change.gif' class=''> <br> <br> <font color='white'>Playing <font color='green'>{1}",
	"MVP.ShowCenter.Ur Final Message": "<font color='purple'>{0} <font color='white'>Is MVP Of The Match! <br> <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/main/cs2-MVP-N-RoundEnd-Music-GoldKingZ/Resources/finalmessage.gif' class=''> <br> <br> <font color='white'>Playing <font color='green'>{1}",
	"MVP.ShowCenter.GoHardHuh": "<font color='purple'>{0} <font color='white'>Is MVP Of The Match! <br> <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/main/cs2-MVP-N-RoundEnd-Music-GoldKingZ/Resources/skull1.gif' class=''> <br> <br> <font color='white'>Playing <font color='green'>{1}",
	"MVP.ShowCenter.History": "<font color='purple'>{0} <font color='white'>Is MVP Of The Match! <br> <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/main/cs2-MVP-N-RoundEnd-Music-GoldKingZ/Resources/history.gif' class=''> <br> <br> <font color='white'>Playing <font color='green'>{1}",
	"MVP.ShowCenter.OT - Johnny Dang": "<font color='purple'>{0} <font color='white'>Is MVP Of The Match! <br> <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/main/cs2-MVP-N-RoundEnd-Music-GoldKingZ/Resources/johnny.gif' class=''> <br> <br> <font color='white'>Playing <font color='green'>{1}",
	"MVP.ShowCenter.A$AP - Lord Pretty Flacko": "<font color='purple'>{0} <font color='white'>Is MVP Of The Match! <br> <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/main/cs2-MVP-N-RoundEnd-Music-GoldKingZ/Resources/lordprettyflacko.gif' class=''> <br> <br> <font color='white'>Playing <font color='green'>{1}",
	"MVP.ShowCenter.Tommy - Million Dollar Baby": "<font color='purple'>{0} <font color='white'>Is MVP Of The Match! <br> <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/main/cs2-MVP-N-RoundEnd-Music-GoldKingZ/Resources/million.gif' class=''> <br> <br> <font color='white'>Playing <font color='green'>{1}",
	"MVP.ShowCenter.Xavier Wulf - Psycho Pass": "<font color='purple'>{0} <font color='white'>Is MVP Of The Match! <br> <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/main/cs2-MVP-N-RoundEnd-Music-GoldKingZ/Resources/psycho.gif' class=''> <br> <br> <font color='white'>Playing <font color='green'>{1}",
	"MVP.ShowCenter.If We Being Real": "<font color='purple'>{0} <font color='white'>Is MVP Of The Match! <br> <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/main/cs2-MVP-N-RoundEnd-Music-GoldKingZ/Resources/real.gif' class=''> <br> <br> <font color='white'>Playing <font color='green'>{1}",
	"MVP.ShowCenter.Separate Ways": "<font color='purple'>{0} <font color='white'>Is MVP Of The Match! <br> <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/main/cs2-MVP-N-RoundEnd-Music-GoldKingZ/Resources/separate.gif' class=''> <br> <br> <font color='white'>Playing <font color='green'>{1}",
	"MVP.ShowCenter.My Soldiers Rage": "<font color='purple'>{0} <font color='white'>Is MVP Of The Match! <br> <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/main/cs2-MVP-N-RoundEnd-Music-GoldKingZ/Resources/soldiers.gif' class=''> <br> <br> <font color='white'>Playing <font color='green'>{1}",
	"MVP.ShowCenter.I Dont Care About You": "<font color='purple'>{0} <font color='white'>Is MVP Of The Match! <br> <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/main/cs2-MVP-N-RoundEnd-Music-GoldKingZ/Resources/skull2.gif' class=''> <br> <br> <font color='white'>Playing <font color='green'>{1}",
	"MVP.ShowCenter.Xcho - Ты и Я": "<font color='purple'>{0} <font color='white'>Is MVP Of The Match! <br> <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/main/cs2-MVP-N-RoundEnd-Music-GoldKingZ/Resources/meandyou.gif' class=''> <br> <br> <font color='white'>Playing <font color='green'>{1}",
	
	"MVP.ShowCenter.Hanumankind - Big Dawgs": "<font color='purple'>{0} <font color='white'>Is MVP Of The Match! <br> <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/main/cs2-MVP-N-RoundEnd-Music-GoldKingZ/Resources/bigdaw.gif' class=''> <br> <br> <font color='white'>Playing <font color='green'>{1}",
	"MVP.ShowCenter.Ratatatataa": "<font color='purple'>{0} <font color='white'>Is MVP Of The Match! <br> <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/main/cs2-MVP-N-RoundEnd-Music-GoldKingZ/Resources/ratata.gif' class=''> <br> <br> <font color='white'>Playing <font color='green'>{1}",
	"MVP.ShowCenter.Misha Xramovi - B экстазе": "<font color='purple'>{0} <font color='white'>Is MVP Of The Match! <br> <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/main/cs2-MVP-N-RoundEnd-Music-GoldKingZ/Resources/ecstasy.gif' class=''> <br> <br> <font color='white'>Playing <font color='green'>{1}",
	"MVP.ShowCenter_Bottom": "{0} Is MVP Of The Match! Playing {1}",
	
	
	//==========================
	//        Round End Music 
	//==========================
	//{0} = Name Of Round End Music 
	//==========================
	
	"RES.ShowChat": "{green}Gold KingZ {grey}| Now Playing {purple}{0}",
	"RES.ShowCenter": "<font color='white'>Playing <font color='green'>{0}",
	"RES.ShowCenter.Lithe - Hold Out": "<font color='white'>Playing <font color='green'>{0} <br> <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/main/cs2-MVP-N-RoundEnd-Music-GoldKingZ/Resources/holdout.gif' class=''> <br>",
	"RES.ShowCenter.What Is That Melody": "<font color='white'>Playing <font color='green'>{0} <br> <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/main/cs2-MVP-N-RoundEnd-Music-GoldKingZ/Resources/melody.gif' class=''> <br>",
	"RES.ShowCenter.Two Twelve Subwoofer": "<font color='white'>Playing <font color='green'>{0} <br> <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/main/cs2-MVP-N-RoundEnd-Music-GoldKingZ/Resources/twotwelvesubwoofer.gif' class=''> <br>",
	"RES.ShowCenter.Untitled #13 - Glwzbll": "<font color='white'>Playing <font color='green'>{0} <br> <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/main/cs2-MVP-N-RoundEnd-Music-GoldKingZ/Resources/untitled13.gif' class=''> <br>",
	"RES.ShowCenter.NXCRE & The Villains - USURPER": "<font color='white'>Playing <font color='green'>{0} <br> <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/main/cs2-MVP-N-RoundEnd-Music-GoldKingZ/Resources/usurper.gif' class=''> <br>",
	"RES.ShowCenter_Bottom": "Now Playing {0}",
	
	
	"Mode_1.MainMenu.Title": "{Magenta} MVP / RES Menu",
	"Mode_1.SubMenu.Title": "{Purple} .:[ {0} ]:.",
	
	"Mode_1.Previewable.Title": "{White}Set {Blue}{0} {White}?",
	"Mode_1.Previewable.Yes": "{Lime}Yes",
	"Mode_1.Previewable.No": "{LightRed}No",
	"Mode_1.Previewable.Preview": "{Olive}Play The Music",
	
	"Mode_1.STATUS.MVPSELECTED": "{Gold} {0}",
	"Mode_1.STATUS.MVPSELECTED.None": "{Darkred} {0}",
	"Mode_1.STATUS.MVPVOL": "{Lime} {0} %",
	"Mode_1.STATUS.MVPVOL.0": "{Darkred} Muted",
	"Mode_1.STATUS.MVPCHAT.Enabled": "{Lime} ✔",
	"Mode_1.STATUS.MVPCHAT.Disabled": "{Darkred} ✖",
	"Mode_1.STATUS.MVPCENTER.Enabled": "{Lime} ✔",
	"Mode_1.STATUS.MVPCENTER.Disabled": "{Darkred} ✖",
	"Mode_1.STATUS.MVPCENTERBOTTOM.Enabled": "{Lime} ✔",
	"Mode_1.STATUS.MVPCENTERBOTTOM.Disabled": "{Darkred} ✖",
	
	"Mode_1.STATUS.RESVOL": "{Lime} {0} %",
	"Mode_1.STATUS.RESVOL.0": "{Darkred} Muted",
	"Mode_1.STATUS.RESCHAT.Enabled": "{Lime} ✔",
	"Mode_1.STATUS.RESCHAT.Disabled": "{Darkred} ✖",
	"Mode_1.STATUS.RESCENTER.Enabled": "{Lime} ✔",
	"Mode_1.STATUS.RESCENTER.Disabled": "{Darkred} ✖",
	"Mode_1.STATUS.RESCENTERBOTTOM.Enabled": "{Lime} ✔",
	"Mode_1.STATUS.RESCENTERBOTTOM.Disabled": "{Darkred} ✖",
	
	
	"Mode_2.MainMenu.Title": "<font class='fontSize-M' color='#b74eae'> MVP / RES Menu</font>",
	"Mode_2.SubMenu.Title": "<font class='fontSize-M' color='#f809e6'> .:[ {0} ]:. </font>",
	
	"Mode_2.Previewable.Title": "<font color='white'>Set <font color='#00f0ff'>{0} <font color='white'>?",
	"Mode_2.Previewable.Yes": "<font color='#0cff00'>Yes",
	"Mode_2.Previewable.No": "<font color='#ff2d00'>No",
	"Mode_2.Previewable.Preview": "<font color='#91dd02'>Play The Music",
	
	"Mode_2.STATUS.MVPSELECTED": "<font color='gold'> {0}",
	"Mode_2.STATUS.MVPSELECTED.None": "<font color='#ff2d00'> {0}",
	"Mode_2.STATUS.MVPVOL": "<font color='#0cff00'> {0} %",
	"Mode_2.STATUS.MVPVOL.0": "<font color='#ff2d00'> Muted",
	"Mode_2.STATUS.MVPCHAT.Enabled": "<font color='#0cff00'> ✔",
	"Mode_2.STATUS.MVPCHAT.Disabled": "<font color='#ff2d00'> ✖",
	"Mode_2.STATUS.MVPCENTER.Enabled": "<font color='#0cff00'> ✔",
	"Mode_2.STATUS.MVPCENTER.Disabled": "<font color='#ff2d00'> ✖",
	"Mode_2.STATUS.MVPCENTERBOTTOM.Enabled": "<font color='#0cff00'> ✔",
	"Mode_2.STATUS.MVPCENTERBOTTOM.Disabled": "<font color='#ff2d00'> ✖",
	
	"Mode_2.STATUS.RESVOL": "<font color='#0cff00'> {0} %",
	"Mode_2.STATUS.RESVOL.0": "<font color='#ff2d00'> Muted",
	"Mode_2.STATUS.RESCHAT.Enabled": "<font color='#0cff00'> ✔",
	"Mode_2.STATUS.RESCHAT.Disabled": "<font color='#ff2d00'> ✖",
	"Mode_2.STATUS.RESCENTER.Enabled": "<font color='#0cff00'> ✔",
	"Mode_2.STATUS.RESCENTER.Disabled": "<font color='#ff2d00'> ✖",
	"Mode_2.STATUS.RESCENTERBOTTOM.Enabled": "<font color='#0cff00'> ✔",
	"Mode_2.STATUS.RESCENTERBOTTOM.Disabled": "<font color='#ff2d00'> ✖",
	
	
	"Mode_3.MainMenu.Title": "<font class='fontSize-M' color='#b74eae'> MVP / RES Menu</font>",
	"Mode_3.SubMenu.Title": "<font class='fontSize-M' color='#f809e6'> .:[ {0} ]:. </font>",
	
	"Mode_3.Previewable.Title": "<font color='white'>Set <font color='#00f0ff'>{0} <font color='white'>?",
	"Mode_3.Previewable.Yes": "<font color='#0cff00'>Yes",
	"Mode_3.Previewable.No": "<font color='#ff2d00'>No",
	"Mode_3.Previewable.Preview": "<font color='#91dd02'>Play The Music",
	
	"Mode_3.STATUS.MVPSELECTED": "<font color='gold'> {0}",
	"Mode_3.STATUS.MVPSELECTED.None": "<font color='#ff2d00'> {0}",
	"Mode_3.STATUS.MVPVOL": "<font color='#0cff00'> {0} %",
	"Mode_3.STATUS.MVPVOL.0": "<font color='#ff2d00'> Muted",
	"Mode_3.STATUS.MVPCHAT.Enabled": "<font color='#0cff00'> ✔",
	"Mode_3.STATUS.MVPCHAT.Disabled": "<font color='#ff2d00'> ✖",
	"Mode_3.STATUS.MVPCENTER.Enabled": "<font color='#0cff00'> ✔",
	"Mode_3.STATUS.MVPCENTER.Disabled": "<font color='#ff2d00'> ✖",
	"Mode_3.STATUS.MVPCENTERBOTTOM.Enabled": "<font color='#0cff00'> ✔",
	"Mode_3.STATUS.MVPCENTERBOTTOM.Disabled": "<font color='#ff2d00'> ✖",
	
	"Mode_3.STATUS.RESVOL": "<font color='#0cff00'> {0} %",
	"Mode_3.STATUS.RESVOL.0": "<font color='#ff2d00'> Muted",
	"Mode_3.STATUS.RESCHAT.Enabled": "<font color='#0cff00'> ✔",
	"Mode_3.STATUS.RESCHAT.Disabled": "<font color='#ff2d00'> ✖",
	"Mode_3.STATUS.RESCENTER.Enabled": "<font color='#0cff00'> ✔",
	"Mode_3.STATUS.RESCENTER.Disabled": "<font color='#ff2d00'> ✖",
	"Mode_3.STATUS.RESCENTERBOTTOM.Enabled": "<font color='#0cff00'> ✔",
	"Mode_3.STATUS.RESCENTERBOTTOM.Disabled": "<font color='#ff2d00'> ✖"
}

```

## .:[ Change Log ]:.
```
(1.0.0)
-Initial Release
```
