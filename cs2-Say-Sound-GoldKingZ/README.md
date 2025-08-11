
## .:[ Price ]:. [(Payment Rules)](https://github.com/oqyh/cs2-Private-Plugins/blob/8040379022008134dde7d34cf08f7a611c750862/README.md?plain=1#L7)
```diff
+ PRICE 10$ + FREE Multiple Servers [Lifetime ( One Time Payment )] 
```

# [CS2] Say-Sound-GoldKingZ (1.0.6)

Let Players Convert Chat/Radio To Say Sound With Radius


[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/GWZRZuL20QA/0.jpg)](https://www.youtube.com/watch?v=GWZRZuL20QA)

![mode1](https://github.com/user-attachments/assets/9a1a1524-a752-4808-8f61-ccfeab800afd)
![mode2](https://github.com/user-attachments/assets/2b63a3ef-0d50-489c-b7f1-0c21603a2b79)
![mode3](https://github.com/user-attachments/assets/0a5f692e-3854-4c3d-a08c-3762046e9b2a)

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
1. Download the latest `Say-Sound-GoldKingZ.x.x.x.zip` In Discord
2. Extract contents to your `csgo` directory
3. Configure settings in `Say-Sound-GoldKingZ/config/config.json`
4. Restart your server

---

# ⚙️ Configuration

> [!IMPORTANT]
> **Main Configuration**  
> `../Say-Sound-GoldKingZ/config/config.json`  
> **Advertisements Configuration**  
> `../Say-Sound-GoldKingZ/config/saysound_config.json`  

## 🛠️ `config/config.json`

<details open>
<summary><b>Main Config</b> (Click to expand 🔽)</summary>

| Property | Description | Values / Example | Required |
|:--------:|:------------|:-----------------|:--------:|
| `Reload_Json_CommandsInGame` | Commands to reload `saysound_config.json` in-game | `""` = disable<br>`"!reloadsaysound,!reloadss"` | - |
| `Reload_Json_Flags` | Who can run reload commands (Flags / Groups / SteamIDs) | e.g. `Flags: @css/root,@css/admin` or `SteamID: 7656119...` or `""` = everyone | - |
| `Reload_Json_Hide` | Hide chat after executing reload command | `0` = No<br>`1` = Yes (only on success)<br>`2` = Always hide | - |
| `OpenMenu_Mode` | Menu mode / UI type | `0` = Disabled<br>`1` = Chat Menu<br>`2` = Center Menu<br>`3` = Center WASD Menu<br>`4` = Screen Text WASD Menu (disabled) | - |
| `OpenMenu_CommandsInGame` | Commands to open SaySound menu | `""` = disable<br>`"!ssmenu,!saysoundmenu,!saysoundsmenu"` | - |
| `OpenMenu_Flags` | Who can use menu (Flags/Groups/SteamIDs) | e.g. `""` = everyone | - |
| `OpenMenu_Hide` | Hide chat after executing open-menu command | `0` = No<br>`1` = Yes (only on success)<br>`2` = Always hide | - |
| `RepositionMenu_CommandsInGame` | (Only for `OpenMenu_Mode = 4`) Commands to reposition menu | `""` = disable<br>`"!ressmenu,!repmenu,!reposition,!rep"` | - |
| `DisableOnWarmUp` | Disable SaySound during warmup | `true` / `false` | - |
| `AllowDeadPlayersToSaySound` | Allow dead players to toggle/play sounds | `true` / `false` | - |
| `PickSoundsByOrder` | Play sounds sequentially (top→bottom) or randomly | `true` = sequential<br>`false` = random | - |
| `Default_Sounds` | Enable sounds by default for new players | `true` / `false` | - |
| `Default_Messages` | Enable messages by default for new players | `true` / `false` | - |
| `Immunity_From_Cooldown_Flags` | Flags/Groups/SteamIDs exempt from cooldown | e.g. `Flags: @css/root,@css/admin` or `""` = disable cooldown | - |
| `Toggle_Sounds.Toggle_Sounds_CommandsInGame` | Commands to toggle/stop sounds | `""` = disable<br>`"!mutesound,!stopsound,!mutesounds,!stopsounds"` | - |
| `Toggle_Sounds.Toggle_Sounds_Flags` | Who can use toggle-sounds commands | e.g. `Flag: @css/root,@css/admin | Group: #css/root,#css/admin` | - |
| `Toggle_Sounds.Toggle_Sounds_Hide` | Hide chat behaviour for toggle-sounds commands | `0` / `1` / `2` (same meanings as other `_*_Hide`) | - |
| `Toggle_Messages.Toggle_Messages_CommandsInGame` | Commands to toggle messages | `""` = disable<br>`"!mutemessage,!stopmessage,!mutemessages,!stopmessages"` | - |
| `Toggle_Messages.Toggle_Messages_Flags` | Who can toggle messages | e.g. `""` = everyone | - |
| `Toggle_Messages.Toggle_Messages_Hide` | Hide chat behaviour for toggle-messages commands | `0` / `1` / `2` | - |
| `Cookies_Enable` | Save player data locally (cookies directory) | `true` / `false` | - |
| `Cookies_AutoRemovePlayerOlderThanXDays` | Auto-delete cookies older than X days (0 = disabled) | Number (e.g. `7`) | Required if `Cookies_Enable = true` |
| `MySql_Enable` | Save players’ data to MySQL | `true` / `false` | - |
| `MySql_Host` | MySQL host | e.g. `"127.0.0.1"` or `"MySql_Host"` | Required if `MySql_Enable = true` |
| `MySql_Database` | Database name | e.g. `"SaySoundDB"` | Required if `MySql_Enable = true` |
| `MySql_Username` | DB username | e.g. `"db_user"` | Required if `MySql_Enable = true` |
| `MySql_Password` | DB password | e.g. `"secret"` | Required if `MySql_Enable = true` |
| `MySql_Port` | DB port | Number (default `3306`) | - |
| `MySql_AutoRemovePlayerOlderThanXDays` | Auto-delete inactive DB rows older than X days (0 = disabled) | Number (e.g. `7`) | Required if `MySql_Enable = true` |

</details>

<details>
<summary><b>Utilities</b> (Click to expand 🔽)</summary>

| Property | Description | Values / Example | Required |
|:--------:|:------------|:-----------------|:--------:|
| `AutoUpdateSignatures` | Auto-update signatures in `gamedata/` | `true` / `false` | - |
| `EnableDebug` | Enable debug output to server console | `true` / `false` | - |

</details>


---

## 🛠️ `config/saysound_config.json`

<details open>
<summary><b>SaySound Options</b> (Click to expand 🔽)</summary>

| Key | Description | Values / Examples |
|-----|-------------|-------------------|
| `"Hide_It_And_Show_Only_ForFlags"` | Hide Menu/SubMenu and only show for these flags | `"group:#css/vips,#css/admins"` |
| `"Only_These_Flags_Can_Access_It"` | Only these can access Menu/SubMenu | `"SteamID: 76561198206086993,76561198974936845 \| Flag: @css/vips,@css/admins"` |
| `"SubMenu.STATUS.TOGGLE_SOUND.xxxxxxxxxxx:"` | Show client current SaySound **Sound** status (Enabled/Disabled) |
| `"SubMenu.STATUS.TOGGLE_MESSAGE.xxxxxxxxxxx:"` | Show client current SaySound **Message** status (Enabled/Disabled) |
| `"Toggle_Sound_In_Radio"` | Hook these radio sounds | `"cheer,coverme"`<br>*(examples: coverme, takepoint, holdpos, regroup, followme, takingfire, go, fallback, sticktog, getinpos, stormfront, report, roger, enemyspot, needbackup, sectorclear, inposition, reportingin, getout, negative, enemydown, sorry, cheer, compliment, thanks, go_a, go_b, needrop, deathcry)* |
| `"Toggle_Sound_In_Radio_Hide"` | Hide radio after toggle passes | `0` = No<br>`1` = Yes (only after success)<br>`2` = Always hide |
| `"Toggle_Sound_In_Chat"` | Toggle shortcut in chat | `"hi,hello"` *(commands starting with `!` or `css_` can be used in both chat & console)* |
| `"Toggle_Sound_In_Chat_Hide"` | Hide chat after toggle passes | `0` = No<br>`1` = Yes (only after success)<br>`2` = Always hide |
| `"PrintToChat"` | Print to chat? | `0` = No<br>`1` = Yes (local to player)<br>`2` = Yes (to all) |
| `"OnlyForTeam"` | Restrict by team | `0` = Any team<br>`1` = CT only<br>`2` = T only |
| `"Give_Cooldown_After_This_InXSecs"` | Cooldown after execution (seconds) | `5` |
| `"Play_Sound_To_Ears"` | Play sound to player’s ears only | `true` / `false` |
| `"Sound_Volume"` | Volume level | `"60%"` *(1% to 100%, default = 100%)* |
| `"Sound_Paths"` | List of sounds to play | `["wakeup","bye"]` |

</details>

---

## 📜 Changelog

<details>
<summary><b>📋 View Version History</b> (Click to expand 🔽)</summary>

### [Say-Sound-GoldKingZ 1.0.6]
- Fix some bugs
- Fix `Reload_Json` When Reload Not Hook/Unhook Radio + Chat
- Updated `Menu-API-GoldKingZ` To 1.0.2
- Added `Sound_Volume` Ability To Reduse Orginal Audio Volume
- Added Ability Sound Enable/Disable Client Side
- Added `Play_Sound_To_Ears` Play Sound To Players Ears? || true = Yes || false OR Not Used = No Player Sound Globally
- Added `PrintToChat` Print To Chat? || 1 = Yes, Locally To Player || 2 = Yes, To All || 0 OR Not Used = No
- Added `Toggle_Sounds_CommandsInGame` Ability To Toggle SaySound Sounds On The Console And Chat
- Added `Toggle_Sounds_Flags` Flags Or Group Or SteamID For `Toggle_Sounds_CommandsInGame` 
- Added `Toggle_Messages_CommandsInGame` Ability To Toggle SaySound Messages On The Console And Chat
- Added `Toggle_Messages_Flags` Flags Or Group Or SteamID For `Toggle_Messages_CommandsInGame` 
- Added `Reload_Json_Hide` Ability To Hide/Show After Reload_Json || 1 = Yes, But Only After Toggle Successfully || 2 = Yes, Hide All The Time || 0 = No
- Added `OpenMenu_Hide` Ability To Hide/Show After OpenMenu || 1 = Yes, But Only After Toggle Successfully || 2 = Yes, Hide All The Time || 0 = No
- Added `Toggle_Sounds_Hide` Ability To Hide/Show After Toggle_Sounds || 1 = Yes, But Only After Toggle Successfully || 2 = Yes, Hide All The Time || 0 = No
- Added `Toggle_Messages_Hide` Ability To Hide/Show After Toggle_Messages || 1 = Yes, But Only After Toggle Successfully || 2 = Yes, Hide All The Time || 0 = No
- Remove `PrintChatToAll`

### [SaySound_App_GoldKingZ 1.0.1]
- Fix some bugs
- Fix vsndevts On Create
- Added `Click_On_Me_To_Run_App.bat` To Start App
- Removed exe For False Virus

---

### [1.0.5]
- Fix some bugs  
- Fix MySQL  
- Rework on plugin  
- Rework on `Sound_Paths`  
- Added `OnlyForTeam`  
- Added `PrintChatToAll`  
- Added `PrintChatToPlayer`  
- Added `Reload_Json_Flags`  
- Added `Reload_Json_CommandsInGame`  
- Added `Default_Toggle_Sound`  
- Added `Default_Toggle_Message`  
- Added `DisableOnWarmUp`  
- Added `Pick_Random_SaySound`  
- Added `AutoUpdateSignatures`  
- Added GKZ `MenuApi`  
- Added `TOGGLE_SOUND`  
- Added `TOGGLE_MESSAGE`  
- Removed `Print_To_Chat`  

---

### [1.0.4]
- Fix some bugs  
- Added `Hide_It_And_ShowThisOnlyForFlags` in SaySound_Settings  
- Added `ImmunityFromCooldownFlags` in configs  

---

### [1.0.3]
- Added `ChangeCheckIpAdressToWebSite`  
- Added `OpenMenu_Mode 3` custom menu (Chat Center WASD navigation for menu and submenus)  
- Added `OpenMenu_Flags`  
- Added `OpenMenu_CommandsInGame`  
- Added `OpenMenu_CloseMenuAfterSelectItem`  
- Added `Toggle_DisableSaySoundsFlags`  
- Added `Toggle_DisableSaySoundsCommandsInGame`  
- Added `Toggle_AutoRemovePlayerCookieOlderThanXDays`  
- Added `MenuWASD_FreezePlayerOnMenuOpen`  
- Added `MenuWASD_ExitMenuOnPressing`  
- Added `Enable_UseMySql`  
- Added `MySqlHost`  
- Added `MySqlDatabase`  
- Added `MySqlUsername`  
- Added `MySqlPassword`  
- Added `MySqlPort`  

---

### [1.0.2]
- Added `AllowDeadPlayersToSaySound`  

---

### [1.0.1]
- Fix some bugs  
- Added `gkz_plugins` to check status of GKZ plugins  
- Added `MAKE_SOUND_3D`  
- Added `Override_These_Plugins`  

---

### [1.0.0]
- Initial release  

</details>

---
