-Module:
Hunter Survival Crafting [unwary]
https://www.moddb.com/mods/stalker-anomaly/addons/hunter-survival-crafting

----------------------------------------------------------
-Compatibility:
NOTE: You still need the original mods. Disable the configs and textures/ui folders.

IMPORTANT: If you were already using this mod in a current save, a new game is required.

Banjaji's Crafting System Improvement:
required for the recipes, as they are too complex for the vanilla system.

Hunter's Kit - A Butchery Engine:
Currently both mods conflict. Have Hunter's Kit on a higher priority than HSC in your load order, so its rework of the ui_mutant_loot.script file takes priority. Or disable this mod and module's ui_mutant_loot.script

Reinforced Cordon:
Redundant with the Unique NPC Loot component, which will overwrite it anyway.

Less Infuriating Hip
Stashes to named NPCs
Additional changes will be done by the Unique NPC Loot component if these mods are present.

Connelly's Unifying Nosorog Tweaks
It will detect if the Unique NPC Loot module here is present.

----------------------------------------------------------
-Explanation:

-Items and crafting
DLTX conversion of several files that hadn't been done so by the original mod yet, and un-DLTX'fying of several items that didn't need it.
The crafted medkits and stimpack are supposed to be inferior improvisations of the vanilla imported items. They will all now be cheaper and heavier than the vanilla items (the heavy medkit having a value of 8500 roubles above was just silly). The stimpack has also been nerfed to heal less.
Small text corrections.
Mipmapped some textures that could use it.
The FDDA patch has been integrated into the main files.

Added default actor effects configs.

-Unique NPC Loot
DLTX and DXML conversion. Still requires the Items and crafting component above.
Turned its copy of itms_manager.script into a monkey patch.
Do note the DXML file will overwrite the inventory (not the worn outfit) of various NPCs. If you have any mod also doing it, consider their filenames make them load in alphabetic order.
Its copy of hxf_tough_important_npcs.script has been updated to the last version of "Tougher Important NPCs and Companions", and made optional for compatibility with Skyki's Fair Story NPC Protection.

-Unique NPC Loot - Everyone is hostile
Unavailable for now. (also, feature creep?)


Integration into:
aLifeTactics
Cold System
More drops from drugs (DLTX Minimod)
NPCs Limping and Healing


----------------------------------------------------------
-Patches:

Original patches have been DLTX'd where possible and needed.

Fillable Canteens
Cook flasks, tea, and tactical tuna.

Placeable Campfires
Craft campfires.

Syringes from medkits
After using a medkit, you'll receive a spare empty syringe. This affects both the new and the vanilla medkits.
In addition to the medkits, now the improvised morphine and stimpacks also provides a syringe.
Do not use with the More drops from drugs patch below, as its redundant.

No drug limit
Merges the changes in itms_manager.script with those in nb79's mod, removing the 'there is a greater effect in place' restriction. nb79's No drug limit is not needed with this and you may disable it.

Unique NPC Loot - MAS
Merges changes from both mods to itms_manager.script

----------------------------------------------------------
-Known issues:
