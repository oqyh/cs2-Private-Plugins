
## .:[ Price ]:.
```diff
+ PRICE 5$ [Lifetime ( One Time Payment )] 
```

# [CS2] Advanced-ReservedSlots-GoldKingZ (1.0.0)  

### Dynamic Kick Reserved Slots Depend Group Priority

![image](https://github.com/oqyh/cs2-Private-Plugins/assets/48490385/c7eea100-f571-40e9-880c-ef2414e055d6)


## .:[ Dependencies ]:.
[Metamod:Source (2.x)](https://www.sourcemm.net/downloads.php/?branch=master)

[CounterStrikeSharp](https://github.com/roflmuffin/CounterStrikeSharp/releases)

[Newtonsoft.Json](https://www.nuget.org/packages/Newtonsoft.Json)


## .:[ Configuration ]:.

> [!CAUTION]
> Weapon Config Located In ..\addons\counterstrikesharp\plugins\Advanced-ReservedSlots-GoldKingZ\config\config.json                                         

```json

{

  //Key To Active Plugin
  "KEY": "",

  //Delay Kick To Show Message To Let Kicked Player Understand Why Get Kicked
  "Delaykick": true,

  //If Delaykick true How Much In Secs
  "DelayTimeXInSecs": 5,

}

```


## .:[ Configuration ReservedSlots ]:.

> [!CAUTION]
> Weapon Config Located In ..\addons\counterstrikesharp\plugins\Advanced-ReservedSlots-GoldKingZ\config\ReservedSlots_Settings.json                                         
```json

{
//it random kick first normal people when group_1 or 2 or 3 joined then if no normal people in game it random kick Group_1 and so on...
  "Group_1": {
    "GROUP_NAME": "VIPS", //Group Name
    "FLAGS": "@css/vip,#css/vip"
  },
  "Group_2": {
    "GROUP_NAME": "VVIPS",
    "FLAGS": "@css/vvip,#css/vvip"
  },
  "Group_3": {
    "GROUP_NAME": "ADMINS",
    "FLAGS": "@css/admin,#css/root"
  }
}

```

## .:[ Change Log ]:.
```
(1.0.0)
-Initial Release
```
