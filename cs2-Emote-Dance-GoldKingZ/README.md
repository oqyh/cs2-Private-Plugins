
## .:[ Price ]:. [(Free Private Rules)](https://github.com/oqyh/cs2-Private-Plugins/blob/11b92dc04067753a390d796dbba39d789f270aab/README.md?plain=1#L27)
```diff
+ PRICE FREE [Only Discord Members] 
```

# [CS2] Emote-Dance-GoldKingZ (1.0.2)  

### Fortnite Dance Emote Animation 


![EmotePlugin](https://github.com/user-attachments/assets/1d8bcb3b-6eb4-4f87-ae18-b3c31cad9e56)

![mode1](https://github.com/user-attachments/assets/16972642-cdbb-4ffd-8ce0-4c57efd1341d)
![mode2](https://github.com/user-attachments/assets/cbb7f77d-143d-4302-91c8-b0c9458c14ae)


## .:[ Dependencies ]:.
[Metamod:Source (2.x)](https://www.sourcemm.net/downloads.php/?branch=master)

[MultiAddonManager](https://github.com/Source2ZE/MultiAddonManager)

[CounterStrikeSharp](https://github.com/roflmuffin/CounterStrikeSharp/releases)

[Newtonsoft.Json](https://www.nuget.org/packages/Newtonsoft.Json)


## .:[ Configuration ]:.

> [!CAUTION]
> Config Located In ..\addons\counterstrikesharp\plugins\Emote-Dance-GoldKingZ\config\config.json                                         

```json

{
//----------------------------[ ↓ Main Config ↓ ]----------------------------

  //Open Menu Mode:
  //0 = Disable Menu
  //1 = Custom Chat Menu By GoldKingZ
  //2 = Custom Chat Menu By GoldKingZ
  //3 = WASD Menu By GoldKingZ
  "OpenMenu_Mode": 3,

  //Allow These Groups Only To Open Emote (Make It Empty "" To Let AnyOne)  [Example:@css/root,@css/admin,@css/vip,#css/admin,#css/vip]
  "OpenMenu_Flags": "",

  //Commands In Game To Open Emote Menu
  "OpenMenu_CommandsInGame": "!emotes,!emote,!dances,!dance",

  //Allow These Groups Only To Reload Json
  "Reload_Json_Flags": "@css/root,@css/admin,#css/root,#css/admin",

  //Commands In Game To Reload Json
  "Reload_Json_CommandsInGame": "!reloademote,!reloaddance",

//----------------------------[ ↓ Emote/Dance Config ↓ ]----------------------------

  //Emote View?
  //true = ThirdPerson View
  //false = FirstPerson View
  "Emote_Thirdperson_View": true,

  //Freeze If Player Emote?
  "Emote_FreezePlayerWhenEmote": true,

  //Check If Player Was Freezed Before Giving (Emote_FreezePlayerWhenEmote) And Dont Unfreeze Him?
  //true = Yes
  //false = No Dont Check
  "Emote_AutoDetectIfPlayerWasFreezedDontUnFreezeHim": true,

  //Cancel Emote If Player Get Damaged
  "Emote_CancelAnimationIfGettingDamaged": true,

  //Hide Default Chat Message If Toggle Emote By Chat?
  "Emote_HideDefaultChatMessageAfterToggleShortCut": true,

  //Do You Want Emote_CancelPlayersAnimationOnPressing Works While Player On WASD Menu
  "Emote_DoCancelPlayersAnimationWhileMenuWASDIsOn": false,

  //Cancel Player Emote On Pressing
  //(jump,space): When Player Jumps/Space
  //(attack3): attack3
  //(walk,shift): When Walk
  //(scoreboard,tab): When Player Open Scoreboard
  //(crouch,duck): When Player Duck
  //(leftclick,attack): When Player Left Click/attack
  //(rightclick,attack2): When Player Right Click/attack2
  //(w,moveforward): When Player Move Forward
  //(s,movebackward): When Player Move Backward
  //(d,moveright): When Player Move Right Side
  //(a,moveleft): When Player Move Left Side
  //(inspect): When Player inspect Weapon
  //(reload,r): When Player Reload
  //(use,e): When Player +Use
  "Emote_CancelPlayersAnimationOnPressing": "walk,moveforward,movebackward,moveright,moveleft,jump,crouch,leftclick",

  //Skip Cooldown For These Flags
  "Emote_ImmunityFromCooldownFlags": "@css/root,@css/admin,#css/root,#css/admin",

//----------------------------[ ↓ Utilities ↓ ]----------------------------

  //Auto Update Signatures
  "AutoUpdateSignatures": true,

  //Enable Debug Will Print Server Console If You Face Any Issue
  "EnableDebug": false
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
// "Only_These_Flags_Can_Access_It": "@css/root,@css/vip" //Only These Can Access The Emote
// "ModelAnimation": "models/goldkingz/emote/goldkingz_emotes.vmdl" //Model That Has Animation
// "RandomAnimationName": ["Animation_1","Animation_2","Animation_3"], //Random Animation
// "AnimationName": "Emote_EasternBloc_Start" //Name Of The Animation
// "AnimationName2": "Emote_EasternBloc" //If Yo Have Continuous Animation Added Here Will Be Looped If Dont Have Make It Empty Or Dont Use It
// "MusicEmote": "Emote_EasternBloc" //Music Name If Dont Have Make It Empty Or Dont Use It
// "Toggle_Emote_In_Chat": "Bloc,EasternBloc" //Toggle Emote In Chat Add As Many As You Like
// "LoopAnimation": true //true = Will Loop AnimationName Or AnimationName2 If Exist  //false OR Not Used = Will Play AnimationName One Time And AnimationName2 If Exist
// "PrintChatToAll": true //true = Print To All Who Emote //false OR Not Used = Wil Be Disabled
// "PrintChatToPlayer": false //true = Print To Player Who Emote //false OR Not Used = Wil Be Disabled
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
			"Toggle_Emote_In_Chat": "dance,ninja",
			"LoopAnimation": true,
			"PrintChatToAll": true,
			"If_LoopAnimation_True_RepeatMusicEmoteAfterXFrames": 204
		}
		//..Add Many As You Like For More Submenus
	}
	//..Add Many As You Like For More Menus
}

```

![329846165-ba02c700-8e0b-4ebe-bc28-103b796c0b2e](https://github.com/oqyh/cs2-Game-Manager/assets/48490385/3df7caa9-34a7-47da-94aa-8d682f59e85d)

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
	"PrintChatToPlayer.Menu.Disabled": "{green}Gold KingZ {grey}| {darkred}Emote Menu Is {darkred}Disabled By The Server",
	"PrintChatToPlayer.Menu.Not.Allowed": "{green}Gold KingZ {grey}| {darkred}Emote Menu Is For {lime}VIPS {darkred}Only",
	"PrintChatToPlayer.Emote.While.He.Is.Dead": "{green}Gold KingZ {grey}| You Cant Emote When You Are Dead",
	"PrintChatToPlayer.Emote.While.He.Is.OnBot": "{green}Gold KingZ {grey}| You Cant Emote While You Are a Bot",
	"PrintChatToPlayer.Emote.While.He.Is.NotOnTheGround": "{green}Gold KingZ {grey}| You Cant Emote While You Are on Air",
	"PrintChatToPlayer.Emote.While.He.Is.OnCooldown": "{green}Gold KingZ {grey}| You Are On Cooldown. Please Wait {yellow}{0} Seconds.",

	//Default Message Emote On Not Allowed (If Not Found Custom Message)
	"PrintChatToPlayer.Selected.Not.Allowed": "{green}Gold KingZ {grey}| {darkred}You Dont Have Permission To Access This",

	//Custom Message For Specific Emote On Not Allowed
	"PrintChatToPlayer.Selected.Not.Allowed.Dance 1": "{green}Gold KingZ {grey}| {darkred}You Dont Have Permission To Access This {lime}VIPS Only",
	"PrintChatToPlayer.Selected.Not.Allowed.Dance 2": "{green}Gold KingZ {grey}| {darkred}You Dont Have Permission To Access This {lime}VIPS Only",
	"PrintChatToPlayer.Selected.Not.Allowed.Dance 3": "{green}Gold KingZ {grey}| {darkred}You Dont Have Permission To Access This {lime}VIPS Only",
	"PrintChatToPlayer.Selected.Not.Allowed.Dance 4": "{green}Gold KingZ {grey}| {darkred}You Dont Have Permission To Access This {lime}VIPS Only",
	"PrintChatToPlayer.Selected.Not.Allowed.Dance 5": "{green}Gold KingZ {grey}| {darkred}You Dont Have Permission To Access This {lime}VIPS Only",
	"PrintChatToPlayer.Selected.Not.Allowed.Dance 6": "{green}Gold KingZ {grey}| {darkred}You Dont Have Permission To Access This {lime}ADMINS Only",
	"PrintChatToPlayer.Selected.Not.Allowed.Dance 7": "{green}Gold KingZ {grey}| {darkred}You Dont Have Permission To Access This {lime}ADMINS Only",
	"PrintChatToPlayer.Selected.Not.Allowed.Dance 8": "{green}Gold KingZ {grey}| {darkred}You Dont Have Permission To Access This {lime}ADMINS Only",

	//Default Message On Start Emote (If Not Found Custom Message)
	"PrintChatToPlayer.Emote": "{green}Gold KingZ {grey}| You Played Emote {yellow}{0}", //{0} = Dance Name 
	"PrintChatToAll.Emote": "{green}Gold KingZ {grey}| {purple}{0} {grey}Played Emote {yellow}{1}", //{0} = Player Name || {1} = Dance Name

	//Custom Message For Specific Emote On Start Emote
	"PrintChatToAll.Emote.Dance 1": "{green}Gold KingZ {grey}| {blue}[VIP] {purple}{0} {grey}Played Emote {yellow}{1}",
	"PrintChatToAll.Emote.Dance 6": "{green}Gold KingZ {grey}| {darkred}[ADMIN] {purple}{0} {grey}Played Emote {yellow}{1}",


	//Menus Style
	"Mode_1.MainMenu.Title": "{Magenta} Emote Menu",
	"Mode_1.SubMenu.Title": "{Purple} .:[ {0} ]:.", //{0} = SubMenu Name

	"Mode_2.MainMenu.Title": "<font class='fontSize-M' color='#b74eae'> Emote Menu</font>",
	"Mode_2.SubMenu.Title": "<font class='fontSize-M' color='#f809e6'> .:[ {0} ]:. </font>", //{0} = SubMenu Name

	"Mode_3.MainMenu.Title": "<font class='fontSize-M' color='#b74eae'> Emote Menu</font>",
	"Mode_3.SubMenu.Title": "<font class='fontSize-M' color='#f809e6'> .:[ {0} ]:. </font>" //{0} = SubMenu Name
}
```

## .:[ Change Log ]:.
```
(1.0.2)
[Fix]
- Rework + Optimize Emote Plugin
- GKZ Api
- Some Bugs
- Bug Emote_CancelPlayersAnimationOnPressing Ability To Walk Emote
- Bug Aim Punching

[Added In config.json]
- GKZ MenuApi 
- Reload_Json_Flags 
- Reload_Json_CommandsInGame 
- AutoUpdateSignatures 

[Removed In config.json]
- KEY No Needed Any More
- ChangeCheckIpAdressToWebSite No Needed Any More

[Removed In Emote_Settings.json]
- Flags Changed To Only_These_Flags_Can_Access_It
- RandomAnimationName_X Changed To RandomAnimationName Add As Many As You Like
- AnimationName2EnterByFrames No Needed Any More
- AnimationName2EnterByTimerInXSecs No Needed Any More
- EmoteName No Needed Any More
- If_LoopAnimation_False_KillAnimationByFrames No Needed Any More
- If_LoopAnimation_False_KillAnimationByTimerInXSecs No Needed Any More

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
