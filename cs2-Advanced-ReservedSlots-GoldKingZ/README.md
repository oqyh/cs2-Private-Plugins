
## .:[ Price ]:.
```diff
+ PRICE 5$ [Lifetime ( One Time Payment )] 
+ If You Have Multiple Servers And You Want Plugin To All Your Servers
+ Rule 1: Must Be Same Prefix Server Name Otherwise You Will Be 5$ Again
+ Rule 2: If Moderator Found Before Paying Was Same Prefix Server Name After Paying Changed Without Telling Them Or Using Tricky Way You Will Be Banned And Your Key Will Removed 

example of Same Prefix Server (GKZ is prefix)
GKZ | Retake Server 
GKZ | 1v1 Server 
GKZ | surf Server

After Paying Will Will Receive Only Compiled Plugin (Not Open Source) + Key To Active Plugin
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
