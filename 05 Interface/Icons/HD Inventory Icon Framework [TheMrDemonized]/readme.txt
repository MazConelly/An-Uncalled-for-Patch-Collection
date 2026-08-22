-Module:
HD Inventory Icon Framework [TheMrDemonized]
https://www.moddb.com/mods/stalker-anomaly/addons/hd-inventory-icons-framework

----------------------------------------------------------
-Compatibility:

----------------------------------------------------------
-Explanation:

----------------------------------------------------------
-Patches:

Compatibility safety for unpatched items
This patch doesn't include actual HD icons.
When the framework is used to patch an item, the changes to any section (item) go downstream. Any daughter sections will appear messed up in some way, for example their icons looking reduced in size.
In some cases, removing their inheritances is required as they would also inherit the new icon and coordinates, messing them up.
For others, adding a "inv_grid_scale = 1" line to their sections is enough to solve this.

This patch cover these currently known cases:
	Vanilla filled artefact containers
	Belt Glowsticks
	Hunter Survival Crafting
	Faction Medkits
	Heatvision
	Perk Based Artefacts
	Storylines
	New backpacks
	Backpacks of the Zone
	Data's New Backpacks
	Sen_nz's Upgradeable Backpacks

Any actual patch for the framework should be able to override this through DLTX:
	mod_system_a_hdicon_safety_items.ltx

----------------------------------------------------------
-Known issues:
