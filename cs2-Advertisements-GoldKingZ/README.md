
## .:[ Price ]:. [(Payment Rules)](https://github.com/oqyh/cs2-Private-Plugins/blob/8040379022008134dde7d34cf08f7a611c750862/README.md?plain=1#L7)
```diff
+ PRICE 10$ + FREE Multiple Servers [Lifetime ( One Time Payment )] 
```

# [CS2] Advertisements-GoldKingZ (1.0.0)  

### Send Ads , Auto Translate , Toggle On Off Ads , Server Logo , And More

![adplugin](https://github.com/user-attachments/assets/249d6046-b8aa-4210-af32-ee988f39738d)


## .:[ Dependencies ]:.

[Metamod:Source (2.x)](https://www.sourcemm.net/downloads.php/?branch=master)

[CounterStrikeSharp](https://github.com/roflmuffin/CounterStrikeSharp/releases)

[Newtonsoft.Json](https://www.nuget.org/packages/Newtonsoft.Json)

[MySqlConnector](https://www.nuget.org/packages/MySqlConnector)

## .:[ Configuration ]:.

> [!CAUTION]
> Config Located In ..\addons\counterstrikesharp\plugins\Advertisements-GoldKingZ\config\config.json                                         

```json

{

	//Key To Active Plugin
	"KEY": "",
	
	//-----------------------------------------------------------------------------------
	
	//Enable MySql? Located In Advertisements-GoldKingZ/config/MySql_Settings.json
	"Enable_MySql": false,
	
	//Default Server Language Uses In Advertisements-GoldKingZ/lang/en.json
	"DefaultServerLanguage": "en",
	
	//Allow These Groups Only To Change Lang (Make It Empty "" To Let AnyOne)
	"ChangeLangFlags": "@css/vip,#css/vip",
	
	//Commands In Game To Change Lang
	"ChangeLangCommandsInGame": "!langs,!lang",
	
	//Allow These Groups Only To Toggle On/Off Client Side Lang (Make It Empty "" To Let AnyOne)
	"ToggleAdsFlags": "@css/vvip,#css/vvip",
	
	//Commands In Game To Toggle On/Off Client Side
	"ToggleAdsCommandsInGame": "!ad,!ads",
	
	//Auto Translate Depend Where Client From Depend Country Lang Mapping Located In Advertisements-GoldKingZ/config/Language_Settings.json
	//false = Server Owner Should Add Many Lang In Advertisements-GoldKingZ/lang/ To Let Client Change Their Ad Lang (ChangeLangCommandsInGame) If Not Found Will Go Back To DefaultServerLanguage 
	//true = Will Get DefaultServerLanguage And Auto Translate Depend (Language_Settings.json) But If Client ChangeLangCommandsInGame This Will Get Skipped And Auto Translate To What Language He Want
	"AutoTranslateDefaultServerToClientCountry": false,
	
	//Send Message Every X Mins
	"SendMessageEveryXMins": 5,
	
	//true = Send Random Messages But Not Duplicated
	//false = Send From Top To Bottom Messages Order
	"SendRandomMessages": false,
	
	//Auto Remove Player Cookie Older Than X Days (Inactive Players)
	"AutoRemovePlayerCookieOlderThanXDays": 7,
	
	//Auto Remove Player MySql Older Than X Days (Inactive Players)
	"AutoRemovePlayerMySqlOlderThanXDays": 7,
	
	//-----------------------------------------------------------------------------------
	
	//Allow These Groups Only To Wall Text (Make It Empty "" To Let AnyOne)
	"Test_WallText_Flags": "@css/vip,#css/vip",
	
	//Commands In Game To Wall Text
	"Test_WallText_CommandsInGame": "!walltext,!wt",
	
	//After Test Wall Text Remove It In X Sec
	"Test_WallText_DeleteTimeInXSec": 10,
	


	//Allow These Groups Only To Wall Logo (Make It Empty "" To Let AnyOne)
	"Test_WallLogo_Flags": "@css/vip,#css/vip",
	
	//Commands In Game To Wall Logo
	"Test_WallLogo_CommandsInGame": "!walllogo,!wl",
	
	//After Test Wall Logo Remove It In X Sec
	"Test_WallLogo_DeleteTimeInXSec": 10,
	


	//Allow These Groups Only To Player Text (Make It Empty "" To Let AnyOne)
	"Test_PlayerText_Flags": "@css/vip,#css/vip",
	
	//Commands In Game To Player Text
	"Test_PlayerText_CommandsInGame": "!playertext,!pt",
	
	//After Test Player Text Remove It In X Sec
	"Test_PlayerText_DeleteTimeInXSec": 10,
	



	//Allow These Groups Only To Player Logo (Make It Empty "" To Let AnyOne)
	"Test_PlayerLogo_Flags": "@css/vip,#css/vip",
	
	//Commands In Game To Player Logo
	"Test_PlayerLogo_CommandsInGame": "!playerlogo,!pl",
	
	//After Test Player Logo Remove It In X Sec
	"Test_PlayerLogo_DeleteTimeInXSec": 10,
	
	//-----------------------------------------------------------------------------------
	
	//Enable Debug Will Print Server Console If You Face Any Issue
	"EnableDebug": false,

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
	//{nextline}                                     = Print On Next Line
	//{SERVERIP}                                     = Print Server Ip Without Port
	//{SERVERIPANDPORT}                              = Print Server Ip With Port
	// "Mode" : 0 Or Not Used                        = Print Chat
	// 			1                        = Print Middle HTML HUD
	// 			2                        = Print Bottom HUD
	// 			3                        = Print Print ALERT HUD
	// "ShowHudMessageForXSecs"                      = Show HUD Time In Secs
	// "DontShowThisADToTheseGroups"                 = Skip Showing This Ads To These Groups
	// "ShowThisADToTheseGroupsOnly"                 = Show This Ads To These Groups Only
	//==========================
	
	"WallText.NotAllowed": "{green}Gold KingZ {grey}| {darkred}You Are Not Allowed To Use This Command. (WallText)",
	"WallText.Saved": "{green}Gold KingZ {grey}| Saved Wall Print Location Values Into {nextline} {green}Gold KingZ {grey}| {lime}../plugins/Advertisements-GoldKingZ/config/{green}WallText_Settings.json {nextline} {green}Gold KingZ {grey}|  Get Values In {lime}\"TEXT.XXX\"",
	"WallLogo.NotAllowed": "{green}Gold KingZ {grey}| {darkred}You Are Not Allowed To Use This Command. (WallLogo)",
	"WallLogo.Saved": "{green}Gold KingZ {grey}| Saved Wall Logo Location Values Into {nextline} {green}Gold KingZ {grey}| {lime}../plugins/Advertisements-GoldKingZ/config/{green}WallLogo_Settings.json {nextline} {green}Gold KingZ {grey}|  Get Values In {lime}\"LOGO.XXX\"",
	"PlayerText.NotAllowed": "{green}Gold KingZ {grey}| {darkred}You Are Not Allowed To Use This Command. (PlayerText)",
	"PlayerText.Saved": "{green}Gold KingZ {grey}| Saved Player Text Values Into {nextline} {green}Gold KingZ {grey}| {lime}../plugins/Advertisements-GoldKingZ/config/{green}PlayerText_Settings.json {nextline} {green}Gold KingZ {grey}|  Get Values In {lime}\"TEXT.XXX\"",
	"PlayerLogo.NotAllowed": "{green}Gold KingZ {grey}| {darkred}You Are Not Allowed To Use This Command. (PlayerLogo)",
	"PlayerLogo.Saved": "{green}Gold KingZ {grey}| Saved Player Logo Values Into {nextline} {green}Gold KingZ {grey}| {lime}../plugins/Advertisements-GoldKingZ/config/{green}PlayerLogo_Settings.json {nextline} {green}Gold KingZ {grey}|  Get Values In {lime}\"LOGO.XXX\"",
	"Ads.VIP": "{green}Gold KingZ {grey}| {darkred}Disabling Ads For VIPs Only",
	"Lang.VIP": "{green}Gold KingZ {grey}| {darkred}Changing Language For VIPs Only",
	"Ads.Enabled": "{green}Gold KingZ {grey}| Ads Has Been {lime}Enabled",
	"Ads.Disabled": "{green}Gold KingZ {grey}| Ads Has Been {darkred}Disabled",
	"Set.FoundLanguage": "{green}Gold KingZ {grey}| Language Set To {purple}{0} / {purple}{1} {purple}({2})",
	"Set.NotFoundLanguage": "{green}Gold KingZ {grey}| Language Not Found. Setting To Default Language: {purple}{0} / {purple}{1} {purple}({2})",
	"Set.CodeLanguage": "{green}Gold KingZ {grey}| Please Set Language Code Example: {purple}ar {grey}/ {purple}en {grey}/ {purple}ru",

	"AD.1": 
	{
		"Message" : "message 1 With No Mode {NEXTLINE} Means Will Print In Chat"
	},
	"AD.2": 
	{
		"Mode" : 0,
		"Message" : "message 2 With Mode 0 {NEXTLINE} Means Will Print In Chat"
	},
	"AD.3": 
	{
		"Mode" : 1,
		"ShowHudMessageForXSecs": 10,
		"Message" : "message 3 With Mode 1 {NEXTLINE} {Gold}Means Will Print Middle HTML HUD"
		
	},
	"AD.4": 
	{
		"Mode" : 2,
		"ShowHudMessageForXSecs": 10,
		"Message" : "message 4 With Mode 2 {NEXTLINE} Means Will Print Bottom HUD"
		
	},
	"AD.5": 
	{
		"Mode" : 3,
		"ShowHudMessageForXSecs": 10,
		"Message" : "message 5 With Mode 3 {NEXTLINE} Means Will Print ALERT HUD",
		"DontShowThisADToTheseGroups" : "@css/root,#css/root"
	},
	"AD.6": 
	{
		"Message" : "{grey}message 6 {NEXTLINE} {grey}This Message Will Show To All Except These Groups {lime}@css/root And #css/root",
		"DontShowThisADToTheseGroups" : "@css/root,#css/root"
	},
	"AD.7": 
	{
		"Message" : "{grey}message 7 {NEXTLINE} {grey}This Message Will Show Only To These Groups {lime}@css/root And #css/root",
		"ShowThisADToTheseGroupsOnly" : "@css/root,#css/root"
	}
}
```

## .:[ Change Log ]:.
```
(1.0.0)
-Initial Release
```
