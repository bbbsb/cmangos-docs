Back to "world database":mangosdb_struct list of tables.

*See also "Creature_template_tbc":Creature_template_tbc  (for 2.4.3)*
*See also "Creature_template_classic":Creature_template_classic  (for 1.12.x)*

h2. The `creature&#95;template` table

This table contains the description of creatures. Each spawned creature is an instance of a template present in this table, this means every creature MUST be defined in this table.

h3. Structure


|*Field*|*Type*|*Null*|*Key*|*Default*|*Extra*|
|"entry":Creature_template#entry|mediumint(8) unsigned|NO|PRI|0||
|"difficulty_entry_1":Creature_template#difficulty_entry|mediumint(8) unsigned|NO||0||
|"difficulty_entry_2":Creature_template#difficulty_entry|mediumint(8) unsigned|NO||0||
|"difficulty_entry_3":Creature_template#difficulty_entry|mediumint(8) unsigned|NO||0||
|"KillCredit1":Creature_template#killcredit|INTEGER unsigned|NO||0||
|"KillCredit2":Creature_template#killcredit|INTEGER unsigned|NO||0||
|"modelid_1":Creature_template#modelid|mediumint(8) unsigned|NO||0||
|"modelid_2":Creature_template#modelid|mediumint(8) unsigned|NO||0||
|"modelid_3":Creature_template#modelid|mediumint(8) unsigned|NO||0||
|"modelid_4":Creature_template#modelid|mediumint(8) unsigned|NO||0||
|"name":Creature_template#name|char(100)|NO||0||
|"subname":Creature_template#subname|char(100)|YES||Null||
|"IconName":Creature_template#iconname|char(100)|YES||Null||
|"gossip_menu_id":Creature_template#gossip_menu_id|MENIUMINT(8)|YES||0||
|"minlevel":Creature_template#minlevel|tinyint(3) unsigned|YES||1||
|"maxlevel":Creature_template#maxlevel|tinyint(3) unsigned|YES||1||
|"minhealth":Creature_template#minhealth|int(10) unsigned|YES||0||
|"maxhealth":Creature_template#maxhealth|int(10) unsigned|YES||0||
|"minmana":Creature_template#minmana|int(10) unsigned|YES||0||
|"maxmana":Creature_template#maxmana|int(10) unsigned|YES||0||
|"armor":Creature_template#armor|mediumint(8) unsigned|NO||0||
|"faction_A":Creature_template#faction_a|smallint(5) unsigned|NO||0||
|"faction_H":Creature_template#faction_h|smallint(5) unsigned|NO||0||
|"npcflag":Creature_template#npcflag|int(10) unsigned|NO||0||
|"speed_walk":Creature_template#speed|float|YES||1||
|"speed_run":Creature_template#speed|float|YES||1.14286||
|"scale":Creature_template#scale|float|NO||0||
|"rank":Creature_template#rank|tinyint(3) unsigned|YES||0||
|"mindmg":Creature_template#mindmg|float|YES||0||
|"maxdmg":Creature_template#maxdmg|float|YES||0||
|"dmgschool":Creature_template#dmgschool|tinyint(4)|NO||0||
|"attackpower":Creature_template#attackpower|int(10) unsigned|NO||0||
|"dmg_multiplier":Creature_template#dmg_multiplier|float|NO||0||
|"baseattacktime":Creature_template#baseattacktime|int(10) unsigned|YES||0||
|"rangeattacktime":Creature_template#rangeattacktime|int(10) unsigned|YES||0||
|"unit_class":Creature_template#unit_class|int unsigned|NO||0||
|"unit_flags":Creature_template#unit_flags|int(10) unsigned|NO||0||
|"dynamicflags":Creature_template#dynamicflags|int(10) unsigned|NO||0||
|"family":Creature_template#family|tinyint(4)|YES||0||
|"trainer_type":Creature_template#trainer_type|tinyint(4)|YES||0||
|"trainer_spell":Creature_template#trainer_spell|mediumint(8) unsigned|YES||0||
|"trainer_class":Creature_template#trainer_class|tinyint(3) unsigned|YES||0||
|"trainer_race":Creature_template#trainer_race|tinyint(3) unsigned|YES||0||
|"minrangedmg":Creature_template#minrangedmg|float|NO||0||
|"maxrangedmg":Creature_template#maxrangedmg|float|NO||0||
|"rangedattackpower":Creature_template#rangedattackpower|smallint(5) unsigned|NO||0||
|"type":Creature_template#type|tinyint(3) unsigned|NO||0||
|"type_flags":Creature_template#type_flags|int(10) unsigned|YES||0||
|"lootid":Creature_template#lootid|mediumint(8) unsigned|NO||0||
|"pickpocketloot":Creature_template#pickpocketloot|mediumint(8) unsigned|NO||0||
|"skinloot":Creature_template#skinloot|mediumint(8) unsigned|NO||0||
|"resistance1":Creature_template#resistance1|int(10) unsigned|NO||0||
|"resistance2":Creature_template#resistance2|smallint(5)|NO||0||
|"resistance3":Creature_template#resistance3|smallint(5)|NO||0||
|"resistance4":Creature_template#resistance4|smallint(5)|NO||0||
|"resistance5":Creature_template#resistance5|smallint(5)|NO||0||
|"resistance6":Creature_template#resistance6|smallint(5)|NO||0||
|"PetSpellDataId":Creature_template#petspelldataid|mediumint(8) unsigned|NO||0||
|"mingold":Creature_template#mingold|mediumint(8) unsigned|NO||0||
|"maxgold":Creature_template#maxgold|mediumint(8) unsigned|NO||0||
|"AIName":Creature_template#ainame|char(64)|NO||||
|"MovementType":Creature_template#movementtype|tinyint(3) unsigned|NO||0||
|"InhabitType":Creature_template#inhabittype|tinyint(3) unsigned|NO||3||
|"unk16":Creature_template#unk16|float|NO||1.0||
|"unk17":Creature_template#unk17|float|NO||1.0||
|"RacialLeader":Creature_template#racialleader|tinyint(3) unsigned|NO||0||
|"questItem1":Creature_template#questitem|INTEGER|NO||0||
|"questItem2":Creature_template#questitem|INTEGER|NO||0||
|"questItem3":Creature_template#questitem|INTEGER|NO||0||
|"questItem4":Creature_template#questitem|INTEGER|NO||0||
|"questItem5":Creature_template#questitem|INTEGER|NO||0||
|"questItem6":Creature_template#questitem|INTEGER|NO||0||
|"movementId":Creature_template#movementid|INTEGER|NO||0||
|"RegenHealth":Creature_template#regenhealth|tinyint(3) unsigned|NO||1||
|"equipment_id":Creature_template#equipment_id|mediumint(8) unsigned|NO||0||
|"trainer_id":Creature_template#trainer_id|mediumint(8)|NO||0||
|"vendor_id":Creature_template#vendor_id|mediumint(8)|NO||0||
|"mechanic_immune_mask":Creature_template#mechanic_immune_mask|int(10) unsigned|NO||0||
|"flags_extra":Creature_template#flags_extra|int(10) unsigned|NO||0||
|"ScriptName":Creature_template#scriptname|char(64)|NO||||


