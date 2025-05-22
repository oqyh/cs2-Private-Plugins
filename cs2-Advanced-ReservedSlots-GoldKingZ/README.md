
## .:[ Price ]:. [(Payment Rules)](https://github.com/oqyh/cs2-Private-Plugins/blob/8040379022008134dde7d34cf08f7a611c750862/README.md?plain=1#L7)
```diff
+ PRICE 5$ + FREE Multiple Servers [Lifetime ( One Time Payment )] 
```

# [CS2] Advanced-ReservedSlots-GoldKingZ (1.0.1)  

### Dynamic Kick Reserved Slots Depend Group Priority 
### When Server Is Full - 1  It Will Start KickMode Depend Priority Group You Set In ReservedSlots_Settings.json 

![image](https://github.com/oqyh/cs2-Private-Plugins/assets/48490385/c7eea100-f571-40e9-880c-ef2414e055d6)

![serverfull](https://github.com/oqyh/cs2-Private-Plugins/assets/48490385/789259bd-a31c-40b5-a140-5ddf26c04bbf)


---

## 📦 Dependencies
[![Metamod:Source](https://img.shields.io/badge/Metamod:Source-2d2d2d?logo=sourceengine)](https://www.sourcemm.net)

[![CounterStrikeSharp](https://img.shields.io/badge/CounterStrikeSharp-83358F)](https://github.com/roflmuffin/CounterStrikeSharp)

[![JSON](https://img.shields.io/badge/JSON-000000?logo=json)](https://www.newtonsoft.com/json) [Included in zip]

---

## 📥 Installation

### Plugin Installation
1. Download the latest `Advanced-ReservedSlots-GoldKingZ.x.x.x.zip` In Discord
2. Extract contents to your `csgo` directory
3. Configure settings in `Advanced-ReservedSlots-GoldKingZ/config/config.json`
4. Restart your server

---

# ⚙️ Configuration

> [!IMPORTANT]
> **Main Configuration**  
> `../Advanced-ReservedSlots-GoldKingZ/config/config.json` 

## 🛠️ `config/config.json`

<details open>
<summary><b>Main Config</b> (Click to expand 🔽)</summary>

| Property | Description | Values | Required |  
|----------|-------------|--------|----------|
| `Reload_Json_CommandsInGame` | Commands to reload ReservedSlots_Settings.json. Commands starting with '!'/`css_` work in chat/console. | Example: `!reloadreserved,!reloadreserv`<br>`""`-Disable | - |
| `Reload_Json_Flags` | Flags/Groups/SteamIDs allowed to reload settings | Format: `SteamID: X \| Flag: Y \| Group: Z`<br>Example: `SteamID: 76561198206086993 \| Flag: @css/vips`<br>`""`-Allow everyone | `Reload_Json_CommandsInGame` ≠ `""` |
| `Reload_Json_Hide` | Hide chat message after successful reload | `true`-Yes<br>`false`-No | `Reload_Json_CommandsInGame` ≠ `""` |
| `KickMode` | Kick priority method for reserved slots. | `0`-Random<br>`1`-Highest Ping<br>`2`-Highest Score<br>`3`-Lowest Score<br>`4`-Longest Time<br>`5`-Shortest Time | - |
| `PriorityKickOnSpecPlayers` | Prioritize kicking spectators first. | `true`-Yes<br>`false`-No | - |
| `KickWithReason` | Show a proper kick reason to players. | `true`-Yes<br>`false`-No | - |
| `Delaykick` | Enable delayed kick. | `true`-Yes<br>`false`-No | - |
| `DelayTimeXInSecs` | Delay duration before kick | Integer (seconds)<br>Example: `10` | `Delaykick` = `true` |

</details>

<details>
<summary><b>Utilities Config</b> (Click to expand 🔽)</summary>

| Property | Description | Values | Required |  
|----------|-------------|--------|----------|
| `EnableDebug` | Debug Mode | `true`-Enable<br>`false`-Disable | - |

</details>

---

## 📜 Changelog

<details>
<summary><b>📋 View Version History</b> (Click to expand 🔽)</summary>

### [1.0.3]
- Rework Plugin
- Remove Unnecessaries
- Added Info On Each Config
- Added Reload_Json_CommandsInGame Ability To Toggle Throw Console/Chat
- Added Reload_Json_Hide

### [1.0.2]
- Fix Api Crash

### [1.0.1]
- Fix Bugs
- Fix GKZ Api
- Remove Port Restricted
- Remove Key No Needed
- Added KickMode (Kick Random Players,Kick Highest Ping,Kick Highest Score,Kick Lowest Score,Kick Player Who In The Server Longest Time,Kick Player Who In The Server Shortest Time)
- Added PriorityKickOnSpecPlayers 
- Added KickWithReason 
- Added Reload_Json_Flags 
- Added Reload_Json_CommandsInGame 

### [1.0.0]
- Initial plugin release

</details>
