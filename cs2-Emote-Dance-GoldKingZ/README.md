
## .:[ Price ]:. [(Free Private Rules)](https://github.com/oqyh/cs2-Private-Plugins/blob/11b92dc04067753a390d796dbba39d789f270aab/README.md?plain=1#L27)
```diff
+ PRICE FREE [Only Discord Members] 
```

# [CS2] Emote-Dance-GoldKingZ (1.0.1)  

### Fortnite Dance Emote Animation 


![EmotePlugin](https://github.com/user-attachments/assets/1d8bcb3b-6eb4-4f87-ae18-b3c31cad9e56)

![mode1](https://github.com/user-attachments/assets/16972642-cdbb-4ffd-8ce0-4c57efd1341d)
![mode2](https://github.com/user-attachments/assets/cbb7f77d-143d-4302-91c8-b0c9458c14ae)


## .:[ Dependencies ]:.
[Metamod:Source (2.x)](https://www.sourcemm.net/downloads.php/?branch=master)

[MultiAddonManager](https://github.com/Source2ZE/MultiAddonManager)

[CounterStrikeSharp](https://github.com/roflmuffin/CounterStrikeSharp/releases)

[Newtonsoft.Json](https://www.nuget.org/packages/Newtonsoft.Json)

[MySqlConnector](https://www.nuget.org/packages/MySqlConnector)

## .:[ Configuration ]:.

> [!CAUTION]
> Config Located In ..\addons\counterstrikesharp\plugins\Emote-Dance-GoldKingZ\config\config.json                                         

```json

{

  //Key To Active Plugin
  "KEY": "",

  //Change Check IpAdress To WebSite
  "ChangeCheckIpAdressToWebSite": "XXXXXXXXX.YYY",

//----------------------------[ ↓ Emote Dance Config ↓ ]----------------------------

  //Emote View?
  //true = ThirdPerson View
  //false = FirstPerson View
  "Emote_Thirdperson_View": true,

  //Freeze If Player Emote?
  "Emote_Freeze": true,

  //Check If Player Was Freezed Before Giving (Emote_Freeze OR MenuWASD_FreezePlayerOnMenuOpen) And Dont Unfreeze Him?
  //true = Yes
  //false = No Dont Check
  "Emote_AutoDetectIfPlayerWasFreezedDontUnFreezeHim": true,

  //Cancel Emote If Player Get Damaged
  "Emote_CancelAnimationIfGettingDamaged": true,

  //Hide Default Chat Message If Toggle Emote By Chat?
  "Emote_HideDefaultChatMessageAfterToggleShortCut": true,

  //Skip Cooldown For These Flags
  "Emote_ImmunityFromCooldownFlags": "@css/root,@css/admin,#css/root,#css/admin",

  //Cancel Player Emote On Pressing
  //( w , a , s , d , jump , crouch , scoreboard , leftclick , rightclick , attack3)
  "Emote_CancelPlayersAnimationOnPressing": "w,s,jump,crouch,leftclick",

  //Open Menu Mode:
  //0 = Disable Menu
  //1 = Custom Chat Menu By GoldKingZ
  //2 = Custom Chat Menu By GoldKingZ
  //3 = WASD Menu By GoldKingZ
  "OpenMenu_Mode": 3,

  //Allow These Groups Only To Open Emote Menu (Make It Empty "" To Let AnyOne)  [Example:@css/root,@css/admin,@css/vip,#css/admin,#css/vip]
  "OpenMenu_Flags": "",

  //Commands In Game To Open Emote Menu
  "OpenMenu_CommandsInGame": "!emotes,!emote,!dances,!dance",

  //Close Menu After Select Emote
  "OpenMenu_CloseMenuAfterSelectItem": false,

//----------------------------[ ↓ Advanced WASD Menu Mode 3 Settings ↓ ]----------------------------

  //If OpenMenu_Mode 3 Freeze Player When Menu Open
  "MenuWASD_FreezePlayerOnMenuOpen": true,
  
  //Do You Want Emote_CancelPlayersAnimationOnPressing Works While Player On WASD Menu
  "Emote_DoCancelPlayersAnimationWhileMenuWASDIsOn": false,
  
  //If OpenMenu_Mode 3 Close Player Menu On Pressing
  //(jump , crouch , scoreboard , leftclick , rightclick , attack3)
  "MenuWASD_ExitMenuOnPressing": "jump,scoreboard,crouch",

//----------------------------[ ↓ Debug ↓ ]----------------------------

  //Enable Debug Will Print Server Console If You Face Any Issue
  "EnableDebug": false,
}

```


## .:[ Configuration Emote ]:.

> [!CAUTION]
> Emote Config Located In ..\addons\counterstrikesharp\plugins\Emote-Dance-GoldKingZ\config\Emote_Settings.json                                       
```json

//==========================
//        Options
//==========================
// "Hide_It_And_ShowThisOnlyForFlags": "@css/root,@css/vip" //Only These Flags Show Menu/NoMenu OR SubMenu 
// "Flags": "@css/root,@css/vip" //Only These Can Access The Emote
// "ModelAnimation": "models/goldkingz/emote/goldkingz_emotes.vmdl" //Model That Has Animation
// "RandomAnimationName_X": "Emote_RockPaperScissor_Paper" //Name Of The Animations Add As Many As You Like Change X to Numbers It Will Pick One Random If Dont Have Make It Empty Or Dont Use It
// "AnimationName": "Emote_EasternBloc_Start" //Name Of The Animation
// "AnimationName2": "Emote_EasternBloc" //If Yo Have Continuous Animation Added Here Will Be Looped If Dont Have Make It Empty Or Dont Use It
// "AnimationName2EnterByTimerInXSecs": 89 //Time In Secs To Exit From AnimationName And Enter AnimationName2 If AnimationName2 Used
// "AnimationName2EnterByFrames": 89 //By Frames To Exit From AnimationName And Enter AnimationName2 If AnimationName2 Used
// "MusicEmote": "Emote_EasternBloc" //Music Name If Dont Have Make It Empty Or Dont Use It
// "EmoteName": "Eastern Bloc" //Name Of The Emote To Use In Lang
// "Toggle_Emote_In_Chat": "Bloc,EasternBloc" //Toggle Emote In Chat Add As Many As You Like
// "LoopAnimation": true //Loop Emote?
// "PrintChatToAll": true //Print To Chat All Players In The Server?
// "PrintChatToPlayer": false //Print To Chat Locally To The Player Only?
// "If_LoopAnimation_False_KillAnimationByTimerInXSecs": 78 //If LoopAnimation false Kill Animation After Time In Secs 
// "If_LoopAnimation_False_KillAnimationByFrames": 78 //if LoopAnimation false Kill Animation By End Of Frames
// "If_LoopAnimation_True_RepeatMusicEmoteOnEveryXSecs": 3.134694 //If LoopAnimation true Repeat Music On Every Time In Secs
// "If_LoopAnimation_True_RepeatMusicEmoteAfterXFrames": 3.134694 //If LoopAnimation true Repeat Music On End Of Frames
// "Give_Cooldown_After_This_InXSecs": 25, //Give Cooldown After This 25 Secs
//==========================

{
	"Menu. Dances": //After Menu. Is The Name Of Menu
	{
		"SubMenu.Dance Moves 1": //After SubMenu. Is The Name Of Submenu
		{
			"ModelAnimation": "models/goldkingz/emote/goldkingz_emotes.vmdl",
			"AnimationName": "DanceMoves",
			"MusicEmote": "DanceMoves1",
			"EmoteName": "Dance Ninja",
			"Toggle_Emote_In_Chat": "dance,ninja",
			"LoopAnimation": true,
			"PrintChatToAll": true,
			"PrintChatToPlayer": false,
			"If_LoopAnimation_True_RepeatMusicEmoteAfterXFrames": 204
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

	"PrintChatToPlayer.EmoteMenu.Disabled": "{green}Gold KingZ {grey}| {darkred}Emote Menu Is {darkred}Disabled By The Server",
	"PrintChatToPlayer.EmoteMenu.Not.Allowed": "{green}Gold KingZ {grey}| {darkred}Emote Menu Is For {lime}VIPS {darkred}Only",
	"PrintChatToPlayer.Emote.Not.Allowed": "{green}Gold KingZ {grey}| {darkred}This Emote Is For {lime}VIPS {darkred}Only", //If Not Found Custom Not Allowed Message (PrintChatToPlayer.Emote.Not.Allowed.XXXXX) Plugin Will Use This Message By Default 
	"PrintChatToPlayer.Emote.Not.Allowed.Dance 8 (Admin)": "{green}Gold KingZ {grey}| {darkred}This Emote Is For {lime}ADMINS {darkred}Only", //Use Custom Not Allowed Message On (SubMenu.Dance 8 (Admin))
	"PrintChatToPlayer.Emote.While.He.Is.Dead": "{green}Gold KingZ {grey}| You cant Emote While You Dead",
	"PrintChatToPlayer.Emote.While.He.Is.OnBot": "{green}Gold KingZ {grey}| You cant Emote While You As Bot",
	"PrintChatToPlayer.Emote.While.He.Is.NotOnTheGround": "{green}Gold KingZ {grey}| You cant Emote While You On Air ",
	"PrintChatToPlayer.Emote.While.He.Is.OnCooldown": "{green}Gold KingZ {grey}| You On Cooldown Please Wait {yellow}{0} Secs",

	//==========================
	//     Emote Messages
	//==========================
	//PrintChatToPlayer = Print To Chat Locally To The Player Only (If PrintChatToPlayer True In Emote_Settings.json)
	//PrintChatToAll = Print To Chat All Players In The Server (If PrintChatToAll True In Emote_Settings.json)
	//{0} = Player Name
	//{1} = EmoteName
	//==========================

	"PrintChatToPlayer.Emote": "{green}Gold KingZ {grey}| You Played Emote {yellow}{1}",//If Not Found Custom Message (PrintChatToPlayer.Emote.XXXXX) Plugin Will Use This Message By Default
	"PrintChatToAll.Emote": "{green}Gold KingZ {grey}| {purple}{0} {grey}Played Emote {yellow}{1}",//If Not Found Custom Message (PrintChatToAll.Emote.XXXXX) Plugin Will Use This Message By Default

	// .:[Custom Emote Messages]:.
	"PrintChatToAll.Emote.Dance 1 (Vip)": "{green}Gold KingZ {grey}| {blue}[VIP] {purple}{0} {grey}Played Emote {yellow}{1}", //Use Custom Message On (SubMenu.Dance 1 (Vip))
	"PrintChatToAll.Emote.Dance 8 (Admin)": "{green}Gold KingZ {grey}| {darkred}[ADMIN] {purple}{0} {grey}Played Emote {yellow}{1}", //Use Custom Message On (SubMenu.Dance 8 (Admin))


	// .:[Menu Settings]:.
	"Menu.Mode_1.Title.MainMenu": "{yellow}.:[ Emote Menu ]:.",
	"Menu.Mode_1.Title.SubMenu": "{gold} {0}",
	"Menu.Mode_1.BreakLine": "{Blue}-----------",
	"Menu.Mode_1.Numbers.Color": "{green}",
	"Menu.Mode_1.SubMenu.Indicator": "",
	"Menu.Mode_1.BackToMainMenu": "{purple}!6 {grey}<- Back to Main Menu",
	"Menu.Mode_1.PreviousPage": "{yellow}!7 {grey}<- Back",
	"Menu.Mode_1.NextPage": "{yellow}!8 {grey}-> Next",
	"Menu.Mode_1.Close": "{red}!9 {grey}-> Close Menu",
	"Menu.Mode_1.MenuClosed": "{green}Gold KingZ {grey}| {red}Menu Closed",



	"Menu.Mode_2.Title.MainMenu": "<font class='fontSize-M' color='yellow'> .:[ Emote Menu ]:. </font>",
	"Menu.Mode_2.Title.SubMenu": "<font class='fontSize-M' color='gold'> {0} </font>",
	"Menu.Mode_2.Numbers.Color": "green",
	"Menu.Mode_2.SubMenu.Indicator": "",
	"Menu.Mode_2.BackToMainMenu": "<font color='purple'>!6</font> &#60;- Back to Main Menu",
	"Menu.Mode_2.PreviousPage": "<font color='yellow'>!7</font> &#60;- Back",
	"Menu.Mode_2.NextPage": "<font color='yellow'>!8</font> -> Next",
	"Menu.Mode_2.Close": "<font color='red'>!9</font> -> Close Menu",


	"Menu.Mode_3.Title.MainMenu": "<font class='fontSize-M' color='yellow'> .:[ Emote Menu ]:. </font>",
	"Menu.Mode_3.Title.SubMenu": "<font class='fontSize-M' color='Gold'> {0} </font>",
	"Menu.Mode_3.Highlighted_Line.Color": "orange",
	"Menu.Mode_3.NOT_Highlighted_Line.Color": "white",
	"Menu.Mode_3.Highlighted_Line.LeftSide": "<font class='fontSize-L' color='darkred'> ►[ </font>",
	"Menu.Mode_3.Highlighted_Line.RightSide": "<font class='fontSize-L' color='darkred'> ]◄ </font>",
	"Menu.Mode_3.Highlighted_Line.SubMenu.Indicator": "",
	"Menu.Mode_3.SubMenu.Indicator": "",
	"Menu.Mode_3.MoreItemsBlow.Indicator": "<img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/refs/heads/main/Resources/arrow.gif' class=''> <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/refs/heads/main/Resources/arrow.gif' class=''> <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/refs/heads/main/Resources/arrow.gif' class=''>",
	"Menu.Mode_3.Bottom.Info": "<font color='cyan'>[ WASD - To Native ]</font> <br><font color='purple'>[ <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/refs/heads/main/Resources/tab.gif' class=''> - To Exit ]<br>"
}
```

## .:[ Change Log ]:.
```
(1.0.1)

[Fix]
- Some Bugs
- Bug OpenMenu_CloseMenuAfterSelectItem Dont Stop Animation If It True
- Bug Camera Bug After Death
- Workshop No Sound (Workshop Updated)
- Emote While On Air Now Emote Will Auto Cancel If Player Not On The Ground
- OpenMenu_Mode 3 WASD Menu+SubMenu Or NoMenu By Gold KingZ
- Players Emote/Dance No Longer Damage By Molly Or Nade
- Emote_DoCancelPlayersAnimationWhileMenuWASDIsOn Bug

[Added In config.json]
- ChangeCheckIpAdressToWebSite
- Emote_AutoDetectIfPlayerWasFreezedDontUnFreezeHim
- Emote_HideDefaultChatMessageAfterToggleShortCut
- Emote_CancelAnimationIfGettingDamaged
- Emote_ImmunityFromCooldownFlags
- OpenMenu_Mode 1 Chat Menu+SubMenu Or NoMenu By Gold KingZ 
- OpenMenu_Mode 2 Center Menu+SubMenu Or NoMenu By Gold KingZ
- Emote_CancelPlayersAnimationOnPressing (scoreboard,leftclick,rightclick,attack3)

[Added In Emote_Settings.json]
- Give_Cooldown_After_This_InXSecs Per Emote
- Hide_It_And_ShowThisOnlyForFlags 
- PrintChatToAll true / false (Off/On) + Auto Detect Custom Messages If Applied In Lang By PrintChatToAll.Emote.XXXXX (XXXXX Is After SubMenu. OR NoMenu.)
- PrintChatToPlayer true / false (Off/On) + Auto Detect Custom Messages If Applied In Lang By PrintChatToPlayer.Emote.XXXXX (XXXXX Is After SubMenu. OR NoMenu.)

[Added In Lang]
- Lang PrintChatToPlayer.Emote.While.He.Is.NotOnTheGround
- Auto Detect Custom Message Abilty For (PrintChatToPlayer.Emote.Not.Allowed) Linked To Emote_Settings.json 
- Auto Detect Custom Message Abilty For (PrintChatToPlayer.Emote) Linked To Emote_Settings.json 
- Auto Detect Custom Message Abilty For (PrintChatToAll.Emote) Linked To Emote_Settings.json 

[Removed In config.json]
- Emote_CooldownInXSecs

[Modification]
- Rework Lang (PrintChatToPlayer / PrintChatToAll)
- Menu Mode 1 2 3 Can Be Modify In Lang

(1.0.0)

-Initial Release
```
