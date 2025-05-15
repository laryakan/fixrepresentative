# Fix Representative
This mod aim to force faction representative spawns. Or maybe you're a modder and don't want to bother about representative relocation ?

## What it does ?
*Works on all Vanilla and DLC factions since v1.2*

Each time you start a new game (or load one, normally), an mdscript will run an check if there is any missing faction representative. For example, this can happen if you use a mod that modify sector or cluster.
Some factions are less impacted than other. But for other, like Free Families, the representative is randomly placed on a whard, shipyard or equipment dock in FRF sectors : If a mod or a bug mess up with FRF sector, the representative could not spawn.

Then, the ForceReprensentative script dispatch the "Missing Representative Task Force", aka **MRTF**.
They will search for the representative and place it on a random station of the targ faction.

## Technically ?
The script will check existance of representative.
If a representative is missing, the script will check if the faction is active.
Then it will check if there is an eligible station for the representative to land on.
If none, the script will abort. But if there is one, the script will reset the default HQ settings for this factions, create the representative, create a room for him to sit in and place him inside it.

- github : https://github.com/laryakan/fixrepresentative
- nexus : https://www.nexusmods.com/x4foundations/mods/1702
- nexus user : https://next.nexusmods.com/profile/Laryakan
