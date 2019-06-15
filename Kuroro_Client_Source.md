
# Changelog Kurorowork Client Source

- [Changelog Kuroro Client Source](#changelog-kurorowork-client-source)
  * [- New Defines / Systems](#--new-defines---systems)
  * [- New Systems](#--new-systems)
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

## - New Systems
```	
#define ENABLE_TARGET_SELECT_COLOR
#define ENABLE_HIGHLIGHT_SYSTEM
#define ENABLE_BIOLOG_SYSTEM
#define WJ_ENABLE_TRADABLE_ICON
#define WJ_ENABLE_BOSS_EFFECT
#define ENABLE_COSTUME_WEAPON_SYSTEM
#define ENABLE_MOUNT_COSTUME_SYSTEM
#define ENABLE_ACCE_COSTUME_SYSTEM	
#define ENABLE_QUIVER_SYSTEM		T
#define ENABLE_VIEW_TARGET_PLAYER_HP
#define ENABLE_VIEW_TARGET_DECIMAL_HP
#define ENABLE_COSTUME_ATTR_SYSTEM
#define ENABLE_TAB_NEXT_TARGET
#define ENABLE_ATTR_TRANSFER_SYSTEM
#define ENABLE_CHANGELOOK_SYSTEM
#define ENABLE_DESTROY_DROP_SYSTEM
#define ENABLE_SPECIAL_STORAGE
#define ELEMENT_NEW_BONUSES
#define ENABLE_REFINE_RENEWAL
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
+ When a private message is received, the icon of the taskbar will flash.
+ Enable boss effect over head.
+ Enable tradable icon like official.
+ Enable hightlight item effect like GF.
+ Enable new biolog system. 
+ Enable target color system.
+ Enable costume weapon system.
+ Enable costume follow mount system.
+ Enable shoulder sash costume system.
+ Enable quiver system. 
+ Enable view target player hp.
+ Enable view target decimal hp.
+ Enable costume attr system.
+ Enable tab next target.
+ Enable attr transfer system.
+ Enable changelook system.
+ Enable destroy drop dialog.
+ Enable special storage.
+ Enable officiel new elemental bonus.
```
## - New Fixes
```
+ "SEQUENCE mismatch 0xaf != 0x64 header 254" fix
+ Sell item to npc.
+ Ctrl+V crash when pasting images&co.
+ For do_view_equip
+ If the client can not connect to the server, the client will wait one second to connect the server again.
+ Fix crash client when you dont have arrow.
+ When a character is logging out from the game near to your character you can see a fast equipment change (the character is unequipping everything from him/herself)
+ When you move camera and minimize client in the same time mouse remains blocked and you need to maximize client , stop move camera and minimize again. I fixed this.
+ Fix the positions of textails (name position changes by every update packet on the main character), and also the position of the emotions when you are on a mount. 
+ If you click a monster without having arrows, the automatic attack will go in loop. I fixed this.
+ When Assignment of skill points when a skill is active fixed.
+ CMapOutdoor::Load - LoadMonsterAreaInfo fixed.
+ Quiver system: When you attack a target with space bar and you switch with arrow, client will crash, i fixed this. 
+ Quiver system: When you have costume weapon, or transmutated weapon, quiver effect is not working. I fixed this. 
```