h3. Description of the fields

h4. difficulty&#95;entry

If not zero, this field refers to an entry of creature&#95;template. Which suppose to be used in certain difficulty see below:


|DUNGEON&#95;DIFFICULTY&#95;NORMAL|0|
|DUNGEON&#95;DIFFICULTY&#95;HEROIC|1|
|RAID&#95;DIFFICULTY&#95;10MAN&#95;NORMAL|0|
|RAID&#95;DIFFICULTY&#95;25MAN&#95;NORMAL|1|
|RAID&#95;DIFFICULTY&#95;10MAN&#95;HEROIC|2|
|RAID&#95;DIFFICULTY&#95;25MAN&#95;HEROIC|3|


h4. modelid

Graphical model that the client applies on this creature. This is a "creature&#95;model&#95;info.entry":creature_model_info#entry

h4. name

Base name of the creature.

h4. subname

The subname of the creature that appears in &lt;&gt; below the creature's name.

h4. IconName

Script icon used by guards with directions menu.

h4. gossip&#95;menu&#95;id

Reference to a "gossip&#95;menu&#95;id":gossip_menu.

h4. minlevel

The minimum level of the creature if the creature has a level range.

h4. maxlevel

The maximum level of the creature if the creature has a level range. When added to world, a level in chosen in the specified level range.

h4. minhealth

The minimum health of the creature if the creature has variable health.

h4. maxhealth

The maximum health of the creature if the creature has a variable health. When added to world, the health value is chosen in proportion to the level chosen.

h4. minmana

The miminum mana of the creature if the creature has variable mana.

