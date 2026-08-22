-Module:
No Unmarked Stashes Plus More Stash Loot [Kolaris]
https://www.moddb.com/mods/stalker-anomaly/addons/no-unmarked-stashes-plus-more-stash-loot

----------------------------------------------------------
-Compatibility:

Grok's Stash Overhaul already includes both features in its "No loot in unmarked stashes" option.

----------------------------------------------------------
-Explanation:

More Stash Loot component has been DLTX converted and split off. The original mod is not required, but disable its configs folder if you use it for the following.

The No Unmarked Stashes component has been monkey patched for convenience and compatibility, with an option to make unmarked stashes always be filled.

However, on one hand, do note you're basically loading an extra script for what's esentially a single number change. Bit by bit, you're clogging your your resources on a game where the main bottleneck is the CPU, so you should keep that in mind.

On the other hand, you may instead use the one in the original mod if you're not using any such mod. If you use Grok's Stash Overhaul, it includes its own option for it.

On a third, mutant tentacle, it's just better to manually tweak yourself whatever version of treasure_manager.script that is winning the load order in MO2.

To do so, find the winning treasure_manager.script and open it in your prefered notepad app, then find the line:
local function on_game_load()

At the end of that block, you'll find:
for i=1, math.floor(caches_count/x) do

You can change x for whatever value from 1 to 100 you want.

From no unmarked stashes:
for i=1, math.floor(caches_count/1) do

To always find unmarked stashes:
for i=1, math.floor(caches_count/100) do

----------------------------------------------------------
-Patches:

----------------------------------------------------------
-Known issues:
