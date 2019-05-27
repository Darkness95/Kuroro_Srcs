
# Changelog Kurorowork Client Source

- [Changelog Kuroro Client Source](#changelog-kurorowork-client-source)
  * [- New Defines / Systems](#--new-defines---systems)
  * [- Modification / Additions](#--modification---additions)
  * [- New Fixes](#--new-fixes)

## - New Defines / Systems
```	
#define ENABLE_INSTANT_QUEST_SPEED	
#define HIDE_GRANNY_SYSERR
#define ENABLE_MONSTERLEVEL
#define ENABLE_MONSTERSTERN
#define DISABLE_BOSS_FLY
#define CHARACTER_NAME_MAX_LEN	24
```
## - Modification / Additions
```
```
## - New Fixes
```
+ "SEQUENCE mismatch 0xaf != 0x64 header 254" fix
+ For do_view_equip (WEAR_MAX_NUM: server 32, client 11) now equal (32 both sides)		
+ Ymir forgot .m_dwVID in the format argument (c_rkCreateData -> c_rkCreateData.m_dwVID)
+ Player.IsValuableItem was selecting a wrong item.cell
+ If you (mouse) click a monster without having arrows, the automatic attack will go in loop (clicking on ground again will fix, but moving with WASD will be bad)
+ Regen.txt was loaded from launcher even though it's used only by the WorldEditor
+ To show the name of the failed mapped .dds load
+ The bottom pic was not shown
+ Ctrl+V crash when pasting images&co (no checks whether the handle was NULL or not)
+ Non-printing/control characters were printed in the (chat) input (the ones you get when you press Ctrl+<key> in game)
+ On arabic locales, the [HyperText code] (alias Prism code) could be edited pressing <Backspace>
+ A new texture was added where the last was put
+ A new textureset index was -1 instead of 0
```


