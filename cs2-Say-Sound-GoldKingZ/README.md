
## .:[ Price ]:. [(Payment Rules)](https://github.com/oqyh/cs2-Private-Plugins/blob/8040379022008134dde7d34cf08f7a611c750862/README.md?plain=1#L7)
```diff
+ PRICE 10$ + FREE Multiple Servers [Lifetime ( One Time Payment )] 
```

# [CS2] Say-Sound-GoldKingZ (1.0.4)  

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

  //Key To Active Plugin
  "KEY": "",

  //Change Check IpAdress To WebSite
  "ChangeCheckIpAdressToWebSite": "XXXXXXXXX.YYY",

//----------------------------[ ↓ Say Sound Config ↓ ]----------------------------

  //Allow Dead Players To Toggle Say Sound?
  "AllowDeadPlayersToSaySound": false,

  //Hide Default Radio Message If Toggle Say Sound By Radio?
  "HideDefaultRadioMessageAfterSaySound": true,

  //Hide Default Chat Message If Toggle Say Sound By Chat?
  "HideDefaultChatMessageAfterToggleShortCutSaySound": true,

  //Skip Cooldown For These Flags
  "ImmunityFromCooldownFlags": "@css/root,@css/admin,#css/root,#css/admin",

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

  //Close Menu After Select Emote
  "OpenMenu_CloseMenuAfterSelectItem": false;

  //Allow These Groups Only To Toggle On / Off SaySound  (Make It Empty "" To Let AnyOne)  [Example:@css/root,@css/admin,@css/vip,#css/admin,#css/vip]
  "Toggle_DisableSaySoundsFlags": "@css/root,@css/admin,@css/vip,#css/admin,#css/vip",

  //Commands In Game To Toggle On / Off SaySound
  "Toggle_DisableSaySoundsCommandsInGame": "!ss,!saysound,!saysounds",

  //Auto Remove Player Cookie Older Than X Days (Inactive Players)
  "Toggle_AutoRemovePlayerCookieOlderThanXDays": 7,

//----------------------------[ ↓ Advanced WASD Menu Mode 3 Settings ↓ ]----------------------------

  //If OpenMenu_Mode 3 Freeze Player When Menu Open
  "MenuWASD_FreezePlayerOnMenuOpen": true,

  //If OpenMenu_Mode 3 Close Player Menu On Pressing
  // ( w , a , s , d , jump , crouch , scoreboard , leftclick , rightclick , attack3)
  "MenuWASD_ExitMenuOnPressing": "jump,scoreboard,crouch,leftclick,rightclick,attack3",

//----------------------------[ ↓ MySql Connections ↓ ]----------------------------

  //MySql Settings
  "Enable_UseMySql": false,
  "MySqlHost": "MySql_Host",
  "MySqlDatabase": "MySql_Database",
  "MySqlUsername": "MySql_Username",
  "MySqlPassword": "MySql_Password",
  "MySqlPort": 3306,

  //Auto Remove Player MySql Older Than X Days (Inactive Players)
  "Toggle_AutoRemovePlayerMySqlOlderThanXDays": 7,

