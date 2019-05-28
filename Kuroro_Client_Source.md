
# Changelog Kurorowork Client Source

- [Changelog Kuroro Client Source](#changelog-kurorowork-client-source)
  * [- New Defines / Systems](#--new-defines---systems)
  * [- Modification / Additions](#--modification---additions)
  * [- New Fixes](#--new-fixes)

## - New Defines / Systems
```	
#define PYTHON_UPDATE				
#define GRANNY_UPDATE					
#define HIDE_GRANNY_SYSERR					
#define HIDE_KINGDOM_FLAG_NPC			
#define ENABLE_INSTANT_QUEST_SPEED			
#define REMOVE_ITALIC_ON_WHISPER		
#define ENABLE_ATLASINFO_FROM_ROOT			
#define ENABLE_LOAD_ALTER_ITEMICON		
#define ENABLE_MONSTERLEVEL				
#define ENABLE_MONSTERSTERN					
#define DISABLE_BOSS_FLY				
#define ENABLE_NO_MOUNT_CHECK			
#define ENABLE_SKIN_EXTENDED				
#define ENABLE_PETS_WITHOUT_COLLISIONS		
#define ENABLE_SHOPS_WITHOUT_COLLISIONS	
#define ENABLE_MOUNTS_WITHOUT_COLLISIONS		
#define ENABLE_STONE_ON_MINIMAP		
#define ENABLE_UPDATE_LEVEL_TEXT
#define ENABLE_FAST_PICK_UP_ITEM_GROUND	
#define ENABLE_DROP_COLOR_OWNER_ITEM_GROUND
#define ENABLE_FLASH_APPLICATION_TASKBAR
#define ENABLE_GF_HEIGHT_OF_ACTORS
```
## - Modification / Additions
```
+ Python 2.7 updated.
+ Granny 2.9 updated.
+ Hide granny warning.
+ Hide kingdom flag in npc.
+ Enable instant quest speed.
+ Disable italic on whisper 	
+ Disable collisions for pets.
+ Disable collisions for shops.
+ Disable collisions for mounts.	
+ Read atlasinfo.txt from root instead of locale.
+ Load a default item icon if the one inside the item_list.txt is missing.
+ Enable level for monster.
+ Enable * before the name of the monster if they are aggressif.
+ If enabled, the boss can't fall when you attack.
+ Enable attack and skill from all horses/mounts.
+ Extended source/targetskin[2-9] inside .msm
+ Enable stone on minimap.
+ Update level text in real time.
+ Checking if the target is on horse or not for position of the range attack.
+ Delay for pick up item in the ground reduce.
+ Color the name of the owner of the drop in red if it is not yours.
+ When a private message is received, the icon of the taskbar will flash.
```
## - New Fixes
```
+ "SEQUENCE mismatch 0xaf != 0x64 header 254" fix
+ Sell item to npc.
+ Ctrl+V crash when pasting images&co.
+ For do_view_equip
+ If the client can not connect to the server, the client will wait one second to connect the server again.
+ When a character is logging out from the game near to your character you can see a fast equipment change (the character is unequipping everything from him/herself)
+ When you move camera and minimize client in the same time mouse remains blocked and you need to maximize client , stop move camera and minimize again. I fixed this.
+ Fix the positions of textails (name position changes by every update packet on the main character), and also the position of the emotions when you are on a mount. 
+ If you click a monster without having arrows, the automatic attack will go in loop. I fixed this.
+ When Assignment of skill points when a skill is active fixed.
+ CMapOutdoor::Load - LoadMonsterAreaInfo fixed.
+ Show the name of the failed mapped .dds load.
+ Non-printing/control characters were printed in the (chat) input (the ones you get when you press Ctrl+<key> in game)
+ On arabic locales, the [HyperText code] (alias Prism code) could be edited pressing <Backspace>
+ A new textureset index was -1 instead of 0
```