h4. maxmana

The maximum mana of the creature if the creature has variable mana. When added to world, the mana value is chosen in proportion to the level chosen.

h4. armor

The armor value of the creature. It controls how much damage reduction the creature gets from physical attacks.

h4. faction&#95;A

The faction if the creature is on the alliance side. See "FactionTemplate.dbc.":FactionTemplate.dbc. Just because more than one faction has the same name, the inter-faction relationships can be different.

Note: This field also controls the creature family assistance mechanic. Only creatures with the same faction will assist each other.

h4. faction&#95;H

The faction if the creature is on the horde side. See "FactionTemplate.dbc.":FactionTemplate.dbc. Just because more than one faction has the same name, the inter-faction relationships can be different.

Note: This field also controls the creature family assistance mechanic. Only creatures with the same faction will assist each other.

h4. npcflag

A bitmask that represents what NPC flags the creature has. Each bit controls a different flag and to combine flags, you can add each flag that you want, in effect activating the respective bits.

|_. Bit|_. Flag|_. Comment|
|1|Gossip|If creature has more gossip options, add this flag to bring up a menu.|
|2|Quest Giver|Any creature giving or taking quests needs to have this flag.|
|16|Trainer|Allows the creature to have a trainer list to teach spells|
|32|Trainer_Class|Allows the creature to have a class trainer list to teach spells.
(MUST USE WITH FLAG: 16)|
|64|Trainer_Profession|Allows the creature to have a profession trainer list to teach spells.
(MUST USE WITH FLAG: 16)|
|128|Vendor|Any creature selling items needs to have this flag.|
|256|Vendor_Ammo|Any creature selling ammo items needs to have this flag. 
(MUST USE WITH FLAG: 128)|
|512|Vendor_Food|Any creature selling food items needs to have this flag.
(MUST USE WITH FLAG: 128)|
|1024|Vendor_Poison|Any creature selling poison items needs to have this flag.
(MUST USE WITH FLAG: 128)|
|2048|Vendor_Reagent|Any creature selling reagent items needs to have this flag.
(MUST USE WITH FLAG: 128)|
|4096|Repairer|Creatures with this flag can repair items.|
|8192|Flight Master|Any creature serving as fly master has this.|
|16384|Spirit Healer|Makes the creature invisible to alive characters and has the resurrect function.|
|32768|Spirit Guide||
|65536|Innkeeper|Creatures with this flag can set hearthstone locations.|
|131072|Banker|Creatures with this flag can show the bank|
|262144|Petitioner||
|524288|Tabard Designer|Allows the designing of guild tabards.|
|1048576|Battlemaster|Creatures with this flag port players to battlegrounds.|
|2097152|Auctioneer|Allows creature to display auction list.|
|4194304|Stable Master|Has the option to stable pets for hunters.|
|16777216|Instantloot|NPC could be loot immediately without killing, just after clicking on it. (Npc&#95;spellclick&#95;spells)|
|33554432|Player Vehicle|players with mounts that have vehicle data should have it set|
|268435456|Guard ???? |Creatures with this flag act as guards in cities.|


So if you want an NPC that is a quest giver, a vendor, and can repair you just add the specific flags together: 1 + 2 + 128 + 4096 = 4227.

h4. speed

Controls how fast the creature can move in a certain mode.

h4. scale

If non-zero, this field defines the size of how the model of the creature appears ingame. If zero, it will use default model size taken from the DBC.

h4. rank

The rank of the creature:

|_. Rank|_. Name|_. Comments|
|0|Normal||
|1|Elite|Higher damage, more health, better loot.|
|2|Rare Elite|A rare mob but with elite damage and health.|
|3|World Boss|Highest rank, best loot, longest respawn time.|
|4|Rare|Somewhat better loot, longer respawn time.|


h4. mindmg

Minimum damage the creature deals in melee. This field is combined with the "attackpower":#attackpower field to calculate the damage. Look at "attackpower":#attackpower to see the formula.

h4. maxdmg

Maximum damage the creature deals in melee. This field is combined with the "attackpower":#attackpower field to calculate the damage. Look at "attackpower":#attackpower to see the formula.

h4. dmgschool

Creature's melee damage school.

|_. ID|_. Name|
|0|SPELL&#95;SCHOOL&#95;NORMAL|
|1|SPELL&#95;SCHOOL&#95;HOLY|
|2|SPELL&#95;SCHOOL&#95;FIRE|
|3|SPELL&#95;SCHOOL&#95;NATURE|
|4|SPELL&#95;SCHOOL&#95;FROST|
|5|SPELL&#95;SCHOOL&#95;SHADOW|
|6|SPELL&#95;SCHOOL&#95;ARCANE|


h4. attackpower

The attack power for the creature's melee attacks. This field along with "mindmg":#mindmg and "maxdmg":#maxdmg dictate how much the creature will hit for. The formula in applying correct damages is as follows:

bc. UPDATE `creature_template` SET 
    `mindmg` = <#1>, 
    `maxdmg` = <#2>, 
    `attackpower` = ROUND((`mindmg` + `maxdmg`) / 4 * 7), 
    `mindmg` = ROUND(`mindmg` - `attackpower` / 7), 
    `maxdmg` = ROUND(`maxdmg` - `attackpower` / 7) 
  WHERE `entry` = ...


In the query above, substitute '&lt;#1&gt;' with the minimum damage you want the creature to deal and '&lt;#2&gt;' with the maximum damage you want the creature to deal.

NOTE: You might also want to double check the values calculated after the query is run because if the difference between mindmg and maxdmg is too high, mindmg will end up being a negative value.

h4. baseattacktime

Creature's melee attack time in milliseconds.

h4. rangeattacktime

h4. unit&#95;class

The NPC Class. There Are Only 4 classes available to creatures.

|_. ID|_. Name|
|CLASS&#95;WARRIOR|1|
|CLASS&#95;PALADIN|2|
|CLASS&#95;ROGUE|4|
|CLASS&#95;MAGE|8|

This Value is Contained in Sniff Data: UNIT_FIELD_BYTES_0 located in SMSG_UPDATE_OBJECT
It is a Critical Field in Determining Class Level Stats For the NPC

h4. unit&#95;flags

Allows the manual application of unit flags to creatures. Again this is a bitmask field and to apply more than one flag, just add the different numbers. Some possible flags are:


|*Flag*|*Name*|*Comments*|
|1|UNIT&#95;FLAG&#95;UNK&#95;0||
|2|UNIT&#95;FLAG&#95;NON&#95;ATTACKABLE||
|4|UNIT&#95;FLAG&#95;DISABLE&#95;MOVE||
|8|UNIT&#95;FLAG&#95;PVP&#95;ATTACKABLE|(allow apply pvp rules to attackable state in addition to faction dependent state)|
|16|UNIT&#95;FLAG&#95;RENAME||
|32|UNIT&#95;FLAG&#95;RESTING||
|64|UNIT&#95;FLAG&#95;UNK&#95;6||
|128|UNIT&#95;FLAG&#95;NOT&#95;ATTACKABLE&#95;1|(??) ((UNIT&#95;FLAG&#95;PVP&#95;ATTACKABLE + UNIT&#95;FLAG&#95;NOT&#95;ATTACKABLE&#95;1) is NON&#95;PVP&#95;ATTACKABLE)|
|256|UNIT&#95;FLAG&#95;OOC&#95;NOT&#95;ATTACKABLE|(2.0.8 - Can not be attacked when not in combat. Removed if unit for some reason enter combat.) (2.4.3, Seems to make the unit unattackable)|
|512|UNIT&#95;FLAG&#95;PASSIVE|(makes unable to attack everything. Almost identical to &quot;civilian&quot;. Will not engage in combat unless &quot;called upon&quot; or engaged by another unit.)|
|1024|UNIT&#95;FLAG&#95;LOOTING|(loot animation)|
|2048|UNIT&#95;FLAG&#95;PET&#95;IN&#95;COMBAT|(in combat?, 2.0.8)|
|4096|UNIT&#95;FLAG&#95;PVP|Allows item spells to be casted upon (?)|
|8192|UNIT&#95;FLAG&#95;SILENCED|Can't cast spells|
|16384|UNIT&#95;FLAG&#95;UNK&#95;14|(2.0.8)|
|32768|UNIT&#95;FLAG&#95;UNK&#95;15||
|65536|UNIT&#95;FLAG&#95;UNK&#95;16||
|131072|UNIT&#95;FLAG&#95;PACIFIED||
|262144|UNIT&#95;FLAG&#95;DISABLE&#95;ROTATE|(stunned, 2.1.1)|
|524288|UNIT&#95;FLAG&#95;IN&#95;COMBAT||
|1048576|UNIT&#95;FLAG&#95;TAXI&#95;FLIGHT|(disable casting at client side spell not allowed by taxi flight (mounted?), probably used with 0x4 flag)|
|2097152|UNIT&#95;FLAG&#95;DISARMED|(disable melee spells casting..., &quot;Required melee weapon&quot; added to melee spells tooltip.)|
|4194304|UNIT&#95;FLAG&#95;CONFUSED||
|8388608|UNIT&#95;FLAG&#95;FLEEING||
|16777216|UNIT&#95;FLAG&#95;PLAYER&#95;CONTROLLED|(used in spell Eyes of the Beast for pet...)|
|33554432|UNIT&#95;FLAG&#95;NOT&#95;SELECTABLE|Can't be selected by mouse|
|67108864|UNIT&#95;FLAG&#95;SKINNABLE||
|134217728|UNIT&#95;FLAG&#95;MOUNT|(the client seems to handle it perfectly)|
|268435456|UNIT&#95;FLAG&#95;UNK&#95;28||
|536870912|UNIT&#95;FLAG&#95;UNK&#95;29|(used in Feing Death spell)|
|1073741824|UNIT&#95;FLAG&#95;SHEATHE||
|2147483648|UNIT&#95;FLAG&#95;UNK&#95;31|(set skinnable icon and also changes color of portrait)|


h4. dynamicflags

Flags that control visual appearance of the creature.

A few known flags and their use are:


|*Flag*|*Name*|*Comments*|
|0|UNIT&#95;DYNFLAG&#95;NONE||
|1|UNIT&#95;DYNFLAG&#95;LOOTABLE||
|2|UNIT&#95;DYNFLAG&#95;TRACK&#95;UNIT||
|4|UNIT&#95;DYNFLAG&#95;OTHER&#95;TAGGER|Makes creatures name appear grey (good for simulating dead creatures)|
|8|UNIT&#95;DYNFLAG&#95;ROOTED||
|16|UNIT&#95;DYNFLAG&#95;SPECIALINFO|Shows creatures basic stats (Health, damage, resistances, tamable).|
|32|UNIT&#95;DYNFLAG&#95;DEAD|Makes the creature appear dead (this DOES NOT make the creatures name grey)|
|64|UNIT&#95;DYNFLAG&#95;TAPPED&#95;BY&#95;ALL&#95;THREAT&#95;LIST||


h4. family

The family this creature belongs to. Only used if "type":#type is 1 (Beast).

|_. ID|_. Family|_. ID|_. Family|_. ID|_. Family|
|1|Wolf|15|Doomguard|29|Nether Ray|
|2|Cat|16|Scorpid|30|Serpent|
|3|Spider|17|Turtle|31|Moth|
|4|Bear|18|Imp|32|Chimaera|
|5|Boar|19|Bat|33|Devilsaur|
|6|Crocolisk|20|Hyena|34|Ghoul|
|7|Carrion Bird|21|Bird of Prey|35|Silithid|
|8|Crab|22|Wind Serpent|36|Worm|
|9|Gorilla|23|Remote Control|37|Rhino|
|10|Raptor|24|Felguard|38|Wasp|
|11|Tallstrider|25|Dragonhawk|39|Core Hound|
|12|Felhunter|26|Ravager|40|Spirit Beast|
|13|Voidwalker|27|Warp Stalker|
|14|Succubus|28|Sporebat|


h4. trainer&#95;type

If the NPC is a trainer (has the trainer flag), then this field controls what kind of trainer it is. Both this field and the related field must be filled in for a trainer to work correctly.

|_. ID|_. Type|_. Related Field|_. Comments|
|0|TRAINER&#95;TYPE&#95;CLASS|trainer&#95;class|Trains class spells|
|1|TRAINER&#95;TYPE&#95;MOUNTS|trainer&#95;race|Trains riding skill|
|2|TRAINER&#95;TYPE&#95;TRADESKILLS|trainer&#95;spell|Trains professions|
|3|TRAINER&#95;TYPE&#95;PETS|trainer&#95;class|Trains pet skills|


h4. trainer&#95;spell

If the NPC is a trainer that teaches professions ("trainer&#95;type":creature_template#trainer_type == 2), then the player must already know the spell ID specified here to be able to talk to this NPC.

h4. trainer&#95;class

If the NPC is a class trainer or a pet trainer ("trainer&#95;type":creature_template#trainer_type == 0 or 3), then the player's class must be the same as the value specified here to talk to this trainer. For pet trainers, this value must be 3 (hunter). See "character.class":character#class

h4. trainer&#95;race

If the NPC is a mount trainer ("trainer&#95;type":creature_template#trainer_type == 1), then the player's race must be the same as the value specified here to talk to this trainer. See "character.race":character#race

h4. minrangedmg

Minimum ranged damage the creature inflicts.

NOTE: This is Damage Inflicted From RANGED WEAPON ATTACK ONLY (Cross-Bow Arrows, Knives, Thrown Axes, ect)

h4. maxrangedmg

Maximum range damage the creature inflicts.

NOTE: This is Damage Inflicted From RANGED WEAPON ATTACK ONLY (Cross-Bow Arrows, Knives, Thrown Axes, ect)

h4. rangedattackpower

h4. type

The type of the creature.

|_. ID|_. Type|
|0|None|
|1|Beast|
|2|Dragonkin|
|3|Demon|
|4|Elemental|
|5|Giant|
|6|Undead|
|7|Humanoid|
|8|Critter|
|9|Mechanical|
|10|Not specified|
|11|Totem|
|12|Non-combat Pet|
|13|Gas Cloud|


h4. type&#95;flags

This field can control whether a mob is minable or herbable. If it is either of those two, then the loot given when it is skinned/mined will be stored in the "skinning_loot_template":skinning_loot_template table. Aside from those two flags, field has no special meaning on the serverside. It will be send to the client in SMSG&#95;CREATURE&#95;QUERY&#95;RESPONSE

Some values provided from the community:


|*Flag*|*Name*|*Comments*|
|1||Makes the mob tameable (must also be a beast and have family set)|
|2|UNIT&#95;FLAG&#95;NOT&#95;ATTACKABLE||
|8|UNIT&#95;FLAG&#95;ATTACKABLE||
|128|UNIT&#95;FLAG&#95;NOT&#95;ATTACKABLE&#95;1||
|136|UNIT&#95;FLAG&#95;NON&#95;PVP&#95;PLAYER||
|256||Makes mob herbable|
|512||Makes mob minable|
|1024|UNIT&#95;FLAG&#95;ANIMATION&#95;FROZEN||
|4096|UNIT&#95;FLAG&#95;WAR&#95;PLAYER||


h4. lootid

The ID of the loot template ID that this creature should use to generate loots. See "creature&#95;loot&#95;template.entry":creature_loot_template#entry

h4. pickpocketloot

The ID of the pickpocketing loot template that this creature should use to generate pickpocketing loots. See "pickpocketing&#95;loot&#95;template.entry":pickpocketing_loot_template#entry

h4. skinloot

The ID of the skinning loot template that this creature should use to generate skinning loots. See "skinning&#95;loot&#95;template.entry":skinning_loot_template#entry

h4. resistance1

Holy resistance.

h4. resistance2

Fire resistance.

h4. resistance3

Nature resistance.

h4. resistance4

Frost resistance.

h4. resistance5

Shadow resistance.

h4. resistance6

Arcane resistance.

h4. PetSpellDataId

ID that displays what spells the pet has in the client.

h4. mingold

Minimum money that the creature drops when killed, in copper.

h4. maxgold

Maximum money that the creature drops when killed, in copper.

h4. AIName

Overrides AI used for the creature.

|_. Name|_. Description|
|NullAI|Empty AI, creature does nothing.|
|AggressorAI|Creature attacks as soon as something is in aggro range.|
|ReactorAI|Creature attacks only if aggroed by attack, spell etc.|
|GuardAI||
|PetAI|Creature is a pet.|
|TotemAI|Creature casts spell from field spell1, otherwise like NullAI.|
|EventAI|Creature uses event based AI.|
||


h4. MovementType

The creature's default movement type.

|_. ID|_. Type|
|0|Idle; stay in one place|
|1|Random movement inside the spawndist radius|
|2|Waypoint movement|


h4. InhabitType

Controls where the creature can move and attack.

|_. ID|_. Type|
|1|Ground only|
|2|Water only|
|3|Both ground and water|
|4|Flying|


h4. unk16

Float values with unknown meaning. Values are from WDB Files.

h4. unk17

Float values with unknown meaning. Values are from WDB Files.

h4. questItem

The entry of the "item":item_template that creature drops and is required within an active quest.

h4. RacialLeader

A flag indicating wheather the creature is a racial leader. Killing racial leaders grants 100 honor.

h4. RegenHealth

Boolean 1 or 0 controlling if the creature should regenerate its health or not.

h4. equipment&#95;id

The default ID of the equipment that this creature should display. See "creature&#95;equip&#95;template.entry":creature_equip_template#entry

h4. trainer&#95;id

The id refers to the "npc_trainer_template.":npc_trainer_template.

h4. vendor&#95;id

The id refers to the "npc_vendor_template.":npc_vendor_template.

h4. mechanic&#95;immune&#95;mask

This makes the creature immune to specific spell natures. See Spell.dbc at row effect&#95;X&#95;mechanic&#95;id.

Uses references from SpellMechanic.dbc.

|_. Bit|_. Type|_. Bit|_. Type|
|1|MECHANIC&#95;CHARM|32768|MECHANIC&#95;BANDAGE|
|2|MECHANIC&#95;CONFUSED|65536|MECHANIC&#95;POLYMORPH|
|4|MECHANIC&#95;DISARM|131072|MECHANIC&#95;BANISH|
|8|MECHANIC&#95;DISTRACT|262144|MECHANIC&#95;SHIELD|
|16|MECHANIC&#95;FEAR|524288|MECHANIC&#95;SHACKLE|
|32|MECHANIC&#95;FUMBLE|1048576|MECHANIC&#95;MOUNT|
|64|MECHANIC&#95;ROOT|2097152|MECHANIC&#95;PERSUADE|
|128|MECHANIC&#95;PACIFY|4194304|MECHANIC&#95;TURN|
|256|MECHANIC&#95;SILENCE|8388608|MECHANIC&#95;HORROR|
|512|MECHANIC&#95;SLEEP|16777216|MECHANIC&#95;INVULNERABILITY|
|1024|MECHANIC&#95;SNARE|33554432|MECHANIC&#95;INTERRUPT|
|2048|MECHANIC&#95;STUN|67108864|MECHANIC&#95;DAZE|
|4096|MECHANIC&#95;FREEZE|134217728|MECHANIC&#95;DISCOVERY|
|8192|MECHANIC&#95;KNOCKOUT|268435456|MECHANIC&#95;IMMUNE&#95;SHIELD|
|16384|MECHANIC&#95;BLEED|536870912|MECHANIC&#95;SAPPED|


To combine immunities just add values. Immune to everything corresponds to the value 1073741823.

h4. flags&#95;extra

These flags control certain creature specific attributes.

|_. Bit|_. Name|_. Description|
|1|CREATURE&#95;FLAG&#95;EXTRA&#95;INSTANCE&#95;BIND|Bounds killer's party to the instance they are in|
|2|CREATURE&#95;FLAG&#95;EXTRA&#95;CIVILIAN|Makes creature ignore aggro|
|4|CREATURE&#95;FLAG&#95;EXTRA&#95;NO&#95;PARRY|Prohibits creature from parrying|
|8|CREATURE&#95;FLAG&#95;EXTRA&#95;NO&#95;PARRY&#95;HASTEN|Creatures parries do not speed up its next attack|
|16|CREATURE&#95;FLAG&#95;EXTRA&#95;NO&#95;BLOCK|Prohibits creature from blocking|
|32|CREATURE&#95;FLAG&#95;EXTRA&#95;NO&#95;CRUSH|Prohibits creature from dealing crushing blows|
|64|CREATURE&#95;FLAG&#95;EXTRA&#95;NO&#95;XP&#95;AT&#95;KILL|Makes creature reward no XP at kill|
|128|CREATURE&#95;FLAG&#95;EXTRA&#95;INVISIBLE|Makes creature invisible for player. Use this for triggers etc.|
|256|CREATURE&#95;FLAG&#95;EXTRA&#95;NOT&#95;TAUNTABLE|creature is immune to taunt auras and effect attack me|
|512|CREATURE&#95;FLAG&#95;EXTRA&#95;AGGRO&#95;ZONE|creature sets itself in combat with zone on aggro|
|1024|CREATURE&#95;FLAG&#95;EXTRA&#95;GUARD|creature is a guard, for Zone under attack announce if guard death|
|2048|CREATURE&#95;FLAG&#95;EXTRA&#95;NO&#95;TALKTO&#95;CREDIT|creature doesn't give quest-credits when talked to (temporarily flag).|


h4. ScriptName

The name of the script that this creature uses, if any. This ties a script from a scripting engine to this creature.