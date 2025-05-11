
## .:[ Price ]:. [(Payment Rules)](https://github.com/oqyh/cs2-Private-Plugins/blob/8040379022008134dde7d34cf08f7a611c750862/README.md?plain=1#L7)
```diff
+ PRICE 10$ + FREE Multiple Servers [Lifetime ( One Time Payment )] 
```

# [CS2] Advertisements-GoldKingZ (1.0.1)  

### Send Ads , Auto Translate , Toggle On Off Ads , Server Logo , And More

![ads](https://github.com/user-attachments/assets/9445a969-1cce-483c-baec-2256640c3d74)

---

## 📦 Dependencies
[![Metamod:Source](https://img.shields.io/badge/Metamod:Source-2d2d2d?logo=sourceengine)](https://www.sourcemm.net)

[![CounterStrikeSharp](https://img.shields.io/badge/CounterStrikeSharp-83358F)](https://github.com/roflmuffin/CounterStrikeSharp)

[![MultiAddonManager](https://img.shields.io/badge/MultiAddonManager-181717?logo=github&logoColor=white)](https://github.com/Source2ZE/MultiAddonManager) [Optional: If You Want Custom Logos]

[![MySQL](https://img.shields.io/badge/MySQL-4479A1?logo=mysql&logoColor=white)](https://dev.mysql.com/doc/connector-net/en/) [Included in zip]

[![JSON](https://img.shields.io/badge/JSON-000000?logo=json)](https://www.newtonsoft.com/json) [Included in zip]

---

## 📥 Installation

### Plugin Installation
1. Download the latest `Advertisements-GoldKingZ.x.x.x.zip` In Discord
2. Extract contents to your `csgo` directory
3. Configure settings in `Advertisements-GoldKingZ/config/config.json`
4. Restart your server

---

# ⚙️ Configuration

> [!IMPORTANT]
> **Main Configuration**  
> `../Advertisements-GoldKingZ/config/config.json`  
> **Advertisements Configuration**  
> `../Advertisements-GoldKingZ/advertisements/en.json`

## 🛠️ `config/config.json`

<details open>
<summary><b>Main Config</b> (Click to expand 🔽)</summary>

| Property | Description | Values | Required |  
|----------|-------------|--------|----------|
| `AutoTranslateToClientCountry` | Auto-translate based on client country | `true`-Yes<br>`false`-No (Manual via commands) | - |
| `SendMessageOnEvery` | Message interval | Format: `5m` (5 mins)<br>`5s` (5 secs) | - |
| `SendMessagesByOrder` | Message order | `true`-Sequential<br>`false`-Random | - |
| `PickSoundsByOrder` | Sound order | `true`-Sequential<br>`false`-Random | - |
| `RenameMaps` | Custom map names | Format: `original : new name`<br>Example: `de_dust2 : Dust 2` | - |
| `RenameGroupsAndFlags` | Custom group/flag names | Format: `Name : Flags`<br>Example: `ADMINS : @css/admins` | - |
| `Player_Logo_Path` | Player logo path | File path: `materials/...` | - |
| `Reload_Advertisements_CommandsInGame` | Reload ads commands | Example: `!reloadad`<br>`""`-Disable | - |
| `Reload_Advertisements_Flags` | Reload ads permissions | Format: Flags/SteamIDs<br>`""`-Everyone | `Reload_Advertisements_CommandsInGame` ≠ `""` |
| `Ads_Menu_CommandsInGame` | Ads menu commands | Example: `!adadmin`<br>`""`-Disable | - |
| `Ads_Menu_Flags` | Ads menu permissions | Format: Flags/SteamIDs<br>`""`-Everyone | `Ads_Menu_CommandsInGame` ≠ `""` |
| `Test_Sounds_CommandsInGame` | Test sounds commands | Example: `!play`<br>`""`-Disable | - |
| `Test_Sounds_Flags` | Test sounds permissions | Format: Flags/SteamIDs<br>`""`-Everyone | `Test_Sounds_CommandsInGame` ≠ `""` |
| `ChangeLang_CommandsInGame` | Language commands | Example: `!lang`<br>`""`-Disable | - |
| `ChangeLang_Flags` | Language permissions | Format: Flags/SteamIDs<br>`""`-Everyone | `ChangeLang_CommandsInGame` ≠ `""` |
| `Toggle_Messages_CommandsInGame` | Toggle messages commands | Example: `!ads`<br>`""`-Disable | - |
| `Toggle_Messages_Flags` | Toggle messages permissions | Format: Flags/SteamIDs<br>`""`-Everyone | `Toggle_Messages_CommandsInGame` ≠ `""` |
| `Toggle_Messages_Sounds_CommandsInGame` | Toggle sound messages commands | Example: `!ad_sound`<br>`""`-Disable | - |
| `Toggle_Messages_Sounds_Flags` | Toggle sound messages permissions | Format: Flags/SteamIDs<br>`""`-Everyone | `Toggle_Messages_Sounds_CommandsInGame` ≠ `""` |
| `Toggle_Wall_Logo_CommandsInGame` | Toggle wall logo commands | Example: `!ad_wl`<br>`""`-Disable | - |
| `Toggle_Wall_Logo_Flags` | Toggle wall logo permissions | Format: Flags/SteamIDs<br>`""`-Everyone | `Toggle_Wall_Logo_CommandsInGame` ≠ `""` |
| `Toggle_Wall_Text_CommandsInGame` | Toggle wall text commands | Example: `!ad_wt`<br>`""`-Disable | - |
| `Toggle_Wall_Text_Flags` | Toggle wall text permissions | Format: Flags/SteamIDs<br>`""`-Everyone | `Toggle_Wall_Text_CommandsInGame` ≠ `""` |
| `Toggle_Player_Logo_CommandsInGame` | Toggle player logo commands | Example: `!ad_pl`<br>`""`-Disable | - |
| `Toggle_Player_Logo_Flags` | Toggle player logo permissions | Format: Flags/SteamIDs<br>`""`-Everyone | `Toggle_Player_Logo_CommandsInGame` ≠ `""` |
| `Ads_Default_Messages` | Default message state | `true`-On<br>`false`-Off | - |
| `Ads_Default_Messages_Sounds` | Default sound messages | `true`-On<br>`false`-Off | - |
| `Ads_Default_Wall_Logo` | Default wall logo | `true`-On<br>`false`-Off | - |
| `Ads_Default_Wall_Text` | Default wall text | `true`-On<br>`false`-Off | - |
| `Ads_Default_Player_Logo` | Default player logo | `true`-On<br>`false`-Off | - |
| `Cookies_Enable` | Local cookie storage | `true`-Yes<br>`false`-No | - |
| `Cookies_AutoRemovePlayerOlderThanXDays` | Auto-delete inactive cookies | `0`-Disable<br>`7`-7 days | `Cookies_Enable` = `true` |
| `MySql_Enable` | MySQL storage | `true`-Yes<br>`false`-No | - |
| `MySql_Host` | MySQL host | IP/Hostname | `MySql_Enable` = `true` |
| `MySql_Database` | MySQL database | Database name | `MySql_Enable` = `true` |
| `MySql_Username` | MySQL username | Database user | `MySql_Enable` = `true` |
| `MySql_Password` | MySQL password | Database password | `MySql_Enable` = `true` |
| `MySql_Port` | MySQL port | Default: `3306` | `MySql_Enable` = `true` |
| `MySql_AutoRemovePlayerOlderThanXDays` | Auto-delete MySQL data | `0`-Disable<br>`7`-7 days | `MySql_Enable` = `true` |

</details>

<details>
<summary><b>Utilities Config</b> (Click to expand 🔽)</summary>

| Property | Description | Values | Required |  
|----------|-------------|--------|----------|
| `AutoUpdateSignatures` | Auto-Update Signatures | `true`-Yes<br>`false`-No | - |
| `EnableDebug` | Debug Mode | `true`-Enable<br>`false`-Disable | - |

</details>

---


## 🛠️ `advertisements/en.json`

<details open>
<summary><b>Message Configuration</b> (Click to expand 🔽)</summary>

### **Colors**  
| Color Tag | Example |
|-----------|---------|
| `{Yellow}` | `{Yellow}Warning Message` |
| `{Gold}` | `{Gold}[VIP] Player` |
| `{Silver}` | `{Silver}Regular Member` |
| `{Blue}` | `{Blue}Information` |
| `{DarkBlue}` | `{DarkBlue}Moderator Tag` |
| `{BlueGrey}` | `{BlueGrey}System Alert` |
| `{Magenta}` | `{Magenta}Event Notification` |
| `{LightRed}` | `{LightRed}Urgent Alert` |
| `{LightBlue}` | `{LightBlue}Server Note` |
| `{Olive}` | `{Olive}Team Chat` |
| `{Lime}` | `{Lime}Success Message` |
| `{Red}` | `{Red}Error!` |
| `{Purple}` | `{Purple}Admin Command` |
| `{Grey}` | `{Grey}12:00:00` |
| `{Default}` | `{Default}Normal Text` |
| `{White}` | `{White}Notification` |
| `{Darkred}` | `{Darkred}Banned!` |
| `{Green}` | `{Green}Connected` |
| `{LightYellow}` | `{LightYellow}Hint Text` |

### **Format**  
| Key | Description | Values/Examples |
|-----|-------------|-----------------|
| `"Welcome"` | Initial connection message | Remove to disable |
| `"OnDeath"` | Death message | Remove to disable |
| `"Message"` | Content container | `"Hello {PLAYER_NAME}!"` |
| `"Show_Mode"` | Display location | `not used`=Chat<br>`0`=Chat<br>`1`=Chat<br>`2`=Console<br>`3`=Center HTML Adding "3:10" Is The Duration In Secs<br>`4`=Bottom center Adding "4:10" Is The Duration In Secs<br>`5`=Alert box Adding "5:10" Is The Duration In Secs<br>`6`=Custom Screen Adding "6:10" Is The Duration In Secs|
| `"Delay_Welcome_InXSecs"` | Welcome message delay | `5` = 5 seconds |
| `"Sound_Volume"` | Audio level | `0`-`100` |
| `"Sound_Paths"` | Sound files | `["sounds/effects/ding.wav"]` |
| `"Font_Name"` | Screen text font | `Arial` (Mode 6 only) |
| `"Font_Size"` | Text size | `24` (Mode 6 only) |
| `"RGBA_Color"` | Text color | `255,255,255,255` (White) |
| `"X_Axis"` | Horizontal position | `0.5` (Center) |
| `"Y_Axis"` | Vertical position | `0.5` (Center) |
| `"BackGround"` | Black background | `true`/`false` |

### **Placeholders**  
| Placeholder | Description | Example Output |
|-------------|-------------|----------------|
| `{nextline}` | Line break | `Line1{nextline}Line2` |
| `{PLAYER_NAME}` | Player's name | `Gold KingZ` |
| `{PLAYER_STEAMID}` | SteamID | `STEAM_0:1:122910632` |
| `{PLAYER_STEAMID3}` | SteamID3 | `[U:1:245821265]` |
| `{PLAYER_STEAMID32}` | SteamID32 | `245821265` |
| `{PLAYER_STEAMID64}` | SteamID64 | `76561198206086993` |
| `{TIME}` | 24h time | `14:30` |
| `{TIME2}` | 12h time | `2:30 PM` |
| `{TIME3}` | 24h with seconds | `14:30:45` |
| `{TIME4}` | 12h with seconds | `2:30:45 PM` |
| `{DATE}` | Day-first date | `25.12.2023` |
| `{DATE2}` | Month-first date | `12.25.2023` |
| `{SERVER_NAME}` | Server name | `Gold KingZ's Server` |
| `{SERVER_MAP_NAME}` | Original map name | `de_dust2` |
| `{SERVER_MAP2_NAME}` | Custom map name In (RenameMaps) | `Dust 2` |
| `{SERVER_IP}` | Server Ip In Server Lunch Option (-ip 127.0.0.1) | `123.45.67.89` |
| `{SERVER_IP2}` | Get Server Public IP | `123.45.67.89` |
| `{SERVER_PORT}` | Server Port | `27015` |
| `{SERVER_DNS}` | Server Domain | `myserver.com` |
| `{SERVER_MAXPLAYERS_COUNT}` | Server Max Players | `32` |
| `{SERVER_PLAYERS_COUNT}` | Players In Server Without Bots | `24` |
| `{SERVER_PLAYERS_WITH_BOTS}` | Players In Server With Bots | `28` |


</details>

---

## 📜 Changelog

<details>
<summary><b>📋 View Version History</b> (Click to expand 🔽)</summary>

### [1.0.1]
- Rework Plugin

- Remove Unnecessaries
- Support GIF 
- Change SendMessageEveryXMins To SendMessageOnEvery Choose Mins/Secs 
- Remove KEY No Longer Needed 
- DefaultServerLanguage No Longer Needed Auto Detect Server Lang
- Added Ads_Menu_CommandsInGame
- Added Ads_Menu_Flags
- Added Better Way On Permissions Flags/Groups/SteamIDs 
- Added PickSoundsByOrder
- Added RenameMaps
- Added RenameGroupsAndFlags
- Added Player_Logo_Path
- Added Reload_Advertisements_CommandsInGame
- Added Reload_Advertisements_Flags
- Added Test_Sounds_CommandsInGame
- Added Test_Sounds_Flags
- Added Ads_Default_Messages
- Added Ads_Default_Messages_Sounds
- Added Ads_Default_Wall_Logo
- Added Ads_Default_Wall_Text
- Added Ads_Default_Player_Logo
- Exlude Ads From Lang Folder Now Ads In `advertisements` Folder

### [1.0.0]
- Initial plugin release

</details>

---


