
# Changelog Kurorowork Server Source

- [Changelog Kuroro Server Source](#changelog-kurorowork-server-source)
  * [- New Defines / Systems](#--new-defines---systems)
  * [- New Fixes](#--new-fixes)
  * [- New Questfunctions](#--new-questfunctions)
  * [- Removed Code](#--removed-code)

## - New Defines / Systems
```
```
## - New Fixes
```
+ Dungeon (core downer)
+ P2P Fix
+ Enable stackable books instead of remove all the pile
+ Guild exploit fix
+ Guild comment flood mysql ( delay 10 min )
+ Mobs in safezone
+ Attack on the markets
+ Guild yang control
+ Guild level control 
+ Adminpage exploit
+ Skill to remain active when skill reset
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
+ Kill a player (guerrier), `when kill begin` will be triggered twice
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
+ CShop class destructor wasn't virtual. If a derived class like CShopEx was deleted, a memory leak would have been generated.
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



