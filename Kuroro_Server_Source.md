
# Changelog M2Tec Server Source

- [Changelog M2Tec Server Source](#changelog-m2tec-server-source)
  * [- New Defines / Systems](#--new-defines---systems)
  * [- New Fixes](#--new-fixes)
  * [- New Questfunctions](#--new-questfunctions)
  * [- Removed Code](#--removed-code)

## - New Defines / Systems
```
+ add #define ENABLE_AUTODETECT_INTERNAL_IP // autodetect internal ip
+ add #define ENABLE_PORT_SECURITY // fix remote adminpage exploits
+ Add #define ENABLE_AGGREGATE_MONSTER_EFFECT ( cape effect )
+ add #define ENABLE_PRIVATE_SHOP_AUTO_CLOSE ( close empty shops )
+ add #define __IMMUNE_100PERCENT__
+ add #define WJ_ENABLE_TRADABLE_ICON
+ add #define WJ_ENABLE_COSTUME_MOUNT
+ add Global Config 
+ Mounts.txt add ( Add new mounts without edit the src for the dmg ) 
+ /reload m ( reload the Mounts.txt ) 
+ Add mark not tradeable items
+ add new gm command ( /gm_list )
+ add bann command ( /bann <name> <time in h> <reason>)
+ add unban command ( /unbann <name> )
+ add coints items ( 80014-80017 ( settings in source ))
+ add group buff system 
```
## - New Fixes
```
+ map/index core crach fixxed ( newline ) 
+ guild_add_member ( check is ns npc or mob ) 
+ when player die is the hp after not negative ( Offical like )
+ can't swap equipment when inv. is full
+ mount backport fix
+ fixed the unsigned bug ( do_war ) 
+ material skip exploit
+ kick Player when use Ghostmode
+ kick Player when use Wallhack 
+ Player can not use DropHack
+ Yangdrop EXPLOIT fixed 
+ Guildname fixed in the guild window
+ Guild Land Fixeds
+ false questname coredowner fix
+ skill group fix after change
+ Boss kick into walls fix
+ Change empire fix for guild
+ Fixed Emotions with color pen ( Kiss, Dance .... )
+ Fixed wedding map npc´s and little more about wedding
+ change sex without relog 
+ instand flash ( fix lost items ) 
+ fixed shaman buff without group
+ fixed guild create yang
+ Enchanted Blade fix
+ Faster disappearance of killed monsters. ( 2 sec ) later with config 
+ Invisible character fix
+ stack items you drop for Other guys in your party
+ Set/Get QuestFlag
+ 100% immune fix update with /full command fix 
```
## - New Questfunctions 
```
+ set_attr
+ get_attr_type
+ get_attr_value
```
## - Removed Code
```
+ removed vcard
+ removed auth_brazil
+ removed ROULETTE
+ Removed unused Packets
+ Removed all AUCTION
+ removed some useless syserr
```



