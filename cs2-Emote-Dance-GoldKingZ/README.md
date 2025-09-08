
## .:[ Price ]:. [(Free Private Rules)](https://github.com/oqyh/cs2-Private-Plugins/blob/11b92dc04067753a390d796dbba39d789f270aab/README.md?plain=1#L27)
```diff
+ PRICE FREE [Only Discord Members] 
```

# [CS2] Emote-Dance-GoldKingZ (1.0.4)  

### Fortnite Dance Emote Animation 

## 🖼️ ShowCase GIF

![Emote_ShowCase](https://github.com/user-attachments/assets/d7ac663e-ba4a-4c2a-b031-e3d3f117f4e6)


## ▶️ ShowCase Video

[![Watch the video](https://img.youtube.com/vi/FfsralH4H9U/maxresdefault.jpg)](https://youtu.be/FfsralH4H9U)

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
1. Download the latest `Emote-Dance-GoldKingZ.x.x.x.zip` In Discord
2. Extract contents to your `csgo` directory
3. Configure settings in `Emote-Dance-GoldKingZ/config/config.json`
4. Restart your server

---

# ⚙️ Configuration

> [!IMPORTANT]
> **Main Configuration**  
> `../Emote-Dance-GoldKingZ/config/config.json`  
> **Emote Configuration**  
> `../Emote-Dance-GoldKingZ/config/emote_config.json`  

## 🛠️ `config/config.json`

<details open>
<summary><b>Main Config</b> (Click to expand 🔽)</summary>

| Property | Description | Values | Required |
|----------|-------------|--------|----------|
| `Reload_Emote_CommandsInGame` | Commands to reload emote plugin | Format: `Console_Commands: cmd1,cmd2 \| Chat_Commands: cmd3,cmd4` | Yes |
| `Reload_Emote_Flags` | Who can use reload commands | Format: `SteamIDs: id1,id2 \| Flags: @flag1 \| Groups: #group1` | Yes |
| `Reload_Emote_Hide` | Hide chat after reload command | `0`-No<br>`1`-Hide on success<br>`2`-Always hide | Yes |
| `OpenMenu_Mode` | How to open emote menu | `0`-Disabled<br>`1`-Chat menu<br>`2`-Center menu<br>`3`-Center WASD<br>`4`-Screen Text WASD | Yes |
| `OpenMenu_CommandsInGame` | Commands to open menu | Format: `Console_Commands: cmd1,cmd2 \| Chat_Commands: cmd3,cmd4` | Yes |
| `OpenMenu_Flags` | Who can open menu | Format: `SteamIDs: id1,id2 \| Flags: @flag1 \| Groups: #group1` | Yes |
| `OpenMenu_Hide` | Hide chat after menu command | `0`-No<br>`1`-Hide on success<br>`2`-Always hide | Yes |
| `DisableOnWarmUp` | Disable emotes during warmup | `true`-Yes<br>`false`-No | - |
| `PickSoundsByOrder` | Play sounds in order | `true`-Sequential<br>`false`-Random | - |
| `CameraViewOnEmote` | Camera view during emote | `0`-No change<br>`1`-Third person<br>`2`-Smooth third person | - |
| `HidePlayersOnEmote` | Hide players during emote | `0`-No<br>`1`-Only enemies<br>`2`-All players | - |
| `FreezePlayerOnEmote` | Freeze player during emote | `0`-No<br>`1`-Yes<br>`2`-Yes (if not already frozen) | - |
| `StopEmoteOnDamage` | Stop emote when taking damage | `true`-Yes<br>`false`-No | - |
| `StopEmoteOnPostion` | Stop emote if position changes | `true`-Yes<br>`false`-No | - |
| `StopEmoteOnPressing` | Keys that stop emote | Comma-separated key names | - |
| `IgnoreStopEmoteOnPressingOnWASD` | Ignore stop keys when WASD menu open | `true`-Yes<br>`false`-No | - |
| `Immunity_From_Cooldown_Flags` | Who has cooldown immunity | Format: `SteamIDs: id1,id2 \| Flags: @flag1 \| Groups: #group1` | - |
| `Default_Sounds` | Default sound setting for new players | `true`-On<br>`false`-Off | - |
| `Default_Messages` | Default message setting for new players | `true`-On<br>`false`-Off | - |
| `Cookies_Enable` | Enable local data storage | `true`-Yes<br>`false`-No | - |
| `Cookies_AutoRemovePlayerOlderThanXDays` | Auto-delete inactive data | `0`-Disabled<br>`>0`-Days to keep | If Cookies_Enable=true |
| `MySql_Enable` | Enable MySQL storage | `true`-Yes<br>`false`-No | - |
| `MySql_Host` | MySQL host address | IP/hostname | If MySql_Enable=true |
| `MySql_Database` | Database name | String | If MySql_Enable=true |
| `MySql_Username` | Database username | String | If MySql_Enable=true |
| `MySql_Password` | Database password | String | If MySql_Enable=true |
| `MySql_Port` | Database port | Number (default: 3306) | If MySql_Enable=true |
| `MySql_AutoRemovePlayerOlderThanXDays` | Auto-delete inactive data | `0`-Disabled<br>`>0`-Days to keep | If MySql_Enable=true |

</details>

<details>
<summary><b>Utility Settings</b> (Click to expand 🔽)</summary>

| Property | Description | Values | Required |
|----------|-------------|--------|----------|
| `AutoUpdateSignatures` | Auto-update game signatures | `true`-Yes<br>`false`-No | - |
| `EnableDebug` | Enable debug mode | `true`-Yes<br>`false`-No | - |

</details>

---


## 🛠️ `config/emote_config.json`

<details open>
<summary><b>Message Configuration</b> (Click to expand 🔽)</summary>

## 🔄 Status Indicators

| Option | Description |
|--------|-------------|
| `SubMenu.STATUS.TOGGLE_SOUND.xxxxxxxxxxx` | Show sound toggle status |
| `SubMenu.STATUS.TOGGLE_MESSAGE.xxxxxxxxxxx` | Show message toggle status |
| `SubMenu.STATUS.REPOSITION.xxxxxxxxxxx` | Allow menu repositioning |

## ⚙️ General Options

| Option | Description | Format/Values |
|--------|-------------|---------------|
| `Hide_It_And_Show_Only_ForFlags` | Restrict visibility | `SteamIDs: id1,id2 \| Flags: @flag1 \| Groups: #group1` |
| `Only_These_Flags_Can_Access_It` | Restrict access | `SteamIDs: id1,id2 \| Flags: @flag1 \| Groups: #group1` |
| `Toggle_In_Radio` | Bind to radio command | Comma-separated radio commands |
| `Toggle_In_Radio_Hide` | Hide radio message | `0`-No<br>`1`-On success<br>`2`-Always |
| `Toggle_In_Chat` | Bind to chat/console command | `Console_Commands: cmd1,cmd2 \| Chat_Commands: cmd3,cmd4` |
| `Toggle_In_Chat_Hide` | Hide chat message | `0`-No<br>`1`-On success<br>`2`-Always |
| `PrintToChat` | Notification type | `0`-None<br>`1`-To player<br>`2`-To all |
| `OnlyForTeam` | Team restriction | `0`-Any<br>`1`-CT only<br>`2`-T only |

## 🎬 Animation Options

| Option | Description | Format/Values |
|--------|-------------|---------------|
| `Model` | Animation model path | `models/path/to/model.vmdl` |
| `RandomAnimationName` | Random animations | `["anim1", "anim2", "anim3"]` |
| `AnimationName` | Primary animation | Animation name string |
| `AnimationName2` | Secondary animation | Animation name string |
| `LoopAnimation` | Loop animation | `true`-Yes<br>`false`-No |
| `RepeatMusicOnEveryXSecs` | Music repeat interval | Number of seconds |
| `RepeatMusicAfterXFrames` | Music repeat by frames | Number of frames |

## 🔊 Sound Options

| Option | Description | Format/Values |
|--------|-------------|---------------|
| `Sound_Volume` | Sound volume level | `1%`-`100%` (default: 100%) |
| `Sound_Paths` | Sound file paths | `["sound1", "sound2", "sound3"]` |

## ⏱️ Cooldown Options

| Option | Description | Format/Values |
|--------|-------------|---------------|
| `Give_Cooldown_After_This_InXSecs` | Cooldown duration | Number of seconds |

</details>

---

## 📜 Changelog

<details>
<summary><b>📋 View Version History</b> (Click to expand 🔽)</summary>

### [1.0.4]
-Rework + Optimize On Plugin 
-Fix Players Flags
-Fix Bug On Gloves + Teleporting
-Rework On ReloadJson To Reload Rntire Plugin
-Rework Config Added Comments Each Config
-Update Menu-API-GoldKingZ To 1.0.2
-Added Reload_Emote_Hide
-Added OpenMenu_Hide
-Added Third Person Smooth Camera
-Added PickSoundsByOrder
-Added DisableOnWarmUp
-Added HidePlayersOnEmote
-Added StopEmoteOnPostion
-Added Default_Sounds
-Added Default_Messages
-Added Cookies_Enable
-Added Cookies_AutoRemovePlayerOlderThanXDays
-Added MySql_Enable
-Added MySql_AutoRemovePlayerOlderThanXDays
-Added AutoUpdateSignatures
-Added AutoUpdateSignatures
-Added OnlyForTeam For Specific Emote
-Added SubMenu.STATUS.TOGGLE_SOUND.xxxxxxxxxxx
-Added SubMenu.STATUS.TOGGLE_MESSAGE.xxxxxxxxxxx
-Added SubMenu.STATUS.REPOSITION.xxxxxxxxxxx
-Added Toggle_In_Radio
-Added Toggle_In_Radio_Hide
-Added Toggle_In_Chat_Hide
-Remove PrintChatToAll
-Remove PrintToChat 1 = Locally | 2 = All

### [1.0.3]
-Fix GKZ Api

### [1.0.2]
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

### [1.0.1]
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

### [1.0.0]
- Initial plugin release

</details>
