
# Changelog Kurorowork Server Source

- [Changelog Kuroro Server Source](#changelog-kurorowork-server-source)
  * [- New Defines / Systems](#--new-defines---systems)
  * [- New Systems](#--new-systems)
  * [- Modification / Additions](#--modification---additions)
  * [- New Fixes](#--new-fixes)
  * [- New Questfunctions](#--new-questfunctions)
  * [- Removed Code](#--removed-code)

## - New Defines / Systems
```
#define ENABLE_CHAT_LOGGING						 
#define ENABLE_CHAT_SPAMLIMIT					     
#define ENABLE_WHISPER_CHAT_SPAMLIMIT		
#define ENABLE_SKILL_NEED_EXP_DISABLE		
#define ENABLE_BUFF_TO_ALL_PARTY_MEMBER		
#define ENABLE_IGNORE_LOWER_BUFFS
#define ENABLE_BLOCK_SKILL_OXEVENT
#define ENABLE_PRIVATE_SHOP_AUTO_CLOSE
#define ENABLE_GOHOME_IFMAP_NOT_ALLOWED
#define ENABLE_GOHOME_IF_MAP_NOT_EXIST	
#define ENABLE_GM_FLAG_IF_TEST_SERVER		
#define ENABLE_GM_FLAG_FOR_LOW_WIZARD		
#define ENABLE_ANTI_CMD_FLOOD					     
#define ENABLE_OPEN_SHOP_WITH_ARMOR	
#define ENABLE_EFFECT_PENETRATE				    
#define ENABLE_EFFECT_EXTRAPOT					    
#define ENABLE_CMD_IPURGE_EX					      
#define ENABLE_SET_STATE_WITH_TARGET	
#define ENABLE_STATPLUS_NOLIMIT					   
#define ENABLE_FORCE2MASTERSKILL	
#define ENABLE_AUTODETECT_INTERNAL_IP
#define ENABLE_MYSQL_QUERY						       
#define ENABLE_TRANSLATE_LUA			
#define ENABLE_NEWSTUFF
#define ENABLE_STACK_POT_BELT_BEFORE_INVENTORY
#define ENABLE_STACK_DROP_ITEM_PARTY

```

## - New Defines / Systems
```
#define ENABLE_COSTUME_WEAPON_SYSTEM
#define ENABLE_MOUNT_COSTUME_SYSTEM
#define ENABLE_HIGHLIGHT_SYSTEM
#define ENABLE_SORT_INVENTORY
#define ENABLE_BIOLOG_SYSTEM
```

## - Modification / Additions
```
+ Player conversation stored in the chatlog table
+ Spam chat limit disconnected
+ Spam chat whisper limit disconnected
+ The required experience is no longer required to read a manual
+ Buff for all member of the party.
+ When you receive a lower buff than the one you currently own, it does not work.
+ Skills are blocked during an OX event ( command enable_block_skill_oxevent 1 for enable 0 for disable )
+ Close the private shop after it's sold out
+ If the position is not allowed, you return to your village
+ If the position is unknown, you return to your village
+ GM logo display in test server mode
+ Logo display for low wizard grade
+ Cmd Flood disconnected
+ Open a shop with your equipment
+ Penetrate effect enabled.
+ Pot Effect. Purple - Green
+ Extended purge commands.
+ State command targeting the player
+ Deleting the status limit
+ The skills pass in master to 17 points
+ Automatically configure the internal ip.
+ Mysql Query Command.
+ Enable translate.lua loading
+ Full_set updated with news items.
+ Die quest event.
+ Revive quest event.
+ Upgrade event quest.
+ Fishing complet event quest.
+ Stack potts directly in belt inventory, before putting them to inventory.
+ Stack items you drop for Other guys in your party.
+ Biolog system.
+ Inventory sort system.
+ Costume weapon system.
+ Costume mount system.
```
## - New Fixes
```
+ Dungeon (core downer)
+ P2P fix
+ Admin tool exploit fix
+ Sequence mismatch header 254 fix.
+ Fix equip item with full inventory.
+ When a character is logging out from the game near to your character you can see a fast equipment change (the character is unequipping everything from him/herself)
+ Enable stackable books instead of remove all the pile
+ Guild exploit fix
+ Guild comment flood mysql ( delay 10 min )
+ Mobs in safezone
+ Attack on the markets
+ Guild yang control
+ Guild level control 
+ Adminpage exploit
+ Skill to remain active when skill reset
+ [YMIR] Secondary skill levelup with skill group 0 fixed
+ [YMIR] Aura activated without weapon
+ Quickslot taskbar items
+ Absorption hp/sp of sura magic sword skill
+ Character delete
+ Change empire with guild
+ Invisibility problem with effect bug
+ Alignment calcul bug
+ ACMD(do_war) fixed the unsigned bug
+ Clientcheckversion fixed and delay from 10 to 0
+ Disabled every korean command
+ Full-speeded player is on a mount
+ Negative hp on dead
+ Call mount is fixed
+ Kill a player (war m), `when kill begin` will be triggered twice
+ IsExchanging and IsEquipped is now gathering
+ ComputePoints function fixed
+ Put item from safebox / mall to belt inventory fixed
+ Few packet IDs not checked
+ Refine scroll item value 1 from the magic stone was generating useless syserrs
+ No check on 6-7 add/change items about costume stuff
+ Lovepoints overflow fixed
+ /cube r_info exploit fix
+ Mining hack fix
+ Moblock/ Bravery cape hack fix
+ If two people buy the same item at the same time from a pc's shop, the slower one will receive a wrong return packet (crash client)
+ Ymir are no checks about the zero division exception: e.g. if you set a mob's max hp to 0 in the mob proto, you'll get random crashes.
+ When a player dies, the HP could have a negative value. Now it's 0 like the official.
+ The belt could be put into the safebox even though the belt inventory isn't empty.
+ The items in the belt inventory could be used even if their slot were not available
+ Sql injection fix about net.SendMessengerRemovePacket
+ Sql injection fix about net.SendAnswerMakeGuildPacket
+ If map/index doesn't end with a newline, the game will crash
+ Guild_add_member can add any vid as guild's member even if it's a mob or an npc
+ Refine material skip exploit if items are swapped
+  When you kill the devil tower boss and get your reward and try to upgrade your weapon or anything, if you press yes and you does not have money less then the cost you will lost the reward. I fixed this 
+ I observed that horse level is missing from client. You are able to see the level only when you advance your horse or when you take with a command (for GMs). I fixed this.
```
## - New Questfunctions 
```
#define ENABLE_QUEST_DIE_EVENT					
#define ENABLE_QUEST_REVIVE_EVENT		
#define ENABLE_QUEST_UPGRADE_EVENT	
#define ENABLE_QUEST_FISHING_EVENT	
```
## - Removed Code
```
+ removed Cryptopp 
+ removed Panama 
+ removed Cipher
+ removed Auth Brazil 
+ removed IMPROVED PACKET ENCRYPTION 
+ removed Nprotect
+ removed Xtrap
+ removed Hackshield
+ removed Auction
+ removed BlockCountry (BlockException)
+ removed Monarch
+ removed SMS pool / Mobile
+ removed PcBang
+ removed SpeedServer
+ removed TeenServer
+ removed Lizenzserver
+ removed TimeBomb
+ removed MatrixCard.
+ removed PassPod
```



