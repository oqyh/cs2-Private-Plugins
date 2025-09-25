
## .:[ Price ]:. [(Free Private Rules)](https://github.com/oqyh/cs2-Private-Plugins/blob/11b92dc04067753a390d796dbba39d789f270aab/README.md?plain=1#L27)
```diff
+ PRICE FREE [Only Discord Members] 
```

# [CS2] MVP-N-RoundEnd-Music-GoldKingZ (1.0.8)  

### Custom MVP Per Player If Not Used Will Play Server Round End Custom Music If Not Found Will Play Player Original Music Kit

## 🖼️ ShowCase GIF

![mvp_showcase](https://github.com/user-attachments/assets/fafd66fe-56ed-4aab-a147-dd09f06f9699)


## ▶️ ShowCase Video


[![Watch the video](https://img.youtube.com/vi/FfsralH4H9U/maxresdefault.jpg)](https://youtu.be/hkjfmDgB7kQ)

---

## 📦 Dependencies
[![Metamod:Source](https://img.shields.io/badge/Metamod:Source-2d2d2d?logo=sourceengine)](https://www.sourcemm.net)

[![CounterStrikeSharp](https://img.shields.io/badge/CounterStrikeSharp-83358F)](https://github.com/roflmuffin/CounterStrikeSharp)

[![MultiAddonManager](https://img.shields.io/badge/MultiAddonManager-181717?logo=github&logoColor=white)](https://github.com/Source2ZE/MultiAddonManager)

[![MySQL](https://img.shields.io/badge/MySQL-4479A1?logo=mysql&logoColor=white)](https://dev.mysql.com/doc/connector-net/en/) [Included in zip]

[![JSON](https://img.shields.io/badge/JSON-000000?logo=json)](https://www.newtonsoft.com/json) [Included in zip]

---

## 📥 Installation

### Plugin Installation
1. Download the latest `MVP-N-RoundEnd-Music-GoldKingZ.x.x.x.zip` In Discord
2. Extract contents to your `csgo` directory
3. Configure settings in `MVP-N-RoundEnd-Music-GoldKingZ/config/config.json`
4. Restart your server

---

# ⚙️ Configuration

> [!IMPORTANT]
> **Main Configuration**  
> `../MVP-N-RoundEnd-Music-GoldKingZ/config/config.json`  
> **MVP Configuration**  
> `../MVP-N-RoundEnd-Music-GoldKingZ/config/mvp_config.json`  
> **Round End Music Configuration**  
> `../MVP-N-RoundEnd-Music-GoldKingZ/config/res_config.json`  

## 🛠️ `config/config.json`

<details open>
<summary><b>Main Config</b> (Click to expand 🔽)</summary>

| Property | Description | Values | Required |
|----------|-------------|--------|----------|
| `Reload_MVP_RES_CommandsInGame` | Commands to reload MVP/RES plugin | Format: `Console_Commands: cmd1,cmd2 \| Chat_Commands: cmd3,cmd4` | - |
| `Reload_MVP_RES_Flags` | Who can use reload commands | Format: `SteamIDs: id1,id2 \| Flags: @flag1 \| Groups: #group1` | `Reload_MVP_RES_CommandsInGame` |
| `Reload_MVP_RES_Hide` | Hide chat after reload command | `0`-No<br>`1`-Hide on success<br>`2`-Always hide | `Reload_MVP_RES_CommandsInGame` |
| `OpenMenu_Mode` | How to open MVP/RES menu | `0`-Disabled<br>`1`-Chat menu<br>`2`-Center menu<br>`3`-Center WASD<br>`4`-Screen Text WASD | - |
| `OpenMenu_CommandsInGame` | Commands to open menu | Format: `Console_Commands: cmd1,cmd2 \| Chat_Commands: cmd3,cmd4` | `OpenMenu_Mode` |
| `OpenMenu_Flags` | Who can open menu | Format: `SteamIDs: id1,id2 \| Flags: @flag1 \| Groups: #group1` | `OpenMenu_CommandsInGame` |
| `OpenMenu_Hide` | Hide chat after menu command | `0`-No<br>`1`-Hide on success<br>`2`-Always hide | `OpenMenu_CommandsInGame` |
| `Disable_Default_MVP_Music` | Disable default MVP music | `true`-Yes<br>`false`-No | - |
| `Custom_Music_length_InSecs` | Custom music duration in seconds | Number (default: 10) | - |
| `Enable_Custom_MVP` | Enable custom MVP sounds | `true`-Yes<br>`false`-No | - |
| `MVP_PickSoundsByOrder` | Play MVP sounds in order | `true`-Sequential<br>`false`-Random | - |
| `MVP_AvailableVolumes` | Available MVP volume levels | Comma-separated values (e.g., "0,20,40,60,80,100") | - |
| `MVP_Default_Volume` | Default MVP volume for new players | String (e.g., "100") | - |
| `MVP_Default_ShowChat` | Default chat display for new players | `true`-On<br>`false`-Off | - |
| `MVP_Default_ShowCenter` | Default center text display for new players | `true`-On<br>`false`-Off | - |
| `MVP_Default_ShowCenterBottom` | Default bottom center text display for new players | `true`-On<br>`false`-Off | - |
| `Enable_Custom_RES` | Enable custom round end sounds | `true`-Yes<br>`false`-No | - |
| `RES_PickSoundsByOrder` | Play RES sounds in order | `true`-Sequential<br>`false`-Random | - |
| `RES_AvailableVolumes` | Available RES volume levels | Comma-separated values (e.g., "0,20,40,60,80,100") | - |
| `RES_Default_Volume` | Default RES volume for new players | String (e.g., "100") | - |
| `RES_Default_ShowChat` | Default chat display for new players | `true`-On<br>`false`-Off | - |
| `RES_Default_ShowCenter` | Default center text display for new players | `true`-On<br>`false`-Off | - |
| `RES_Default_ShowCenterBottom` | Default bottom center text display for new players | `true`-On<br>`false`-Off | - |
| `Combine_MVP_RES` | Combine MVP and RES settings | `true`-Yes<br>`false`-No | - |
| `BOTH_AvailableVolumes` | Available combined volume levels | Comma-separated values (e.g., "0,20,40,60,80,100") | - |
| `BOTH_Default_Volume` | Default combined volume for new players | String (e.g., "100") | - |
| `BOTH_Default_ShowChat` | Default chat display for new players | `true`-On<br>`false`-Off | - |
| `BOTH_Default_ShowCenter` | Default center text display for new players | `true`-On<br>`false`-Off | - |
| `BOTH_Default_ShowCenterBottom` | Default bottom center text display for new players | `true`-On<br>`false`-Off | - |
| `Cookies_Enable` | Enable local data storage | `true`-Yes<br>`false`-No | - |
| `Cookies_AutoRemovePlayerOlderThanXDays` | Auto-delete inactive data | `0`-Disabled<br>`>0`-Days to keep | `Cookies_Enable` |
| `MySql_Enable` | Enable MySQL storage | `true`-Yes<br>`false`-No | - |
| `MySql_Host` | MySQL host address | IP/hostname | `MySql_Enable` |
| `MySql_Database` | Database name | String | `MySql_Enable` |
| `MySql_Username` | Database username | String | `MySql_Enable` |
| `MySql_Password` | Database password | String | `MySql_Enable` |
| `MySql_Port` | Database port | Number (default: 3306) | `MySql_Enable` |
| `MySql_AutoRemovePlayerOlderThanXDays` | Auto-delete inactive data | `0`-Disabled<br>`>0`-Days to keep | `MySql_Enable` |
| `EnableDebug` | Enable debug mode | `true`-Yes<br>`false`-No | - |
</details>

---


## 🛠️ `config/mvp_config.json`

<details open>
<summary><b>MVP Configuration</b> (Click to expand 🔽)</summary>

## 🔄 Status Indicators

| Option | Description | Condition |
|--------|-------------|-----------|
| `SubMenu.STATUS.MVPSELECTED.xxxxxxxxxxx` | Show client's current MVP selection | - |
| `SubMenu.STATUS.MVPNONSELECTED.xxxxxxxxxxx` | Allow client to set no MVP selection | - |
| `SubMenu.STATUS.MVPVOL.xxxxxxxxxxx` | Show client's current MVP volume | Requires `Combine_MVP_RES` = false |
| `SubMenu.STATUS.MVPCHAT.xxxxxxxxxxx` | Show client's MVP chat message setting | Requires `Combine_MVP_RES` = false |
| `SubMenu.STATUS.MVPCENTER.xxxxxxxxxxx` | Show client's MVP center message setting | Requires `Combine_MVP_RES` = false |
| `SubMenu.STATUS.MVPCENTERBOTTOM.xxxxxxxxxxx` | Show client's MVP center bottom message setting | Requires `Combine_MVP_RES` = false |
| `SubMenu.STATUS.RESVOL.xxxxxxxxxxx` | Show client's current RES volume | Requires `Combine_MVP_RES` = false |
| `SubMenu.STATUS.RESCHAT.xxxxxxxxxxx` | Show client's RES chat message setting | Requires `Combine_MVP_RES` = false |
| `SubMenu.STATUS.RESCENTER.xxxxxxxxxxx` | Show client's RES center message setting | Requires `Combine_MVP_RES` = false |
| `SubMenu.STATUS.RESCENTERBOTTOM.xxxxxxxxxxx` | Show client's RES center bottom message setting | Requires `Combine_MVP_RES` = false |
| `SubMenu.STATUS.BOTHVOL.xxxxxxxxxxx` | Show client's combined MVP+RES volume | Requires `Combine_MVP_RES` = true |
| `SubMenu.STATUS.BOTHCHAT.xxxxxxxxxxx` | Show client's combined chat message setting | Requires `Combine_MVP_RES` = true |
| `SubMenu.STATUS.BOTHCENTER.xxxxxxxxxxx` | Show client's combined center message setting | Requires `Combine_MVP_RES` = true |
| `SubMenu.STATUS.BOTHCENTERBOTTOM.xxxxxxxxxxx` | Show client's combined center bottom message setting | Requires `Combine_MVP_RES` = true |
| `SubMenu.STATUS.REPOSITION.xxxxxxxxxxx` | Reposition menu | Requires Menu Mode 4 |

## ⚙️ General Options

| Option | Description | Format/Values |
|--------|-------------|---------------|
| `Hide_It_And_Show_Only_ForFlags` | Hide menu and only show for specific flags | `SteamIDs: id1,id2 \| Flags: @flag1 \| Groups: #group1`<br>Empty = Everyone can see |
| `Only_These_Flags_Can_Access_It` | Restrict access | `SteamIDs: id1,id2 \| Flags: @flag1 \| Groups: #group1`<br>Empty = Everyone can access |
| `Only_These_Flags_Can_Vol.0` | Restrict volume 0 | `SteamIDs: id1,id2 \| Flags: @flag1 \| Groups: #group1`<br>Empty = Everyone can access |
| `Toggle_In_Chat` | Chat/console commands to toggle menu | `Console_Commands: cmd1,cmd2 \| Chat_Commands: cmd3,cmd4`<br>Empty = Disabled |
| `Toggle_In_Chat_Hide` | Hide chat after toggle command | `0`-No<br>`1`-Hide on success<br>`2`-Always hide |
| `Unique_Name` | Unique identifier for plugin | String (Required for MVP to work) |
| `ShowChat` | Show MVP chat message | `true`-Yes<br>`false`-No |
| `ShowCenter` | Show MVP center message | `true`-Yes<br>`false`-No |
| `ShowCenter_Bottom` | Show MVP center bottom message | `true`-Yes<br>`false`-No |

## 🔊 Sound Options

| Option | Description | Format/Values |
|--------|-------------|---------------|
| `Make_It_Previewable` | Enable music preview before selection | `true`-Yes<br>`false`-No |
| `Sound_Volume` | Sound volume percentage | `1%`-`100%` (default: 100%) |
| `Sound_Paths` | Sound file paths | `["sound1", "sound2", "sound3"]` |

</details>

---


## 🛠️ `config/res_config.json`

<details open>
<summary><b>Round End Music Configuration</b> (Click to expand 🔽)</summary>

## ⚙️ General Options

| Option | Description | Format/Values |
|--------|-------------|---------------|
| `ShowChat` | Show MVP chat message | `true`-Yes<br>`false`-No |
| `ShowCenter` | Show MVP center message | `true`-Yes<br>`false`-No |
| `ShowCenter_Bottom` | Show MVP center bottom message | `true`-Yes<br>`false`-No |

## 🔊 Sound Options

| Option | Description | Format/Values |
|--------|-------------|---------------|
| `Sound_Volume` | Sound volume percentage | `1%`-`100%` (default: 100%) |
| `Sound_Paths` | Sound file paths | `["sound1", "sound2", "sound3"]` |

</details>

---


## 📜 Changelog

<details>
<summary><b>📋 View Version History</b> (Click to expand 🔽)</summary>

### [1.0.8]
- Fix Bug On Flags Conflict On Other Plugins (Vipcore, ect...)
- Fix Bug MVP Will Stop On Dead Players When Change Camera

### [1.0.7]
- Rework + Optimize On Plugin 
- Rework On Client Volume Side Music No Need For Multiple Folders
- Rework On MVP + RES Configs Now They Are Separate Configs
- Fix Players Flags
- Fix Overlap Music On Spam Preview Music
- Rework On ReloadJson To Reload Entire Plugin
- Rework Config Added Comments Each Config
- Update Menu-API-GoldKingZ To 1.0.2
- Removed AutoUpdateSignatures
- Added Reload_MVP_RES_Hide
- Added OpenMenu_Mode 4
- Added OpenMenu_Hide
- Added Combine_MVP_RES
- Added BOTH_AvailableVolumes
- Added BOTH_Default_Volume
- Added BOTH_Default_ShowChat
- Added BOTH_Default_ShowCenter
- Added BOTH_Default_ShowCenterBottom
- Added SubMenu.STATUS.BOTHVOL.xxxxxxxxxxx
- Added SubMenu.STATUS.BOTHCHAT.xxxxxxxxxxx
- Added SubMenu.STATUS.BOTHCENTER.xxxxxxxxxxx
- Added SubMenu.STATUS.BOTHCENTERBOTTOM.xxxxxxxxxxx
- Added SubMenu.STATUS.REPOSITION.xxxxxxxxxxx

### [1.0.6]
- Fix Api Crash

### [1.0.5]
- Rework On Plugin
- Some Clean Up On Mysql
- Fix Player Not Saved Data On Disconnect 
- Fix MVP Not Set On Disconnect / Map Changed 

### [1.0.4]
- Fix GKZ Api

### [1.0.3]
- Fix Bugs
- Fix Error invoking callback
- Fix GKZ Api
- Remove Port Restricted
- Remove Key No Needed
- Remove ChangeCheckIpAdressToWebSite

### [1.0.2]
- Fix Bugs
- Fix When Enable_Custom_MVP Disabled Default MVP Not Turned Off On RES
- Fix MenuApi jump,space On Dead/Spec Players
- Fix MenuApi walk,shift
- Added MenuApi inspect
- Added MenuApi reload
- Added MenuApi +Use

### [1.0.1]
- Fix Bugs
- Fix Enable_Cookies
- Fix Enable_MySql
- Fix On Plugin Load Will Create MySql Table
- Fix Enable_Custom_MVP With Enable_MySql And Enable_Cookies
- Fix Enable_Custom_RES With Enable_MySql And Enable_Cookies
- Added AutoUpdateSignatures

### [1.0.0]
- Initial plugin release

</details>

