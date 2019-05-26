
# Changelog Kurorowork Server Source

- [Changelog Kuroro Server Source](#changelog-kurorowork-server-source)
  * [- New Defines / Systems](#--new-defines---systems)
  * [- Modification / Additions](#--modification---additions)
  * [- List of new game/ CONFIG options](#--New-game---config-options)
  * [- New Fixes](#--new-fixes)
  * [- New Questfunctions](#--new-questfunctions)
  * [- Removed Code](#--removed-code)

## - New Defines / Systems
```
#define ENABLE_CHAT_LOGGING						 
#define ENABLE_CHAT_SPAMLIMIT					     
#define ENABLE_WHISPER_CHAT_SPAMLIMIT		
#define ENABLE_SKILL_NEED_EXP_DISABLE		
#define ENABLE_IGNORE_LOWER_BUFFS
#define ENABLE_BLOCK_SKILL_OXEVENT
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
#define ENABLE_QUEST_DIE_EVENT					
#define ENABLE_QUEST_REVIVE_EVENT		
#define ENABLE_QUEST_UPGRADE_EVENT	
#define ENABLE_QUEST_FISHING_EVENT	

```
## - List of new game/ CONFIG options

```
+ MAX_LEVEL //  <0-1>  // Set the level max
+ TRADE_EFFECT  //  <0-1>  // Enable the effect when an exchange is made
+ GLOBAL_SHOUT  //  <0-1>  // Enable shout as global (not enabled by default)
+ STONE_CHANCE  //  <int>  // Set the % of succes of liking stone (default 30)
+ REMOVE_STONE  //  <0-1>  // Remove the piece of broken stone when extracting stone from an item (not enabled bu default)
+ BOOTARY_CHECK // <0-1> // Enable opening a shop only in village maps (not enabled by default)
+ GM_HOST_CHECK // <0-1> // Enable the gm host check based on ip (unchecked by default)
+ UNLIMITED_CAPE // <0-1> // Enable the capes of bravery unlimited  (not enabled by default)
+ UNLIMITED_POTION // <0-1> // Enable the potion red & blue unlimited  (not enabled by default)
+ ITEM_COUNT_LIMIT // <1-250> // You can set the maximum item count (e.g.) to 250 (200 by default)
+ ACCESSORY_CHANCE //  <int>  // Set the % of succes of liking accessory  (default 50)
+ ADD_BONUS_CHANCE //  <int>  // Set the % of succes of add a bonus (default 50)
+ ADD_BONUS_CHANCE5 //  <int>  // Set the % of succes of add the 5th bonus (default 30)
+ SHOP_PRICE_3X_TAX // <0-1> // Disable the price increase on foreign empires (not disabled by default)
+ SHOUT_LIMIT_LEVEL // <int> // Set the requirement level to use the shout (default 15)
+ PRISM_ITEM_REQUIRE // <0-1> // Disable prism requirement (not disabled by default)
+ BLOCK_CHAR_CREATION // <0-1> // If enabled, character creation will be disabled
+ EMOTION_MASK_REQUIRE // <0-1> // Disable emotion mask requirement (not disabled by default)
+ EMPIRE_LANGUAGE_CHECK // <0-1> // If enabled, you won’t need to read language books or have the relative ring to understand other empires
+ CHANGE_ATTR_TIME_LIMIT // <seconds> // Alternative (60 secs as default, 0=disable)
+ GUILD_INFINITE_MEMBERS // <0-1> // If enabled, every guild can have infinite members (not enabled by default)
+ SKILLBOOK_NEXTREAD_MIN // <int> // Set the min value of the next read skill book time (default 28800)
+ SKILLBOOK_NEXTREAD_MAX // <int> // Set the max value of the next read skill book time (default 43200)
+ ITEM_DESTROY_TIME_AUTOGIVE // Set the destroy time for the autogive items (from boxes if inventory is full and so on) spawned (on the ground) (300 as default)
+ ITEM_DESTROY_TIME_DROPGOLD // Set the destroy time for the gold (yang) dropped by the players (150 as default)
+ ITEM_DESTROY_TIME_DROPITEM // Set the destroy time for the items dropped by the players (300 as default)
+ STATUS_POINT_SET_MAX_VALUE // <int> // Set the maximum settable points for status (default 90)
+ STATUS_POINT_GET_LEVEL_LIMIT // <level> // Set the maximum level to get status point (default lvl 90)

```
## - Modification / Additions
```
+ Player conversation stored in the chatlog table
+ Spam chat limit disconnected
+ Spam chat whisper limit disconnected
+ The required experience is no longer required to read a manual
+ When you receive a lower buff than the one you currently own, it does not work.
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
```
## - New Fixes
```
+ Dungeon (core downer)
+ P2P fix
+ Admin tool exploit fix 
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
```
## - New Questfunctions 
```
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



