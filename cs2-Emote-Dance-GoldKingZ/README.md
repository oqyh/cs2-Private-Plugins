
## .:[ Price ]:. [(Free Private Rules)](https://github.com/oqyh/cs2-Private-Plugins/blob/11b92dc04067753a390d796dbba39d789f270aab/README.md?plain=1#L27)
```diff
+ PRICE FREE [Only Discord Members] 
```

# [CS2] Emote-Dance-GoldKingZ (1.0.0)  

### Fortnite Dance Emote Animation 


![EmotePlugin](https://github.com/user-attachments/assets/1d8bcb3b-6eb4-4f87-ae18-b3c31cad9e56)



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
  KEY = "";

//-----------------------------------------------------------------------------------------

  //Emote View?
  //true = ThirdPerson View
  //false = FirstPerson View
  "Emote_Thirdperson_View" = true;

  //Freeze If Player Emote?
  "Emote_Freeze" = true;

  //Give Cooldown X Secs After Emote
  "Emote_CooldownInXSecs" = 25;

  //Cancel Player Emote On Pressing
  // ( w , a , s , d , jump , crouch , scoreboard)
  "Emote_CancelPlayersAnimationOnPressing" = "w,s,jump,crouch";

  // Do You Want Emote_CancelPlayersAnimationOnPressing Works While Player On WASD Menu
  "Emote_DoCancelPlayersAnimationWhileMenuWASDIsOn" = false;

  // Emote Menu Mode
  // 1 = Chat Menu
  // 2 = Center Menu
  // 3 = WASD Menu (You Can Add Menu And SubMenu)
  "OpenMenu_Mode" = 3;

  // Allow These Groups Only To Open Emote Menu (Make It Empty "" To Let AnyOne)  [Example:@css/root,@css/admin,@css/vip,#css/admin,#css/vip]
  "OpenMenu_Flags" = "";

  //Commands In Game To Open Emote Menu
  "OpenMenu_CommandsInGame" = "!emotes,!emote,!dances,!dance";

  //Close Menu After Select Emote
  "OpenMenu_CloseMenuAfterSelectItem" = false;

//------------------------------[Advanced WASD Menu Settings Mode 3]--------------------------------------

  //If OpenMenu_Mode 3 Freeze Player When Menu Open
  "MenuWASD_FreezePlayerOnMenuOpen" = true;

  //If OpenMenu_Mode 3 Close Player Menu On Pressing
  // ( w , a , s , d , jump , crouch , scoreboard)
  "MenuWASD_ExitMenuOnPressing" = "jump,scoreboard,crouch";

//-----------------------------------------------------------------------------------------

  //Enable Debug Will Print Server Console If You Face Any Issue
	"EnableDebug": false,
}

```


## .:[ Configuration FakeRcon ]:.

> [!CAUTION]
> Emote Config Located In ..\addons\counterstrikesharp\plugins\Emote-Dance-GoldKingZ\config\Emote_Settings.json                                       
```json
//On OpenMenu_Mode 3 Only You Can Add Menu And Submenu On OpenMenu_Mode 1 or 2 Put Emote Directly

//==========================
//        Options
//==========================
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
// "If_LoopAnimation_False_KillAnimationByTimerInXSecs": 78 //If LoopAnimation false Kill Animation After Time In Secs 
// "If_LoopAnimation_False_KillAnimationByFrames": 78 //if LoopAnimation false Kill Animation By End Of Frames
// "If_LoopAnimation_True_RepeatMusicEmoteOnEveryXSecs": 3.134694 //If LoopAnimation true Repeat Music On Every Time In Secs
// "If_LoopAnimation_True_RepeatMusicEmoteAfterXFrames": 3.134694 //If LoopAnimation true Repeat Music On End Of Frames

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
	
    "PrintToClient.EmoteMenu.Disabled": "{green}Gold KingZ {grey}| {darkred}Emote Menu Is {darkred}Disabled By The Server",
    "PrintToClient.EmoteMenu.Player.Not.Allowed": "{green}Gold KingZ {grey}| {darkred}Emote Menu Is For {lime}VIPS {darkred}Only",
    "PrintToClient.Emote.Player.Not.Allowed": "{green}Gold KingZ {grey}| {darkred}This Emote Is For {lime}VIPS {darkred}Only",
    "PrintToClient.Player.Played.Emote.While.He.Is.Dead": "{green}Gold KingZ {grey}| You cant Emote While You Dead",
    "PrintToClient.Player.Played.Emote.While.He.Is.OnBot": "{green}Gold KingZ {grey}| You cant Emote While You As Bot",
    "PrintToClient.Player.Played.Emote.While.He.Is.OnCooldown": "{green}Gold KingZ {grey}| You On Cooldown Please Wait {yellow}{0} Secs", //0 = Time Remaining
    "PrintToClient.Player.Played.Emote": "{green}Gold KingZ {grey}| You Played Emote {yellow}{0}", //0 = Emote Name
    "PrintToAll.Player.Played.Emote": "{green}Gold KingZ {grey}| {purple}{0} {grey}Played Emote {yellow}{1}", //0 = Player Name  1= Emote Name

    "Menu.Title": ".:[ Emote Menu ]:.",
    "Menu.Left.Side": "",
    "Menu.Right.Side": "",
    "Menu.More.Down": "<img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/main/cs2-Emote-Dance-GoldKingZ/Resources/arrow.gif' class=''> <img src='https://raw.githubusercontent.com/oqyh/cs2-Kill-Sound-GoldKingZ/main/Resources/arrow.gif' class=''> <img src='https://raw.githubusercontent.com/oqyh/cs2-Kill-Sound-GoldKingZ/main/Resources/arrow.gif' class=''>",
    "Menu.Bottom": "           <font color='cyan'>[ WASD - To Native ]</font> <br><font color='purple'>[ <img src='https://raw.githubusercontent.com/oqyh/cs2-Kill-Sound-GoldKingZ/main/Resources/tab.gif' class=''> - To Exit ]<br>"
}
```

## .:[ Change Log ]:.
```
(1.0.0)
-Initial Release
```