//----------------------------[ ↓ Debug ↓ ]----------------------------
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
	//        Menu Settings
	//==========================
	//Menu. = To Make Menu With SubMenu
	//NoMenu. = To Make Only Item Show WithOut SubMenu
	//SubMenu.Status. = Will Show + Toggle On / Off SaySound But With SubMenu
	//NoMenu.Status. = Will Show + Toggle On / Off SaySound But Without SubMenu
	//==========================
	//        Options
	//==========================
	// "Hide_It_And_ShowThisOnlyForFlags": "@css/root,@css/vip" //Only These Flags Show Menu/NoMenu OR SubMenu 
	// "Flags": "@css/root,@css/vip" //Only These Can Access The Emote
	// "Sound_Name": "Hi :D" //This Will Be {1} Used ShortCut In Lang
	// "Hook_Radio": "cheer", //Hook This Sound Into Player Radio [Example: coverme,takepoint,holdpos,regroup,followme,takingfire,go,fallback,sticktog,getinpos,stormfront,report,roger,enemyspot,needbackup,sectorclear,inposition,reportingin,getout,negative,enemydown,sorry,cheer,compliment,thanks,go_a,go_b,needrop,deathcry]
	// "Toggle_Sound_In_Chat": "hi,hello", //Toggle In Chat ShortCut By hi Or hello You Can Add As Many As You Like
	// "Print_To_Chat": true, //True = Show Message || false = Dont Show Message 
	// "Give_Cooldown_After_This_InXSecs": 5, //Give Cooldown After This 5 Secs
	// "Sound_Path_1": "hi" // Using sounds/saysound/hi.vsnd Will Be Not 3d Radius || Using hi Only Will Be 3d Radius (Note: You Can Add Sound_Path_2 Sound_Path_3 For Multiple Sounds)
	//==========================

	"Menu.SaySound Settings": // (SaySound Settings) Is Then Display Menu Name
	{
		"SubMenu.Status.Sounds":{} (Sounds)  Will Toggle On / Off Say Sounds 
	},
	"Menu.(Free) SaySounds":// ((Free) SaySounds) Is Then Display Menu Name
	{
		"Hide_It_And_ShowThisOnlyForFlags": "@css/root,@css/admin,#css/root,#css/admin", //Hide `Menu.(Free) SaySounds` Only Show It To These Flags
		"SubMenu.Hi":// (Hi) Is Then Display SubMenu Name
		{
			"Hide_It_And_ShowThisOnlyForFlags": "@css/root,@css/admin,#css/root,#css/admin", //Hide `SubMenu.Hi` Only Show It To These Flags

			"Flags": "@css/root,@css/vip",
			"Sound_Name": "Hi :D",
			"Hook_Radio": "cheer",
			"Toggle_Sound_In_Chat": "hi,hello",
			"Print_To_Chat": true,
			"Give_Cooldown_After_This_InXSecs": 5,
			"Sound_Path_1": "hi"
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

	"PrintToChat.SaySound.Menu.Disabled": "{green}Gold KingZ {grey}| {darkred}Say Sound Menu Is {darkred}Disabled By The Server",
	"PrintToChat.SaySound.Menu.Player.Not.Allowed": "{green}Gold KingZ {grey}| {darkred}Say Sound Menu Is For {lime}VIPS {darkred}Only",
	"PrintToChat.Player.Not.Allowed.SaySound": "{green}Gold KingZ {grey}| You Are Not Allowed To Used This Say Sound Its For {lime}VIPS Only",
	"PrintToChat.Player.Not.Allowed.SaySound.Dead": "{green}Gold KingZ {grey}| You Are Not Allowed To Say Sound While You Are {darkred}Dead",
	"PrintToChat.Player.Not.Allowed.Toggle": "{green}Gold KingZ {grey}| You Are Not Allowed To Toggle Off/On Say Sounds Its For {lime}VIPS Only",
	"PrintToChat.Player.On.Cooldown": "{green}Gold KingZ {grey}| You Need To Wait {darkred}{0} {grey}Cooldown",
	"PrintToChat.SaySound.Enabled": "{green}Gold KingZ {grey}| Say Sound Is {lime}Enabled",
	"PrintToChat.SaySound.Disabled": "{green}Gold KingZ {grey}| Say Sound Is {darkred}Disabled",

	"PrintToChatToAll.SaySound": "{green}Gold KingZ {grey}| {purple}{0} {grey}Saying.... {yellow}{1}", //If Not Found Custom Sound Message Plugin Will Use This Message By Default

	// .:[Custom Sound Messages]:.
	//SubMenu.Hi By Removing SubMenu. And Making PrintToChatToAll.SaySound.xxx To PrintToChatToAll.SaySound.Hi Plugin Will Automatic Will Use Custom Sound Message Not PrintToChatToAll.SaySound 

	"PrintToChatToAll.SaySound.Hi": "{green}Gold KingZ {grey}| {purple}{0} {grey}: Hi :))))", //{0} = Player Name || {1} = Sound_Name
	"PrintToChatToAll.SaySound.Wake Up (Not 3d Sound)": "{green}Gold KingZ {grey}| {darkred}[ADMIN] {purple}{0} {yellow}{1}", //{0} = Player Name || {1} = Sound_Name

	// .:[Menu Settings]:.
	"Menu.Mode_1.Title.MainMenu": "{yellow}.:[ Say Sound Menu ]:.",
	"Menu.Mode_1.Title.SubMenu": "{gold} {0}",
	"Menu.Mode_1.BreakLine": "{Blue}-----------",
	"Menu.Mode_1.Numbers.Color": "{green}",
	"Menu.Mode_1.Status.Enabled": "{orange}: {lime}Enabled",
	"Menu.Mode_1.Status.Disabled": "{orange}: {red}Disabled",
	"Menu.Mode_1.SubMenu.Indicator": "",
	"Menu.Mode_1.BackToMainMenu": "{purple}!6 {grey}<- Back to Main Menu",
	"Menu.Mode_1.PreviousPage": "{yellow}!7 {grey}<- Back",
	"Menu.Mode_1.NextPage": "{yellow}!8 {grey}-> Next",
	"Menu.Mode_1.Close": "{red}!9 {grey}-> Close Menu",
	"Menu.Mode_1.MenuClosed": "{green}Gold KingZ {grey}| {red}Menu Closed",



	"Menu.Mode_2.Title.MainMenu": "<font class='fontSize-M' color='yellow'> .:[ Say Sound Menu ]:. </font>",
	"Menu.Mode_2.Title.SubMenu": "<font class='fontSize-M' color='gold'> {0} </font>",
	"Menu.Mode_2.Numbers.Color": "green",
	"Menu.Mode_2.Status.Enabled": " <font color='orange'>:</font> <font color='lime'> Enabled </font>",
	"Menu.Mode_2.Status.Disabled": " <font color='orange'>:</font> <font color='red'> Disabled </font>",
	"Menu.Mode_2.SubMenu.Indicator": "",
	"Menu.Mode_2.BackToMainMenu": "<font color='purple'>!6</font> &#60;- Back to Main Menu",
	"Menu.Mode_2.PreviousPage": "<font color='yellow'>!7</font> &#60;- Back",
	"Menu.Mode_2.NextPage": "<font color='yellow'>!8</font> -> Next",
	"Menu.Mode_2.Close": "<font color='red'>!9</font> -> Close Menu",


	"Menu.Mode_3.Title.MainMenu": "<font class='fontSize-M' color='yellow'> .:[ Say Sound Menu ]:. </font>",
	"Menu.Mode_3.Title.SubMenu": "<font class='fontSize-M' color='Gold'> {0} </font>",
	"Menu.Mode_3.Highlighted_Line.Color": "orange",
	"Menu.Mode_3.NOT_Highlighted_Line.Color": "white",
	"Menu.Mode_3.Highlighted_Line.LeftSide": "<font class='fontSize-L' color='darkred'> ►[ </font>",
	"Menu.Mode_3.Highlighted_Line.RightSide": "<font class='fontSize-L' color='darkred'> ]◄ </font>",
	"Menu.Mode_3.Highlighted_Line.SubMenu.Indicator": "",
	"Menu.Mode_3.Status.Enabled": " <font color='orange'>:</font> <font color='lime'> Enabled </font>",
	"Menu.Mode_3.Status.Disabled": " <font color='orange'>:</font> <font color='red'> Disabled </font>",
	"Menu.Mode_3.SubMenu.Indicator": "",
	"Menu.Mode_3.MoreItemsBlow.Indicator": "<img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/refs/heads/main/Resources/arrow.gif' class=''> <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/refs/heads/main/Resources/arrow.gif' class=''> <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/refs/heads/main/Resources/arrow.gif' class=''>",
	"Menu.Mode_3.Bottom.Info": "<font color='cyan'>[ WASD - To Native ]</font> <br><font color='purple'>[ <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/refs/heads/main/Resources/tab.gif' class=''> - To Exit ]<br>"
}
```

## .:[ Change Log ]:.
```
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
