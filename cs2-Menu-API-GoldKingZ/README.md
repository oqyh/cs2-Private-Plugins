
## .:[ Price ]:. [(Free Private Rules)](https://github.com/oqyh/cs2-Private-Plugins/blob/11b92dc04067753a390d796dbba39d789f270aab/README.md?plain=1#L27)
```diff
+ PRICE FREE [Only Discord Members] +Its Only Included With GKZ Plugins
```

# [CS2] Menu-API-GoldKingZ (1.0.0)  


### Custom Menu Api

![menuapi](https://github.com/user-attachments/assets/703e9007-0b2d-4cc3-ab5d-a01c03d18906)


## .:[ Dependencies ]:.

[Metamod:Source (2.x)](https://www.sourcemm.net/downloads.php/?branch=master)

[CounterStrikeSharp](https://github.com/roflmuffin/CounterStrikeSharp/releases)

## .:[ Configuration ]:.

> [!CAUTION]
> Config Located In ..\addons\counterstrikesharp\plugins\XXXXXXXXXXX\MenuApiGoldKingZ\MenuConfig.json                                        

```json

{

	//----------------------------[ ↓ Chat Menu Config ↓ ]----------------------------
	
	//Break Line
	"Chat_BreakLine": "{BlueGrey}----------------------",
	
	//Previous Page
	"Chat_PrevPage": "{yellow}!7 {grey}<- Back",
	
	//Next Page
	"Chat_NextPage": "{yellow}!8 {grey}-> Next",
	
	//Close Menu
	"Chat_CloseMenu": "{red}!9 {grey}-> Close Menu",
	
	//If There Is Sub Menu String Will Indicate
	"Chat_SubMenuIndicator": "",
	
	//Enabled Color Numbers
	"Chat_EnabledNumbersColor": "{green}",
	
	//Disabled Color Numbers
	"Chat_DisabledNumbersColor": "{grey}",
	
	//----------------------------[ ↓ Center Menu Config ↓ ]----------------------------
	
	//Previous Page
	"Center_PrevPage": "<font color='yellow'>!7</font> <font color='grey'>&#60;- Back</font>",
	
	//Next Page
	"Center_NextPage": "<font color='yellow'>!8</font> <font color='grey'>-> Next</font>",
	
	//Close Menu
	"Center_CloseMenu": "<font color='red'>!9</font> <font color='grey'>-> Close Menu</font>",
	
	//If There Is Sub Menu String Will Indicate
	"Center_SubMenuIndicator": "",
	
	//Enabled Color Numbers
	"Center_EnabledNumbersColor": "green",
	
	//Disabled Color Numbers
	"Center_DisabledNumbersColor": "grey",
	
	//----------------------------[ ↓ Center WASD Menu Config ↓ ]----------------------------
	
	//Freeze When Player Open Menu
	"WASD_FreezePlayerOnMenuOpen": true,
	
	//Detect If Player Was Freezed Dont UnFreeze Him
	"WASD_AutoDetectIfPlayerWasFreezedDontUnFreezeHim": true,
	
	//Keys Available
	//(jump): When Player Jumps
	//(attack3): attack3
	//(walk): When Walk
	//(scoreboard,tab): When Player Open Scoreboard
	//(crouch,duck): When Player Duck
	//(leftclick,attack): When Player Left Click/attack
	//(rightclick,attack2): When Player Right Click/attack2
	//(w,moveforward): When Player Move Forward
	//(s,movebackward): When Player Move Backward
	//(d,moveright): When Player Move Right Side
	//(a,moveleft): When Player Move Left Side
	//(sprint,speed): When Player Speed
	
	//Scroll Down Menu
	"WASD_ScrollDownMenuOnPressing": "movebackward",
	
	//Scroll Up Menu
	"WASD_ScrollUpMenuOnPressing": "moveforward",
	
	//Previous Page
	"WASD_PrevPageMenuOnPressing": "moveleft",
	
	//Enter Page / Select
	"WASD_SelectMenuOnPressing": "moveright",
	
	//Exit Menu
	"WASD_ExitMenuOnPressing": "leftclick,rightclick,jump,scoreboard,crouch",
	
	//Highlighted Line Color
	"WASD_HighlightedLineColor": "orange",
	
	//Not Highlighted Line Color
	"WASD_Not_HighlightedLineColor": "white",
	
	//Highlighted Line Left Side 
	"WASD_HighlightedLine_LeftSide": "<font class='fontSize-L' color='darkred'> ►[ </font>",
	
	//Highlighted Line Right Side 
	"WASD_HighlightedLine_RightSide": "<font class='fontSize-L' color='darkred'> ]◄ </font>",
	
	//Highlighted Line If There Is Sub Menu String Will Indicate
	"WASD_HighlightedLine_SubMenuIndicator": "",
	
	//Not Highlighted Line If There Is Sub Menu String Will Indicate
	"WASD_Not_HighlightedLine_SubMenuIndicator": "",
	
	//If There Is More Menus Down String Will Indicate
	"WASD_MoreItemsBlow_Indicator": "<img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/refs/heads/main/Resources/arrow.gif' class=''> <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/refs/heads/main/Resources/arrow.gif' class=''> <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/refs/heads/main/Resources/arrow.gif' class=''>",
	
	//Bottom Info
	"WASD_Bottom_Info": "<font color='cyan'>[ WASD - To Native ]</font> <br><font color='purple'>[ <img src='https://raw.githubusercontent.com/oqyh/cs2-Private-Plugins/refs/heads/main/Resources/tab.gif' class=''> - To Exit ]<br>"

}

```


## .:[ Change Log ]:.
```
(1.0.0)
-Initial Release
```
